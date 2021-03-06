---
title: Gestire Power BI risposte
ms.author: dawholl
author: dawholl
manager: jeffkizn
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
ms.assetid: c0c814d0-f7e4-444e-b18e-09beb45c9322
description: Gestire la modalità Power BI i report e i dati nei risultati di ricerca
ms.openlocfilehash: 4b2251bdb8039c25fb1ec5290f3374a9f4eb3fd1
ms.sourcegitcommit: 4b72a31910753d46373a829a64ffec77fe6bc855
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547701"
---
# <a name="manage-power-bi-answers"></a>Gestire Power BI risposte

Per facilitare agli utenti l'individuazione dei dati e dell'analisi necessari per prendere decisioni informate, Microsoft Search ha aggiunto il supporto per i dashboard e i report Power BI utenti. Ecco alcuni dei vantaggi della Power BI ricerca:

* **Facile da usare:** Questa esperienza di ricerca avanzata consente agli utenti di trovare facilmente e rapidamente Power BI dashboard e report all'interno dell'organizzazione.
* **Contenuto più ricco:** Per rendere Power BI risultati di ricerca più utili, includono informazioni chiave come il tipo di contenuto, ovvero dashboard o report, e il team o la persona a cui è proprietario.
* **Protezione dei dati incorporata: Power BI** risultati verranno visualizzati solo per gli utenti che hanno accesso al dashboard o al report.
* **Esperienza di ricerca unificata:** Per mantenere un'esperienza coerente, Power BI risultati sono coerenti in tutti i punti di ingresso della ricerca. Ovunque si eserciti la ricerca, si otterrà gli stessi risultati con lo stesso aspetto.

## <a name="what-users-experience"></a>Esperienza degli utenti

Gli utenti di Microsoft Search possono trovare Power BI risultati eseguendo una ricerca dalla casella Windows ricerca, SharePoint, Office 365 e Bing. Gli utenti possono cercare report e dashboard con query come queste:

* Power BI informazioni`<topic>`
* Power BI per`<topic>`
* `<topic>`Power BI dashboard o Power BI dashboard`<topic>`
* `<topic>`Power BI report o Power BI report`<topic>`
* `<topic>`Power BI metriche o Power BI metriche`<topic>`
* `<topic>`Power BI scorecard o Power BI scorecard`<topic>`

Sostituire negli esempi precedenti con le informazioni che si stanno cercando, ad esempio `<topic>` vendite, utilizzo, capacità, 2021, Q1 e altro ancora, per visualizzare i risultati pertinenti da Power BI.

:::image type="content" source="media/powerbi-answers/powerbi-serp.png" alt-text="Screenshot di una pianificazione serp con Power BI e verticali" border="true":::

## <a name="turn-power-bi-search-on-or-off"></a>Attivare o Power BI ricerca

Power BI i risultati sono abilitati per l'organizzazione per impostazione predefinita. L Power BI admin può disabilitarli in qualsiasi momento. Nel portale Power BI di amministrazione passare a Impostazioni tenant e disabilitare l'impostazione Usa ricerca **globale per** Power BI. Per ulteriori informazioni, vedere [Administering Power BI nel portale di amministrazione.](/power-bi/admin/service-admin-portal#use-global-search-for-power-bi-preview)

:::image type="content" source="media/powerbi-answers/powerbi-admin.png" alt-text="Screenshot dell'impostazione per attivare o disattivare Power BI risposte" border="true":::

> [!NOTE]
> Quando si utilizza Microsoft Search, la query di ricerca e i risultati restituiti da Power BI possono essere elaborati in un'area geografica diversa da quella in cui si trovano i dati del tenant di Power BI.

## <a name="frequently-asked-questions"></a>Domande frequenti

**D: La Power BI ricerca è abilitata per impostazione predefinita?**

**A:** Sì. Power BI ricerca è abilitata per impostazione predefinita per Microsoft Search. L'amministratore tenant non richiede alcuna configurazione per la prima volta per questa funzionalità.

**D: È possibile Power BI ricerca per gruppi o utenti specifici?**

**A:** Attualmente, può essere abilitato o disabilitato solo per l'intera organizzazione.

**D: Se Power BI ricerca è disabilitata, la Power BI dei risultati della ricerca è nascosta?**

**A:** No. La Power BI dei risultati della ricerca verrà visualizzata con un messaggio che informa gli utenti che non è attualmente disponibile per l'organizzazione.

**D: Verrà visualizzata la pagina dei Power BI dei risultati della ricerca se non si dispone di una licenza Power BI licenza?**

**A:** No. Se un utente di ricerca non dispone di una licenza Power BI, la Power BI dei risultati della ricerca non verrà visualizzata nei risultati di Microsoft Search.

**D: Verranno visualizzati Power BI risultati di ricerca a cui non è possibile accedere?**

**A:** No. Microsoft Search restituirà solo Power BI risultati a cui si ha accesso.

**D: È possibile personalizzare i Power BI di ricerca (ad esempio, il tipo di report o il proprietario del report)?**

**A:** Attualmente non è possibile personalizzare i campi inclusi nei risultati Power BI ricerca.