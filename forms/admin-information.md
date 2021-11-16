---
title: Administratorinformationen
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Dieser Artikel beantwortet die am häufigsten gestellten Fragen zu Administratorinformationen für Microsoft Forms.
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951487"
---
# <a name="admin-information"></a>Administratorinformationen

## <a name="getting-started"></a>Erste Schritte

**Wie kann ich Microsoft Forms deaktivieren oder aktivieren?**

Standardmäßig ist Microsoft Forms für alle Benutzer in einer Organisation aktiviert. Microsoft 365 IT-Administratoren können Microsoft Forms im Microsoft 365 Admin Center auf der Registerkarte **Benutzerverwaltung** deaktivieren. Weitere Informationen finden Sie unter [Einrichten von Microsoft Forms](set-up-microsoft-forms.md) und [Deaktivieren oder Aktivieren von Microsoft Forms](turn-off-turn-on-microsoft-forms.md).

**Wie kann ich den Zugriff auf Microsoft Forms nur für bestimmte Personen in meiner Organisation zulassen?**

Administratoren können Zugriffsberechtigungen für bestimmte Personen in der Organisation ändern. Siehe [Administratoreinstellungen in Microsoft Forms](administrator-settings-microsoft-forms.md).

## <a name="data-storage"></a>Datenspeicher

**Wo werden Daten für Microsoft Forms gespeichert?**

Microsoft Forms-Daten werden auf Servern in den USA gespeichert, mit Ausnahme von Daten für in Europa ansässige Mandanten. Die Daten für in Europa ansässige Mieter werden auf Servern in Europa gespeichert.

## <a name="user-activity"></a>Benutzeraktivität

**Wie kann ich sehen, welche Aktivitäten in Microsoft Forms von Personen in meiner Organisation ausgeführt werden?**

Sie können [Microsoft Forms-Aktivitäten](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities) im [Microsoft 365 Security Center](https://security.microsoft.com/?rfr=OfficeScc)-Überwachungsprotokoll überprüfen. Erfahren Sie mehr über die [Überwachung in Office 365 (für Administratoren)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906).

## <a name="user-account-information"></a>Benutzerkontoinformationen

**Wie kann ich überprüfen, ob ein Benutzerkonto „endgültig gelöscht“ wurde?**

1. Administratoren können sich bei [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer) anmelden.

2. Fügen Sie im oberen Suchfeld die folgende URL ein:

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*user email* = E-Mail-Adresse des Formularbesitzers, der Ihre Organisation verlassen hat und/oder dessen Konto deaktiviert wurde

3. Klicken Sie auf **Abfrage ausführen**.

Wenn die gesuchten Kontoinformationen in Ihrer Abfrage zurückgegeben werden, bedeutet dies, dass das Konto vorläufig gelöscht wurde und innerhalb der 30-Tage-Frist liegt. Ein globaler Administrator kann die Formulare, die dem vorläufig gelöschten Konto gehören, wie zuvor beschrieben mithilfe der Übertragungsmethode übertragen.

Wenn die gesuchten Kontoinformationen in Ihrer Abfrage nicht zurückgegeben werden, bedeutet dies, dass das Konto im Office 365 Mandanten noch vorhanden ist oder vor mehr als 30 Tagen gelöscht wurde. Wenn das Konto im Office 365 Mandanten vorhanden oder deaktiviert ist, kann ein globaler Administrator die Formulare, die dem Konto gehören, übertragen. Wenn das Konto aus dem Office 365 Mandanten "endgültig gelöscht" wurde, kann ein globaler Administrator die Formulare, die diesem Kontos gehörten, nicht übertragen. Diese Formulare können auch nicht wiederhergestellt werden.

**Ist die Anzahl der Benutzer und die Datenmenge, die für Benutzerkonten gespeichert werden, auch nach dem Verlassen meiner Organisation begrenzt?**

Derzeit gibt es keine Begrenzung für die Anzahl der Benutzer, für die Daten aufbewahrt werden, solange die Bereitstellung ihrer Konten im Rahmen der Onlinedienstvereinbarung Ihrer Organisation erfolgt. Auch die Menge der gespeicherten Daten für Benutzerkonten ist nicht begrenzt.

**Was geschieht mit den Daten eines Formulars, wenn die Microsoft Forms-Lizenz des Besitzers entfernt wurde oder der Benutzer deaktiviert oder aus Ihrem Mandanten gelöscht wird (Azure AD)?**

Wenn die Besitzerlizenz entfernt wurde oder das Konto des Besitzers deaktiviert ist, gibt es keine Änderung für die für das Benutzerkonto gespeicherte Datenmenge.

Wenn ein Benutzerkonto aus Ihrem Mandanten gelöscht wurde (Azure AD), werden alle kontobezogenen Daten 30 Tage nach dem Löschen des Benutzers gelöscht.

## <a name="form-ownership-transfer"></a>Übertragung des Formularbesitzes

**Der ursprüngliche Besitzer eines Formulars ist nicht mehr bei meiner Organisation. Wie kann ich den Besitz des Formulars übertragen?**

Um das Formular einer Person zu übertragen, die Ihre Organisation verlassen hat, müssen die folgenden Anforderungen erfüllt sein:

  - Sie sind der globale Administrator der Organisation und verfügen über eine gültige Formularlizenz.

  - Der Mitarbeiter, dessen Formular Sie übertragen möchten, verfügt über ein Konto, das gelöscht oder deaktiviert wurde.

  - Das Formular wird innerhalb von 30 Tagen nach dem Löschen eines Kontos übertragen.

> [!Note]
> Es gibt keine Zeiteinschränkung, um den Besitz eines Formulars von einem Konto zu übertragen, das deaktiviert (und nicht gelöscht) wurde.

1. Wenn alle Anforderungen erfüllt sind, können Sie den Formularbesitz übertragen. Ersetzen Sie in der Adressleiste Ihres Browsers die vorhandene URL durch Folgendes:

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*user email* = E-Mail-Adresse des Formularbesitzers, der Ihre Organisation verlassen hat und/oder dessen Konto deaktiviert wurde
   > Wenn beispielsweise der Formularbesitzer („Jason Fabian“) Ihre Organisation („Contoso“) verlassen hat, sieht die URL für die Problemumgehung wie folgt aus: `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. Sie haben nun Zugriff auf die Formulare des ehemaligen Mitarbeiters. Klicken Sie auf dem Formular, das Sie übertragen möchten, auf die Schaltfläche **Weitere Formularaktionen**![ Weitere Optionen](./media/image2.png) und dann auf **Verschieben**.

   >[!Note]
   >Wenn Sie versuchen, den Besitz des Formulars an einen derzeit aktiven Mitarbeiter in Ihrer Organisation zu übertragen, können Sie es in eine Gruppe verschieben, der er angehört. Wenn Sie noch kein Mitglied dieser Gruppe sind, müssen Sie dieser beitreten, um die Übertragung durchzuführen. Nachdem die Übertragung des Formularbesitzes abgeschlossen ist, können Sie die Gruppe verlassen.

**Warum erhalte ich einen Fehler, wenn ich versuche, den Besitz eines Formulars zu übertragen?**

Wenn eine Fehlermeldung angezeigt wird, kann eine der folgenden Optionen sie daran hindern, den Besitz zu übertragen:

|Fehlermeldung|Erklärung|
| --- | --- |
| ***Wir können nicht auf diese Seite zugreifen***<br/><br/>Der Formularbesitzer verfügt weiterhin über ein aktives Konto. | Der Besitzer des Formulars verfügt weiterhin über eine aktive Formularlizenz und ein aktives Konto. |
| ***Wir können nicht auf diese Seite zugreifen***<br/><br/>Vergewissern Sie sich, dass Sie die E-Mail-Adresse richtig eingegeben haben und dass das Konto des Formularbesitzers nicht vor mehr als 30 Tagen gelöscht wurde. | Die E-Mail-Adresse ist falsch geschrieben und/oder das Konto des Formularbesitzers wurde vor mehr als 30 Tagen gelöscht. |
| ***Wir können nicht auf diese Seite zugreifen***<br/><br/>Vergewissern Sie sich, dass Sie die E-Mail-Adresse richtig eingegeben haben, und versuchen Sie es dann erneut. | Die E-Mail-Adresse fehlt oder ist falsch geschrieben. |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Formularverwendung in Outlook oder PowerPoint

**Personen in meiner Organisation können einer Outlook E-Mail-Nachricht keine Abstimmung hinzufügen. Wie kann ich dies beheben?**

Die Einstellung **Moderne Authentifizierung** für Outlook muss aktiviert sein, um sicherzustellen, dass Personen in Ihrer Organisation [eine Abstimmung in Outlook erstellen](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0) können.

1. Melden Sie sich bei [https://admin.microsoft.com](https://admin.microsoft.com/) mit Ihrem Geschäfts- oder Schulkonto an.

2. Wählen Sie **Einstellungen** \> **Organisationseinstellungen** aus.

   >[!Note]
   > Wenn die Option **Einstellungen** nicht angezeigt wird, wählen Sie im linken Bereich die Schaltfläche ![Weitere Optionen](./media/image2.png)**Alles anzeigen** aus.

3.  Wählen Sie die Option **Moderne Authentifizierung** aus.

4.  Aktivieren Sie die Option **Moderne Authentifizierung für Outlook 2013 für Windows und höher aktivieren (empfohlen)**.

Erfahren Sie mehr über die moderne und die [mehrstufige Authentifizierung](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide) und darüber, wie Sie sie einrichten und in Ihre rOrganisation bereitstellen.

**Ich möchte Office-Add-Ins nicht für meine gesamte Organisation bereitstellen. Können Personen in meiner Organisation das Formular-Add-In weiterhin für PowerPoint verwenden?**

Ja, Sie können die [zentrale Bereitstellung](/office/dev/add-ins/publish/centralized-deployment) verwenden, um nur das Forms-Add-In für PowerPoint bereitzustellen.

1.  Melden Sie sich bei [https://admin.microsoft.com](https://admin.microsoft.com/) mit Ihrem Geschäfts- oder Schulkonto an.

2.  Wählen Sie **Einstellungen** \> **Add-Ins** aus.

    >[!Note]
    >Wenn die Option **Einstellungen** nicht angezeigt wird, wählen Sie im linken Bereich die Schaltfläche ![Weitere Optionen](./media/image2.png)**Alles anzeigen** aus.

3.  Wählen Sie in der **Add-Ins**-List die Option **Formulare** aus.

4.  Wählen Sie im Bereich **Formulare bearbeiten** unter **Benutzer zuweisen** die Option **Jeder** aus.

5.  Klicken Sie auf **Speichern**.


## <a name="forms-and-anti-phishing"></a>Formulare und Antiphishing

**Was kann ich gegen Phishing und potenzielle böswillige Absichten in Formularen in meinem Mandanten tun?**

In Microsoft Forms ermöglichen wir automatisierten Computerüberprüfungen, die bösartige Sammlung vertraulicher Daten in Formularen proaktiv zu erkennen und diese Formulare vorübergehend für die Sammlung von Antworten zu sperren.

Erfahren Sie mehr über [Microsoft Forms und proaktives Verhindern von Phishing](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

Wenn Sie ein globaler und/oder Sicherheitsadministrator sind, können Sie sich bei der Microsoft 365 Admin Center unter [admin.microsoft.com](https://admin.microsoft.com/) anmelden und zum [Nachrichtencenter](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) wechseln. Hier finden Sie eine tägliche Zusammenfassung aller gesperrten Formulare. Für jedes aufgeführte Formular können Sie auswählen, ob die Sperre aufgehoben oder der Phishingversuch bestätigt werden soll. Erfahren Sie mehr über das [Überprüfen und Aufheben der Sperre von Formularen oder Benutzern, die wegen potenziellen Phishing-Angriffen erkannt und gesperrt wurden](review-unblock-forms-users-detected-blocked-potential-phishing.md).
