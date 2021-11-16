---
title: Überprüfen und Entsperren von Formularen oder Benutzern, die wegen potenziellen Phishings erkannt und blockiert wurden
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms ermöglicht automatische maschinelle Überprüfungen zur proaktiven Erkennung von böswilliger Sammlung vertraulicher Daten in Formularen und Umfragen. Wenn Sie ein globaler und/oder Sicherheitsadministrator sind, können Sie sich beim Microsoft 365 Admin Center anmelden, um Formulare zu überprüfen und freizugeben, die als potenzielle Phishing- oder böswillige Absichten erkannt und deshalb gesperrt wurden.
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951499"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>Überprüfen und Entsperren von Formularen oder Benutzern, die wegen potenziellen Phishings erkannt und blockiert wurden

Microsoft Forms ermöglicht automatische maschinelle Überprüfungen, um die böswillige Sammlung vertraulicher Daten in Formularen proaktiv zu erkennen und diese Formulare vorübergehend für die Sammlung von Antworten zu sperren. Erfahren Sie mehr über [Microsoft Forms und proaktives Verhindern von Phishing](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

>[!Note]
>Die Schritte in diesem Dokument gelten auch für [Dynamics 365 Customer Voice](https://go.microsoft.com/fwlink/p?linkid=2128500) (früher als Forms Pro bezeichnet). Beachten Sie, dass eine Dynamics 365 Customer Voice-Lizenz erforderlich ist, um die Blockierung von Dynamics 365 Customer Voice-Umfragen aufzuheben. [Weitere Informationen](/dynamics365/customer-voice/help-hub).

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>Überprüfen von Warnungen im Microsoft 365 Defender-Portal

Wenn Sie ein globaler oder Sicherheitsadministrator sind, erhalten Sie im [Microsoft 365 Defender](https://security.microsoft.com/) Portal Benachrichtigungen zu potenziellen Phishingformularen, für die Sie Maßnahmen ergreifen können.

>[!Note]
> Wenn Sie ein globaler Administrator sind, erhalten Sie Datenschutznachrichten für Ihr Unternehmen, einschließlich täglicher Benachrichtigungen über alle Formulare, die in Ihrem Mandanten erstellt wurden und wegen möglicher Phishing-Attacken erfasst und gesperrt wurden. Sie können diese Benachrichtigungen im [Nachrichtencenter](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) sehen, indem Sie nach **Microsoft Forms Phishing Notification** suchen. (Wenn diese Benachrichtigung auf der Registerkarte bzw. in der Ansicht **Alle aktiven Nachrichten** nicht angezeigt wird, finden Sie sie möglicherweise auf der Registerkarte bzw. in der Ansicht **Verworfene Nachrichten**). Wählen Sie für jede Benachrichtigung den Link **URL der Formularadministratorüberprüfung** oder Links zum Überprüfen gesperrter Formulare aus.  
  
Damit Sicherheitsadministratoren auch Benachrichtigungen zu potenziellen Phishingformularen erhalten, müssen globale Administratoren ihnen die Rolle [Nachrichtencenter-Datenschutzleser](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) zuweisen. Weitere Informationen zum Nachrichtencenter finden Sie unter [Häufig gestellte Fragen](/microsoft-365/admin/manage/message-center). Erfahren Sie auch, wie Sie [E-Mail-Einstellungen für Datenschutznachrichten festlegen](/microsoft-365/admin/manage/message-center#preferences).

1.  Melden Sie sich beim [Microsoft 365 Defender-Portal](https://security.microsoft.com/) an.

2.  Wählen Sie **Vorfälle und Warnungen** \> **Warnungen** aus. Möglicherweise werden eine oder alle der folgenden Warnungen für Forms angezeigt:
    
      - **Benutzer, der keine Formulare teilen und keine Antworten sammeln darf**
    
      - **Formular, das als Phishing gekennzeichnet und bestätigt ist**
    
      - **Formular, das wegen eines potenziellen Phishingversuchs blockiert wurde**

3.  Wählen Sie eine Warnung aus, um sie zu überprüfen. Um das gekennzeichnete Formular zu überprüfen, tippen oder klicken Sie auf die drei Punkte in der unteren rechten Ecke neben der Schaltfläche **Warnung verwalten** und wählen Sie dann **Dieses Formular überprüfen**aus.
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="Option „Dieses Formular überprüfen“":::

    >[!Tip]
    >Weitere Informationen zu [Warnungsrichtlinien in Microsoft 365](/microsoft-365/compliance/alert-policies).

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>Aufheben der Sperre eines Formulars oder Bestätigen des Phishingversuchs

Für jedes Formular, das Sie überprüfen, können Sie auswählen, ob es entsperrt oder der Phishingversuch bestätigt werden soll.

### <a name="unblock"></a>Entsperren

Wählen Sie **Entsperren** aus, wenn Sie nicht glauben, dass ein Formular eine böswillige Absicht hat.

>[!Note]
>Wenn sie von einer Person in Ihrem Mandanten aufgefordert werden, die Sperre ihres Formulars aufzuheben, empfehlen wir Ihnen, bestimmte Formularinformationen (z.B. Datum und Uhrzeit der Sperre, Titel) anzufordern, um die Benachrichtigung im Admin Center effizienter zu identifizieren. Da Benachrichtigungen täglich gesendet werden und alle erkannten Formulare in den letzten 24 Stunden beinhalten, sind identifizierbare Informationen für das Formular hilfreich.

### <a name="confirm-phishing"></a>Bestätigen des Phishingversuchs

Wählen Sie **Phishing bestätigen** aus, wenn Sie der Meinung sind, dass ein Formular eine böswillige Absicht hat. Das Formular wird dauerhaft gesperrt, und der Besitzer kann es nicht mehr bearbeiten oder löschen.

Nachdem Sie **Phishing bestätigen**ausgewählt haben, klicken oder tippen Sie auf **Formular löschen**, um das Formular dauerhaft aus Ihrem Mandanten zu löschen. Wir empfehlen dringend eine sofortige Kennwortzurücksetzung für ein Konto in Ihrem Mandanten, von dem Sie glauben, dass es kompromittiert wurde.

>[!Tip]
>Ihre Auswahl von **Phishing bestätigen** hilft Microsoft Forms bei der Verbesserung der Erkennungsgenauigkeit. 

## <a name="commonly-asked-questions"></a>Häufig gestellte Fragen

**Warum werden beim Überprüfen eines gesperrten Formulars keine Optionen zum Entsperren oder zum Bestätigen des Phishingversuchs angezeigt?**

Bei der Überprüfung wird möglicherweise ein Sperre für ein Formular angezeigt, das bereits entsperrt wurde. Dies bedeutet, dass der Formularbesitzer zwischen dem Zeitpunkt, zu dem ein Formular gesperrt wurde, und dem Zeitpunkt, zu dem Sie es überprüft haben, Schlüsselwörter entfernt hat, die für potenzielle Phishing-Angriffe gekennzeichnet wurden. In diesem Szenario ist keine weitere Aktion von Ihnen erforderlich.

**Kann ich ein Formular entfernen, wenn es wegen eines bestätigten Phishingversuchs gesperrt wurde?**

Wenn das Formular bereits wegen eines bestätigten Phishing-Angriffe gesperrt wurde, wählen Sie **Formular löschen** aus, um es aus Ihrem Mandanten zu entfernen.

**Was geschieht, wenn ich keine Aktion für ein gesperrtes Formular ausführe?**

Wenn Sie keine Maßnahmen ergreifen (entweder das Formular entsperren oder seine Phishing-Absicht bestätigen), bleibt das Formular gesperrt. Der Formularbesitzer kann das Formular weiterhin bearbeiten und Schlüsselwörter entfernen, die als potenzielles Phishing gekennzeichnet wurden.

**Was geschieht, wenn ich den gesperrten Inhalt im Formular bearbeiten oder löschen möchte?**

Wenn Sie es vorziehen, gesperrte Inhalte zu bearbeiten und/oder zu löschen, können Sie eine Seite für die gemeinsame Dokumenterstellung erstellen und das Formular als Mitautor verwalten. Klicken Sie dazu auf den Link **Seite für gemeinsame Dokumenterstellung öffnen** in der Nachricht über dem Formular, das Sie überprüfen.

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>Entfernen von Einschränkungen für gesperrte Microsoft Forms-Benutzer

Microsoft Forms verhindert, dass Benutzer, die wiederholt versucht haben, persönliche oder vertrauliche Informationen zu sammeln, Formulare verteilen und Antworten sammeln. Globale Administratoren werden über das [Nachrichtencenter](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) über diese gesperrten Benutzer benachrichtigt. Wenn Sie der Meinung sind, dass ein gesperrter Benutzer keine böswillige Absichten hat und sein Konto sicher ist, können Sie die folgenden Schritte zum Entsperren ausführen.

>[!Note]
>Sicherheitsadministratoren können auch Benachrichtigungen zu potenziellen Phishingformularen erhalten, sobald ein globaler Administrator ihnen die Rolle [Nachrichtencenter-Datenschutzleser](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) zuweist.

1.  Wechseln Sie zum [Nachrichtencenter](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) und suchen Sie nach der Benachrichtigung **Verhindern/Beheben: Microsoft Forms erkannte potenzielles Phishing**.

    >[!Note]
    >Wenn diese Benachrichtigung auf der Registerkarte bzw. in der Ansicht **Alle aktiven Nachrichten** nicht angezeigt wird, finden Sie sie möglicherweise auf der Registerkarte bzw. in der Ansicht **Verworfene Nachrichten**.
 
    Diese Benachrichtigung enthält eine Liste der Benutzer in Ihrem Mandanten, die am Freigeben von Formularen und Sammeln von Antworten gehindert werden.

2.  Klicken Sie auf den in der Benachrichtigung angegebenen Link, um gesperrte Benutzer zu überprüfen.

3.  Für jeden Benutzer, von dem Sie glauben, dass er keine böswillige Absicht hat, können Sie auf den Link **Entsperren** in der Spalte **Aktionen** klicken, der diesem Benutzer zugeordnet ist.

    >[!Note]
    >Wenn Sie der Meinung sind, dass ein Benutzer böswillige Absichten hat, ist keine weitere Aktion von Ihnen erforderlich.

    >[!Note]
    >Es kann bis zu 30 Minuten oder länger dauern, bis Einschränkungen aufgehoben werden.

