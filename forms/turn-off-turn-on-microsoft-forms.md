---
title: Aktivieren oder Deaktivieren von Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: In diesem Artikel wird beschrieben, wie Microsoft 365 Administratoren Microsoft Forms für ihre gesamte Organisation oder bestimmte Personen in ihrer Organisation deaktivieren oder aktivieren können.
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951460"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>Aktivieren oder Deaktivieren von Microsoft Forms

Standardmäßig ist [Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) für alle Benutzer in Ihrer Organisation aktiviert. Wenn Sie ein [Administrator](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504) sind, können Sie [Microsoft Forms einrichten](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240), dann deaktivieren oder erneut für Ihre gesamte Organisation oder nur für bestimmte Personen aktivieren.

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>Deaktivieren von Microsoft Forms für alle Personen in Ihrer Organisation

1.  Melden Sie sich bei [Microsoft Azure](https://portal.azure.com/) an.

2.  Klicken Sie im linken Bereich auf **Azure Active Directory**.

3.  Klicken Sie auf **Unternehmensanwendungen**.

4.  Navigieren Sie zu den erforderlichen Diensten, und wiederholen Sie dann die Schritte 5 bis 7 für den **Anwendungstyp** \> **CollabDBService** und für **Microsoft Applications** \> **Microsoft Forms**.
    
      - Geben Sie im Suchfeld unter der Dropdownliste **Anwendungstyp** **CollabDBService** ein. Wählen Sie **CollabDBService** in der Liste der Suchergebnisse aus.
    
      - Wählen Sie in der Dropdownliste **Anwendungstyp** die Option **Microsoft-Anwendungen** aus. Geben Sie im Suchfeld unter der Dropdownliste **Anwendungstyp** **Microsoft Forms** ein und wählen Sie dann **Microsoft Forms** in der Liste der Suchergebnisse aus.

5.  Klicken Sie unter **Verwalten** auf **Eigenschaften**.

6.  Wählen Sie für die Option **Für Benutzeranmeldung aktiviert?** die Option **Nein** aus.

7.  Klicken Sie auf **Speichern**.

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>Deaktivieren von Microsoft Forms für bestimmte Personen in Ihrer Organisation

1.  Melden Sie sich bei Microsoft 365 mit Ihrem Firmen- oder Schulkonto als globaler Administrator an. [Hier erfahren Sie, wie Sie sich anmelden.](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4)

2.  Wählen Sie im Microsoft 365 Admin Center **Benutzer** \> **Aktive Benutzer** aus.

3.  Aktivieren Sie das Kontrollkästchen neben dem Namen der Person, für die Sie Microsoft Forms deaktivieren möchten.

4.  Klicken Sie auf dem Menüband auf **Produktlizenzen verwalten**.

5.  Erweitern Sie auf dem daraufhin geöffneten Kontoformular auf der Registerkarte **Lizenzen und Apps** den Abschnitt „Apps“ und scrollen Sie nach unten zur Microsoft Forms-Option. 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Formular „Kontooptionen“ in Microsoft 365 Admin Center":::

6.  Deaktivieren Sie das Kontrollkästchen, um Microsoft Forms zu deaktivieren. Aktivieren Sie das Kontrollkästchen, um es zu aktivieren.

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text=" Microsoft Forms-Umschaltfläche":::

     > [!Note]
     > [Überprüfen Sie diese Liste](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e), um festzustellen, ob Sie über eine Office Lizenz verfügen, die Microsoft Forms enthält. Wenn Ihre Lizenz aufgeführt ist, müssen Sie das Microsoft Forms-Kontrollkästchen deaktivieren, um den Benutzerzugriff vollständig zu deaktivieren.

7.  Klicken Sie unten in der Liste **Apps** auf **Änderungen speichern**.

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>Ich habe Microsoft Forms aktiviert, aber Personen in meiner Organisation können weiterhin nicht darauf zugreifen

Überprüfen Sie die folgende Einstellung in Microsoft Azure, um sicherzustellen, dass Microsoft Forms aktiviert ist:

1.  Melden Sie sich bei [Microsoft Azure](https://portal.azure.com/) an.

2.  Klicken Sie im linken Bereich auf **Azure Active Directory**.

3.  Klicken Sie auf **Unternehmensanwendungen**.

4.  Navigieren Sie zu den erforderlichen Diensten, und wiederholen Sie dann die Schritte 5 bis 7 für den **Anwendungstyp** \> **CollabDBService** und für **Microsoft Applications** \> **Microsoft Forms**.
    
      - Geben Sie **CollabDBService** in das Suchfeld unter der Dropdownliste **Anwendungstyp** ein. Wählen Sie **CollabDBService** in der Liste der Suchergebnisse aus.
    
      - Wählen Sie in der Dropdownliste **Anwendungstyp** die Option **Microsoft-Anwendungen** aus. Geben Sie im Suchfeld unter der Dropdownliste **Anwendungstyp** **Microsoft Forms** ein und wählen Sie dann **Microsoft Forms** in der Liste der Suchergebnisse aus.

5.  Klicken Sie unter **Verwalten** auf **Eigenschaften**.

6.  Wählen Sie für die Option **Für Benutzeranmeldung aktiviert?** die Option **Ja** aus.

7.  Klicken Sie auf **Speichern**.

    >[!Note]
    >SharePoint Dienste müssen auch aktiviert sein, damit Personen in Ihrer Organisation auf Microsoft Forms zugreifen können.

## <a name="feedback-for-microsoft-forms"></a>Feedback für Microsoft Forms

Wir freuen uns über Ihr Feedback\! Um Feedback zu Microsoft Forms zu senden, gehen Sie in die obere rechte Ecke Ihres Formulars und wählen Sie **Weitere Formulareinstellungen** ![Schaltfläche „Weitere Optionen“](./media/image2.png)\> **Feedback**.

