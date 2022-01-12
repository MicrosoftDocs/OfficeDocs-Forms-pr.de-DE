---
title: Einrichten von Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: microsoft-365-education
ms.localizationpriority: high
description: Erfahren Sie, wie Microsoft 365 Administratoren steuern können, wie Microsoft Forms in ihrer Organisation verwendet wird. Außerdem erhalten Sie Antworten auf Fragen zur Sicherheit und Compliance, z.B. wo Daten für Microsoft Forms gespeichert sind.
ms.openlocfilehash: bb0e1a6ba8e2085550eb18a8bb393b34b197fe51
ms.sourcegitcommit: 80aa5565b4008855be844e8e5ab3f2779fba9a83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/05/2022
ms.locfileid: "61723723"
---
# <a name="set-up-microsoft-forms"></a>Einrichten von Microsoft Forms

## <a name="overview"></a>Übersicht

Mit Microsoft Forms können Ihre Benutzer schnell und einfach benutzerdefinierte Testfragen, Umfragen, Fragebögen, Registrierungen und vieles mehr erstellen. Wenn Sie ein Quiz oder ein Formular erstellen, können Sie andere dazu einladen, über einen Webbrowser darauf zu antworten, auch auf mobilen Geräten. Wenn Ergebnisse übermittelt werden, können Sie integrierte Analysen verwenden, um die Antworten auszuwerten. Formulardaten, z.B. Testergebnisse, können einfach zur weiteren Analyse oder Bewertung nach Excel exportiert werden.

Weitere Informationen finden Sie unter [Was ist Microsoft Forms?](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) Weitere Informationen finden auch Sie in unserem [Microsoft 365 Blogbeitrag](https://go.microsoft.com/fwlink/?linkid=852256) zu Microsoft Forms.

>[!Note]
>Microsoft Forms ist im Allgemeinen für Kunden mit Office 365 für Bildungseinrichtungen, Kunden mit Microsoft 365 Apps for Business und Kunden mit einem Microsoft-Konto (Hotmail, Live oder Outlook.com) verfügbar.

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="Vorschau, wie ein Formular auf einem mobilen Gerät aussieht.":::

## <a name="configure"></a>Konfigurieren

Microsoft 365 Administratoren können mithilfe der folgenden Aufgaben steuern, wie Microsoft Forms in ihrer Organisation verwendet wird:

|Administratoraufgabe   |Beschreibung   |
|----------|-----------|
|**Aktivieren oder Deaktivieren von Microsoft Forms**|Microsoft Forms ist standardmäßig für Ihre Organisation aktiviert. Sie können es jederzeit [deaktivieren](turn-off-turn-on-microsoft-forms.md).|
|**Deaktivieren von Microsoft Forms für einzelne Personen in Ihrer Organisation**|Wenn Sie Microsoft Forms für eine bestimmte Person deaktivieren, kann sie es nicht verwenden, und die *Formularkachel* wird nicht im Microsoft 365 App-Startfeld oder auf der Startseite angezeigt. Erfahren Sie, wie Sie [Formulare für bestimmte Personen deaktivieren](turn-off-turn-on-microsoft-forms.md).|
|**Einrichten des bedingten Zugriffs in Azure Active Directory für Microsoft Forms**|Wenn Sie eine Richtlinie für bedingten Zugriff für Microsoft Forms einrichten möchten, lesen Sie die [Dokumentation zum bedingten Zugriff in Azure AD](/azure/active-directory/conditional-access) und fügen Sie *Microsoft Form* den *Cloud-Apps-Zuweisungen* hinzu. <br/><br/> **Hinweis:** Wenn Benutzer in Ihrer Organisation auch nach dem Einrichten des bedingten Zugriffs für Microsoft Forms weiterhin blockiert werden, stellen Sie sicher, dass SharePoint Online und Exchange Online ebenfalls Zugriff über bedingtem Zugriff erhalten haben. [Weitere Informationen](/azure/active-directory/conditional-access/block-legacy-authentication).|
|**Steuern der Einstellungen für die externe Freigabe, Aufzeichnen von Namen von Personen in Ihrer Organisation und/oder Schützen von Formularen vor Phishing**|Im Microsoft 365 Admin Center haben Sie folgende Möglichkeiten: <ul><li>Sie können steuern, ob externe Benutzer mit Benutzern in Ihrer Organisation an einem Formular oder Test zusammenarbeiten dürfen.</li><li>Sie können auswählen, ob die Namen von Personen in Ihrer Organisation erfasst werden sollen, die Formulare ausfüllen.</li><li>Sie können die automatische Phishingerkennung auf Formularen deaktivieren oder aktivieren.</li></ul><br/>Erfahren Sie mehr über diese [Administratoreinstellungen](administrator-settings-microsoft-forms.md).|
|**Benutzern das Einfügen eines Formulars in PowerPoint ermöglichen**|<ol><li>Melden Sie sich bei https://admin.microsoft.com an.</li><li>Klicken Sie auf **Einstellungen** > **Einstellungen**.</li><li>Klicken Sie auf der Seite **Einstellungen** auf der Registerkarte **Dienste** auf die Option **Apps und Dienste im Besitz des Benutzers**.</li><li>Aktivieren Sie die Option **Benutzern den Zugriff auf den Office Speicher ermöglichen**, damit Benutzer ein Formular in PowerPoint einfügen können.</li></ol><br/>Beachten Sie, dass es einige Stunden dauern kann, bis die Änderung wirksam wird. [Weitere Informationen](/microsoft-365/admin/manage/manage-deployment-of-add-ins)|

## <a name="security--compliance"></a>Sicherheit und Compliance

Wenn Ihr Unternehmen in Hinsicht auf die Inhaltssicherheit und Datennutzung rechtliche, behördliche und technische Standards erfüllen muss, sollten Sie diesen Abschnitt unbedingt lesen.

**Wo werden Daten für Microsoft Forms gespeichert?**

Microsoft Forms-Daten werden auf Servern in den USA und Europa gespeichert. Alle Daten befindet sich in den USA, mit Ausnahme von Mandanten mit Sitz in Europa, die nach Mai 2017 mit der Verwendung von Microsoft Forms begonnen haben. Ihre Daten werden in Datenbanken in Europa gespeichert.

**Ist Microsoft Forms regelkonform?**

Microsoft Forms erfüllt die DSGVO-Complianceanforderungen vom May 2018. Weitere Informationen finden Sie unter [Microsoft 365 – Anträge betroffener Personen für die DSGVO](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json).

**Sind FERPA- und BAA-Schutzmaßnahmen vorhanden?**

Microsoft Forms erfüllt die [FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa)- und [BAA-Schutzstandards](https://www.microsoft.com/TrustCenter/Compliance/HIPAA).

**Ist die Anzahl der Benutzer und die Datenmenge, die für Benutzerkonten gespeichert werden, auch nach dem Verlassen meiner Organisation begrenzt?**

Derzeit gibt es keine Begrenzung für die Anzahl der Benutzer, für die Daten aufbewahrt werden, solange die Bereitstellung ihrer Konten im Rahmen der Onlinedienstvereinbarung Ihrer Organisation erfolgt. Auch die Menge der gespeicherten Daten für Benutzerkonten ist nicht begrenzt.

**Der ursprüngliche Eigentümer eines Formulars gehört nicht mehr zu meiner Organisation und/oder seine Microsoft Forms-Lizenz wurde entfernt. Was passiert also mit den Daten, die mit dem von ihm erstellten Formular verknüpft sind?**

Alle kontobezogenen Daten werden 30 Tage nach der Löschung eines Benutzerkontos von Ihrem Mandanten (Azure AD) gelöscht.

## <a name="faq"></a>Häufig gestellte Fragen

**Wofür kann ich Microsoft Forms verwenden?**

Microsoft Forms ist eine einfache, kleine App, mit der Sie auf einfache Weise Umfragen, Tests und Fragebögen erstellen können. In Bildungseinrichtungen kann sie zum Erstellen von Prüfungsfragen, zum Einholen des Feedbacks von Lehrern und Eltern oder zum Planen von Kurs- und Mitarbeiteraktivitäten verwendet werden. In Unternehmen wird sie zum Einholen von Kundenfeedback, zum Messen der Mitarbeiterzufriedenheit, zum Verbessern von Produkten oder Geschäftsvorgängen bzw. zum Organisieren von Unternehmensereignissen eingesetzt.

**Wer kann Microsoft Forms verwenden?**

Microsoft Forms kann kostenlos für alle Benutzer mit einem Microsoft-Konto (Hotmail, Live oder Outlook.com) verwendet werden. Die folgenden Kunden mit Office 365 für Bildungseinrichtungen und Microsoft 365 Apps for Business können auch Microsoft Forms verwenden:

**Office 365 Education**

  - Office 365 A1 Plus

  - Office 365 A5

  - Bestehende Kunden, die Office 365 für Bildungseinrichtungen E3 vor der Einstellung erworben haben

**Microsoft 365 Apps for Business**

  - Microsoft 365 Business Basic

  - Microsoft 365 Business Standard

  - Microsoft 365 Business Premium

  - Microsoft 365 Apps for Enterprise

  - Microsoft 365 Enterprise E1, E3 und E5 Pläne

  - Vorhandene Office 365 Enterprise E4 Kunden, die E4 vor der Einstellung erworben haben

Melden Sie sich auf der Website [forms.office.com](https://forms.office.com/) an und beginnen Sie mit der Erstellung von Umfragen, Tests und Abstimmungen.

**Können Personen ohne Microsoft 365 Konto weiterhin eine Umfrage oder einen Test in Microsoft Forms übermitteln?**

Microsoft Forms-Autoren können die Einstellungen so festlegen, dass Benutzer außerhalb ihrer Organisation auf ihre Umfrage oder ihren Test antworten können. In diesem Fall übermitteln die Benutzer ihre Antworten anonym. Wenn Sie sehen möchten, wer Ihre Umfrage oder Prüfung ausgefüllt hat, können Sie im Rahmen der Befragung die Befragten auffordern, ihre Namen im Fragebogen einzugeben.

**Wie hoch ist die Anzahl der Formulare, die erstellt werden können, und wie hoch ist die Anzahl der Antworten, die ein Formular erhalten kann?**

Kunden mit Office 365 für Bildungseinrichtungen und Microsoft 365 Apps for Business können bis zu 200 Formulare erstellen, und jedes Formular kann bis zu 50.000 Antworten erhalten. Microsoft Forms-Benutzer mit einem Microsoft-Konto (Hotmail, Live oder Outlook.com) können bis zu 200 Formulare erstellen, wobei jedes Formular bei kostenpflichtigen Konten bis zu 1.000 Antworten und bei kostenlosen Konten bis zu 200 Antworten erhalten kann. Erfahren Sie mehr über [die Beschränkungen für Formulare, Fragen, Antworten und Zeichen in Formularen](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea).

Wenn Sie mehr Antworten benötigen, empfehlen wir, vorhandene Antworten in eine Excel-Arbeitsmappe zu exportieren und diese dann aus der Umfrage oder Prüfung zu entfernen. Nach dem Entfernen können Sie dann weitere Antworten sammeln.

**Mit welchen Webbrowsern funktioniert Microsoft Forms?**

Microsoft Forms ist für Internet Explorer 11, Edge, Chrome (neueste Version), Firefox (neueste Version), Chrome unter Android (neueste Version) und Safari unter iOS (neueste Version) optimiert.

**In welchen Sprachen ist Microsoft Forms verfügbar?**

Informationen dazu finden Sie unter [Unterstützte Sprachen](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac) und [Spracheinstellungen](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27) für Microsoft Forms.

**Ersetzt Microsoft Forms Microsoft InfoPath?**

Nein. Microsoft InfoPath war eine Lösung zum Erstellen anpassbarer Formulare, die automatisierte Workflows ermöglichen, wohingegen Microsoft Forms eine einfache, kleine App zum schnellen Sammeln von Informationen mittels Umfragen und Prüfungsfragen ist.

Microsoft InfoPath wird durch SharePoint-Listen, Microsoft Flow und PowerApps ersetzt – moderne Lösungen für die Digitalisierung herkömmlicher Unternehmensformulare, für die Automatisierung von Workflows und für die Umwandlung von Geschäftsprozessen. [Weitere Informationen](https://products.office.com/business/business-process-automation).

**Wo kann ich Feedback (z.B. Produktfehler oder Featurewünsche) übermitteln?**

Wir freuen uns auf Ihre Kommentare! Um Feedback zu Microsoft Forms zu senden, gehen Sie in die obere rechte Ecke Ihres Formulars und wählen Sie **Weitere Formulareinstellungen** ![Schaltfläche „Weitere Optionen“](./media/image2.png) >  **Feedback** aus.

> [!Note]
> Weitere Informationen finden Sie auch unter [Häufig gestellte Fragen zu Microsoft Forms (Preview)](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c).

