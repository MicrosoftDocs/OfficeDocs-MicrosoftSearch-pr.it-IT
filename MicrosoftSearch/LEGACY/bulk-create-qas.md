---
title: Creare in blocco domande e risposte
ms.author: dawholl
author: dawholl
manager: kellis
ms.date: 12/18/2018
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
ms.assetid: 7bada218-8908-4956-aae3-6ffaeef384ca
ROBOTS: NoIndex
description: Rispondere rapidamente alle domande frequenti con gli strumenti di importazione nel portale di amministrazione di Microsoft Search
ms.openlocfilehash: 660f5663ff6238f4ab59dab36d51f1311d5c7260
ms.sourcegitcommit: 6b531b2ce7253c16251c7089795dedf1d2f3fc33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/13/2019
ms.locfileid: "38311683"
---
# <a name="bulk-create-qas"></a><span data-ttu-id="73bc6-103">Creare in blocco domande e risposte</span><span class="sxs-lookup"><span data-stu-id="73bc6-103">Bulk create Q&As</span></span>

> [!IMPORTANT]
> <span data-ttu-id="73bc6-104">Questo articolo si applica al portale di amministrazione di Microsoft Search in Bing.</span><span class="sxs-lookup"><span data-stu-id="73bc6-104">This article applies to the Microsoft Search in Bing admin portal.</span></span> <span data-ttu-id="73bc6-105">Il portale di amministrazione di Microsoft Search in Bing sta per essere trasferito nell'interfaccia di amministrazione di Microsoft 365 e successivamente verrà rimosso.</span><span class="sxs-lookup"><span data-stu-id="73bc6-105">We’re moving the portal to the Microsoft 365 admin center, and then the Microsoft Search in Bing portal will be removed.</span></span> <span data-ttu-id="73bc6-106">Per iniziare, è consigliabile usare l'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="73bc6-106">We recommend that you use the Microsoft 365 admin center to get started.</span></span> <span data-ttu-id="73bc6-107">[Panoramica di Microsoft Search](overview-microsoft-search.md).</span><span class="sxs-lookup"><span data-stu-id="73bc6-107">[Overview of Microsoft Search](overview-microsoft-search.md).</span></span>
    
<span data-ttu-id="73bc6-108">Scaricare e usare il modello CSV per creare o modificare in blocco domande e risposte.</span><span class="sxs-lookup"><span data-stu-id="73bc6-108">Download and use the .csv template to bulk create or bulk edit Q&As.</span></span> <span data-ttu-id="73bc6-109">È anche un modo semplice per salvare in blocco bozze di domande e risposte che richiedono ulteriori modifiche o aggiornamenti.</span><span class="sxs-lookup"><span data-stu-id="73bc6-109">It's also a simple way to bulk save draft Q&As that need additional edits or updates.</span></span> <span data-ttu-id="73bc6-110">Se è necessario modificare in blocco domande e risposte esistenti, esportarle dal portale di amministrazione, apportare le modifiche necessarie e quindi importarle.</span><span class="sxs-lookup"><span data-stu-id="73bc6-110">If you need to bulk edit existing Q&As, export them from the Admin portal, make the necessary edits, and then import them.</span></span>
  
1. <span data-ttu-id="73bc6-111">Nell'angolo superiore destro della sezione Domande e risposte, fare clic su **Importa**.</span><span class="sxs-lookup"><span data-stu-id="73bc6-111">In the upper-right corner of the Q&As section, click **Import**</span></span>
    
2. <span data-ttu-id="73bc6-112">Fare clic su **Scarica modello domande e risposte (CSV)**.</span><span class="sxs-lookup"><span data-stu-id="73bc6-112">Click **Download Q&A template (.csv)**</span></span>
    
3. <span data-ttu-id="73bc6-113">Salvare e aprire il file CSV</span><span class="sxs-lookup"><span data-stu-id="73bc6-113">Save and open the .csv file</span></span>
    
4. <span data-ttu-id="73bc6-114">Aggiungere contenuto e impostazioni delle domande e risposte e salvare il file.</span><span class="sxs-lookup"><span data-stu-id="73bc6-114">Add the Q&A content and settings and save the file</span></span>

    <span data-ttu-id="73bc6-115">Il file CSV deve essere salvato come file UTF-8 CSV, altre codifiche e/o tipi di file potrebbero causare errori di importazione</span><span class="sxs-lookup"><span data-stu-id="73bc6-115">The .csv file should be saved as a CSV UTF-8 file, other file types and or encodings may cause import errors</span></span>
    
5. <span data-ttu-id="73bc6-116">Nell'angolo superiore destro della sezione Domande e risposte, fare clic su **Importa**.</span><span class="sxs-lookup"><span data-stu-id="73bc6-116">In the upper-right corner of the Q&As section, click **Import**</span></span>
    
6. <span data-ttu-id="73bc6-117">Nel riquadro Importa domande e risposte fare clic su \*\*Sfoglia \*\*e passare al file CSV da importare.</span><span class="sxs-lookup"><span data-stu-id="73bc6-117">In the Import Q&As pane, click **Browse** and navigate to the .csv file you want to import</span></span> 
    
7. <span data-ttu-id="73bc6-118">Fare clic su **Importa**.</span><span class="sxs-lookup"><span data-stu-id="73bc6-118">Click **Import**</span></span>

## <a name="prevent-import-errors"></a><span data-ttu-id="73bc6-119">Evitare gli errori di importazione</span><span class="sxs-lookup"><span data-stu-id="73bc6-119">Prevent import errors</span></span>      
<span data-ttu-id="73bc6-120">Se i dati necessari sono mancanti o non validi, si riceverà un messaggio di errore.</span><span class="sxs-lookup"><span data-stu-id="73bc6-120">You'll get an error if any required data is missing or invalid.</span></span> <span data-ttu-id="73bc6-121">A seconda dell'errore, può essere generato un file di log con altre informazioni sulle righe e sulle colonne da correggere.</span><span class="sxs-lookup"><span data-stu-id="73bc6-121">Depending on the error, a log file may be generated with more information about the rows and columns that need to be corrected.</span></span> <span data-ttu-id="73bc6-122">Apportare le modifiche necessarie e ritentare l'importazione del file.</span><span class="sxs-lookup"><span data-stu-id="73bc6-122">Make any necessary edits, and try importing the file again.</span></span>

> [!NOTE]
> <span data-ttu-id="73bc6-123">Fino a quando non sono stati risolti tutti gli errori, non è possibile creare o modificare le domande e risposte.</span><span class="sxs-lookup"><span data-stu-id="73bc6-123">Until all errors are resolved, you can't create or edit any Q&As.</span></span> 

<span data-ttu-id="73bc6-124">Per evitare errori, verificare che il file di importazione sia formattato correttamente, ossia che:</span><span class="sxs-lookup"><span data-stu-id="73bc6-124">To help prevent errors, make sure your import file is properly formatted:</span></span>
- <span data-ttu-id="73bc6-125">Includa la riga di intestazione presente nel modello di importazione</span><span class="sxs-lookup"><span data-stu-id="73bc6-125">Includes the header row that was in the import template</span></span>
- <span data-ttu-id="73bc6-126">Includa tutte le colonne presenti nel modello di importazione</span><span class="sxs-lookup"><span data-stu-id="73bc6-126">Includes all columns that were in the import template</span></span>
- <span data-ttu-id="73bc6-127">L'ordine delle colonne equivalga a quello del modello di importazione</span><span class="sxs-lookup"><span data-stu-id="73bc6-127">The column order is the same as the import template</span></span>
- <span data-ttu-id="73bc6-128">Queste colonne possono essere vuote: ID, Ultima modifica e Autore ultima modifica</span><span class="sxs-lookup"><span data-stu-id="73bc6-128">These columns can be empty: Id, Last Modified, and Last Modified By</span></span>
- <span data-ttu-id="73bc6-129">La colonna Stato non può essere vuota, perché si tratta di informazioni obbligatorie</span><span class="sxs-lookup"><span data-stu-id="73bc6-129">The State column can't be empty, this information is required</span></span>  
<span data-ttu-id="73bc6-130">In base al campo Stato, le domande e risposte saranno salvate come bozza, suggerite o pianificate, oppure saranno pubblicate automaticamente.</span><span class="sxs-lookup"><span data-stu-id="73bc6-130">Based on the State field, Q&As will be saved as draft, suggested, scheduled, or they will be published automatically.</span></span>

<span data-ttu-id="73bc6-131">Se si include l'Id di una domanda e risposta esistente, verrà sostituito con le informazioni presenti nel file di importazione.</span><span class="sxs-lookup"><span data-stu-id="73bc6-131">Also, if you include the Id of an existing Q&A, it will be replaced with the information in the import file.</span></span>

<span data-ttu-id="73bc6-132">Per i partner che gestiscono più organizzazioni, è possibile esportare le&Q come da una org e importarle in un'altra.</span><span class="sxs-lookup"><span data-stu-id="73bc6-132">For partners who manage multiple organizations, you can export your Q&As from one org and import them into another.</span></span> <span data-ttu-id="73bc6-133">È tuttavia necessario rimuovere i dati dalla colonna Id prima dell'importazione.</span><span class="sxs-lookup"><span data-stu-id="73bc6-133">But you must remove all of the data in the Id column before you import.</span></span>

<span data-ttu-id="73bc6-134">Per altre informazioni sui campi obbligatori e consigliati, vedere [Creare domande e risposte](create-qas.md).</span><span class="sxs-lookup"><span data-stu-id="73bc6-134">To find out more about required and recommended fields, see [Create Q&As](create-qas.md).</span></span>

  
