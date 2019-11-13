---
title: Gestire i piani di piano
ms.author: rasrivas
author: rasrivas
manager: tonytha
ms.date: 11/01/2019
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
description: La caratteristica planimetria di Microsoft Search aiuta gli utenti a trovare persone, uffici e altre amenità all'interno di un edificio.
ms.openlocfilehash: 68912a8f440443c14cbc27019c7b30dc2d7a34c6
ms.sourcegitcommit: bfcab9d42e93addccd1e3875b41bc9cc1b6986cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949866"
---
# <a name="manage-floor-plans"></a><span data-ttu-id="0481c-103">Gestire i piani di piano</span><span class="sxs-lookup"><span data-stu-id="0481c-103">Manage floor plans</span></span>

<span data-ttu-id="0481c-104">Le planimetrie di Microsoft Search aiutano gli utenti a trovare persone e sale riunioni all'interno di un edificio.</span><span class="sxs-lookup"><span data-stu-id="0481c-104">Microsoft Search floor plans help users find people and meeting rooms within a building.</span></span> <span data-ttu-id="0481c-105">Planimetrie rispondere a queste domande:</span><span class="sxs-lookup"><span data-stu-id="0481c-105">Floor plans answer these questions:</span></span>
- <span data-ttu-id="0481c-106">Dove si trova Allan DeYoung ' s Office?</span><span class="sxs-lookup"><span data-stu-id="0481c-106">Where is Allan Deyoung's office?</span></span>
- <span data-ttu-id="0481c-107">Dove si trova la sala riunioni C1?</span><span class="sxs-lookup"><span data-stu-id="0481c-107">Where is meeting room C1?</span></span>

![Planimetria che individua la posizione dell'ufficio dell'utente all'interno dell'edificio.](media/floorplans-officelocation.png)

<span data-ttu-id="0481c-109">Per semplificare la ricerca di risposte a domande di questo tipo, è necessario che informazioni sugli edifici, gli uffici e le strutture di un'organizzazione debbano essere disponibili e reperibili.</span><span class="sxs-lookup"><span data-stu-id="0481c-109">To make it easy to find answers to questions like these, information about an organization's buildings, offices, and facilities needs to be available and made searchable.</span></span> <span data-ttu-id="0481c-110">Le organizzazioni di grandi dimensioni hanno in genere strutture o team di gestione dello spazio e potrebbero essere già disponibili per queste informazioni.</span><span class="sxs-lookup"><span data-stu-id="0481c-110">Larger organizations usually have facilities or space management teams and might already have this info available.</span></span> <span data-ttu-id="0481c-111">In un'organizzazione di dimensioni ridotte, potrebbe essere necessario creare e aggiungere l'amministratore della ricerca.</span><span class="sxs-lookup"><span data-stu-id="0481c-111">In a smaller organization, the Search admin might have to create and add it.</span></span>

## <a name="48-hours-before-you-begin"></a><span data-ttu-id="0481c-112">48 ore prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="0481c-112">48 hours before you begin</span></span>
<span data-ttu-id="0481c-113">Prima di iniziare a caricare planimetrie, è necessario indicizzare le posizioni di Office degli utenti.</span><span class="sxs-lookup"><span data-stu-id="0481c-113">Before you start to upload floor plans, you need to index the users' office locations.</span></span> <span data-ttu-id="0481c-114">A seconda delle dimensioni dell'organizzazione, è possibile richiedere fino a 48 ore per il completamento.</span><span class="sxs-lookup"><span data-stu-id="0481c-114">Depending on the size of your organization, it can take up to 48 hours to complete.</span></span> <span data-ttu-id="0481c-115">Se si ignora questo passaggio, viene visualizzato un errore durante l'esecuzione della procedura.</span><span class="sxs-lookup"><span data-stu-id="0481c-115">If you ignore this step, you get errors while performing the procedure.</span></span>

![Schermata di acquisizione della pagina planimetrie con "Microsoft ha bisogno di raccogliere e organizzare le posizioni di Office prima di poter caricare i piani di piano".](media/floorplans_hydrationstep.png)

<span data-ttu-id="0481c-117">Nell'interfaccia di [Amministrazione](https://admin.microsoft.com)di Microsoft 365, passare a **Impostazioni** > **piani**di**ricerca di Microsoft Search** > , quindi selezionare **inizia**.</span><span class="sxs-lookup"><span data-stu-id="0481c-117">In the Microsoft 365 [admin center](https://admin.microsoft.com), go to **Settings** > **Microsoft Search** > **Floor plans**, and then select **Get started**.</span></span>

<span data-ttu-id="0481c-118">Se non viene visualizzato questo avviso, l'utente o un utente dell'organizzazione ha già avviato questo passaggio.</span><span class="sxs-lookup"><span data-stu-id="0481c-118">If you don't see this notice, then you or someone in your organization has already initiated this step.</span></span>

## <a name="things-to-consider"></a><span data-ttu-id="0481c-119">Osservazioni</span><span class="sxs-lookup"><span data-stu-id="0481c-119">Things to consider</span></span>
<span data-ttu-id="0481c-120">Per consentire agli utenti di trovare informazioni su uffici e strutture di creazione, è necessario aggiungere:</span><span class="sxs-lookup"><span data-stu-id="0481c-120">To help users to find information about offices and building facilities, you need to add:</span></span>

|<span data-ttu-id="0481c-121">Considerazione</span><span class="sxs-lookup"><span data-stu-id="0481c-121">Consideration</span></span>     |<span data-ttu-id="0481c-122">Ma perché è così importante?</span><span class="sxs-lookup"><span data-stu-id="0481c-122">Why is this important?</span></span>  |
|---------|---------|
|<span data-ttu-id="0481c-123">Posizione dell'edificio</span><span class="sxs-lookup"><span data-stu-id="0481c-123">Building location</span></span>    |    <span data-ttu-id="0481c-124">È necessario aggiungere ogni edificio nei percorsi di ricerca di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0481c-124">You'll need to add each building into Microsoft Search locations.</span></span> <span data-ttu-id="0481c-125">Per ogni edificio dovrebbe essere presente un formato di denominazione standard.</span><span class="sxs-lookup"><span data-stu-id="0481c-125">You should come up with a standard naming format for each building.</span></span> <span data-ttu-id="0481c-126">È possibile aggiungere l'edificio utilizzando un indirizzo o le coordinate della mappa.</span><span class="sxs-lookup"><span data-stu-id="0481c-126">You can add the building by using a street address or map coordinates.</span></span>     |
|<span data-ttu-id="0481c-127">Proprietà di **Office** in tutti gli account utente</span><span class="sxs-lookup"><span data-stu-id="0481c-127">**Office** property on all user accounts</span></span>     |    <span data-ttu-id="0481c-128">Ogni account utente deve disporre della proprietà **Office** con il relativo percorso di Office.</span><span class="sxs-lookup"><span data-stu-id="0481c-128">Each user account needs to have the **office** property with their office location.</span></span> <span data-ttu-id="0481c-129">E le posizioni degli uffici devono seguire un formato standard e includere informazioni su edifici, pavimenti e sale.</span><span class="sxs-lookup"><span data-stu-id="0481c-129">And office locations should follow a standard format and include building, floor and room info.</span></span>   <br> <span data-ttu-id="0481c-130">In Azure AD, questa proprietà è denominata **PhysicalDeliveryOfficeName**.</span><span class="sxs-lookup"><span data-stu-id="0481c-130">In Azure AD, this property is called **PhysicalDeliveryOfficeName**.</span></span>    |
|<span data-ttu-id="0481c-131">File planimetria in formato DWG</span><span class="sxs-lookup"><span data-stu-id="0481c-131">Floor plan file in DWG format</span></span>     |   <span data-ttu-id="0481c-132">È necessario disporre di una planimetria separata per ogni piano o ala dell'edificio e includere le informazioni di Office nello stesso formato utilizzato nella proprietà Office dell'utente.</span><span class="sxs-lookup"><span data-stu-id="0481c-132">You need a separate floor plan for each floor or wing of your building and include the office information in the same format that you used in the user's Office property.</span></span> <span data-ttu-id="0481c-133">Il file deve essere nel formato DWG di disegno AutoCAD.</span><span class="sxs-lookup"><span data-stu-id="0481c-133">The file needs to be in AutoCAD drawing DWG format.</span></span> |

<span data-ttu-id="0481c-134">Per ulteriori informazioni, vedere [procedure consigliate per i piani di ricerca di Microsoft Search](floorplans-bestpractices.md).</span><span class="sxs-lookup"><span data-stu-id="0481c-134">For more information, see [Best practices for Microsoft Search floor plans](floorplans-bestpractices.md).</span></span>

## <a name="building-location"></a><span data-ttu-id="0481c-135">Posizione dell'edificio</span><span class="sxs-lookup"><span data-stu-id="0481c-135">Building location</span></span>

<span data-ttu-id="0481c-136">Identificare gli edifici che devono essere aggiunti come percorsi.</span><span class="sxs-lookup"><span data-stu-id="0481c-136">Identify the buildings that need to be added as locations.</span></span> <span data-ttu-id="0481c-137">L'indirizzo della posizione e le coordinate della mappa di un edificio sono il primo punto di identificazione.</span><span class="sxs-lookup"><span data-stu-id="0481c-137">The location address and map coordinates of a building are the first point of identification.</span></span> <span data-ttu-id="0481c-138">Se l'edificio non è ancora stato aggiunto come percorso, l'amministratore deve aggiungerlo.</span><span class="sxs-lookup"><span data-stu-id="0481c-138">If the building isn't added yet as a location, the admin needs to add it.</span></span> <span data-ttu-id="0481c-139">Per ulteriori informazioni, vedere [Manage locations](manage-locations.md) .</span><span class="sxs-lookup"><span data-stu-id="0481c-139">See [Manage Locations](manage-locations.md) for more details.</span></span>

## <a name="floor-plans-files"></a><span data-ttu-id="0481c-140">File planimetrie</span><span class="sxs-lookup"><span data-stu-id="0481c-140">Floor plans files</span></span>

<span data-ttu-id="0481c-141">Dopo l'identificazione di un edificio, è possibile aggiungerne le planimetrie.</span><span class="sxs-lookup"><span data-stu-id="0481c-141">After a building is identified, you can add its floor plans.</span></span> <span data-ttu-id="0481c-142">Tutti i file planimetrici devono essere in formato DWG.</span><span class="sxs-lookup"><span data-stu-id="0481c-142">All floor plan files must be in DWG format.</span></span> <span data-ttu-id="0481c-143">Se l'organizzazione non è già in uso, è necessario creare le planimetrie in un'app compatibile con DWG.</span><span class="sxs-lookup"><span data-stu-id="0481c-143">If your organization doesn't already have them, you need to create the floor plans in a DWG-compatible app.</span></span> <span data-ttu-id="0481c-144">Le planimetrie devono mappare correttamente tutte le sale, incluse le sale conferenze o riunioni, i servizi igienici, le cucine, le sale di posta e altre strutture su ogni piano dell'edificio per abilitare la ricerca.</span><span class="sxs-lookup"><span data-stu-id="0481c-144">Floor plans must correctly map all rooms, including conference or meeting rooms, restrooms, kitchens, mail rooms, and other facilities on each floor of the building to enable search.</span></span>

### <a name="office-locations"></a><span data-ttu-id="0481c-145">Percorsi di Office</span><span class="sxs-lookup"><span data-stu-id="0481c-145">Office locations</span></span>

<span data-ttu-id="0481c-146">Per essere mappato a planimetrie, tutte le posizioni di Office e i dati di Office dei dipendenti devono essere nell'account dell'utente.</span><span class="sxs-lookup"><span data-stu-id="0481c-146">To be mapped to floor plans, all office locations and employee office data must be in the user's account.</span></span> <span data-ttu-id="0481c-147">Nella planimetria, i percorsi di Office devono essere univoci e non possono essere ripetuti.</span><span class="sxs-lookup"><span data-stu-id="0481c-147">In the floor plan, the office locations must be unique and cannot repeat.</span></span> <span data-ttu-id="0481c-148">Ad esempio, se due persone condividono Office 2/1173, **2/1173** può avere solo un'istanza univoca nelle planimetrie, ma gli account utente in Azure ad avranno la stessa posizione di Office.</span><span class="sxs-lookup"><span data-stu-id="0481c-148">For example, if two people share office 2/1173, **2/1173** can only have one unique instance in your floor plans, but the user accounts in Azure AD will both have the same office location.</span></span>

![floorplans-peoplecard. png](media/floorplans-peoplecard.png)

 > [!Note] 
 > <span data-ttu-id="0481c-150">Quando un utente cerca una posizione in una stanza o in un'ufficio di un collega, i numeri di sala nei piani di pavimento vengono confrontati con le posizioni di Office in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0481c-150">When a user searches for a room or office location of a colleague, the room numbers in floor plans are matched with office locations in Azure AD.</span></span> <span data-ttu-id="0481c-151">Se viene trovata una corrispondenza, viene mostrata la mappa.</span><span class="sxs-lookup"><span data-stu-id="0481c-151">If a match is found, then the map is shown.</span></span>

## <a name="add-floor-plan"></a><span data-ttu-id="0481c-152">Aggiungere una planimetria</span><span class="sxs-lookup"><span data-stu-id="0481c-152">Add floor plan</span></span>

 <span data-ttu-id="0481c-153">La prima volta che si passa a un piano, potrebbe essere visualizzata una nota nella parte superiore della pagina che indica che *Microsoft deve raccogliere e organizzare le posizioni di Office prima di poter caricare i piani*di base.</span><span class="sxs-lookup"><span data-stu-id="0481c-153">The first time you go to floor plans, you might see a note at the top of the page that says, *Microsoft needs to gather and organize office locations before you can upload floor plans*.</span></span> <span data-ttu-id="0481c-154">Selezionare iniziare a indicizzare le posizioni di **Azure ad Office** .</span><span class="sxs-lookup"><span data-stu-id="0481c-154">Select **Get started** to index your Azure AD office locations.</span></span> 

1. <span data-ttu-id="0481c-155">Nell'interfaccia [di amministrazione](https://admin.microsoft.com), passare a **Impostazioni** > **piani**di**Microsoft Search** >, quindi selezionare **Aggiungi planimetrie**.</span><span class="sxs-lookup"><span data-stu-id="0481c-155">In the [admin center](https://admin.microsoft.com), go to **Settings** > **Microsoft Search** >**Floor plans**, and then select **Add floor plans**.</span></span>
4. <span data-ttu-id="0481c-156">Selezionare l'edificio nell'elenco a discesa e quindi fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="0481c-156">Select the building in the drop-down and select **Next**.</span></span> <span data-ttu-id="0481c-157">Se l'edificio non è elencato, è necessario aggiungerlo nelle posizioni.</span><span class="sxs-lookup"><span data-stu-id="0481c-157">If the building isn't listed, you need to add it in Locations.</span></span> <span data-ttu-id="0481c-158">Per altre informazioni, vedere [Manage locations](manage-locations.md) .</span><span class="sxs-lookup"><span data-stu-id="0481c-158">See [Manage Locations](manage-locations.md) for more info.</span></span>
6. <span data-ttu-id="0481c-159">Selezionare **Carica file**e quindi selezionare la planimetria che si desidera caricare.</span><span class="sxs-lookup"><span data-stu-id="0481c-159">Select **Upload files**, and then select the floor plan you want to upload.</span></span> 
1. <span data-ttu-id="0481c-160">Dopo aver eseguito il caricamento del file, è necessario identificare il numero di piano o l'ala rappresentata.</span><span class="sxs-lookup"><span data-stu-id="0481c-160">After the file uploads successfully, you need to identify how the floor number or wing is represented.</span></span> 
7. <span data-ttu-id="0481c-161">Immettere il codice che identifica l'edificio.</span><span class="sxs-lookup"><span data-stu-id="0481c-161">Enter the code that identifies the building.</span></span> <span data-ttu-id="0481c-162">Il codice dell'edificio può essere trovato nell'account dell'utente nella proprietà **posizione di Office** .</span><span class="sxs-lookup"><span data-stu-id="0481c-162">The building code can be found on the user's account in the **Office location** property.</span></span> <span data-ttu-id="0481c-163">Ad esempio, se l'ubicazione dell'ufficio dell'utente è **2/1173**, il codice di compilazione è **2**.</span><span class="sxs-lookup"><span data-stu-id="0481c-163">For example, if the user's office location is **2/1173**, then building code is **2**.</span></span> 
9. <span data-ttu-id="0481c-164">Esaminare e identificare i modelli di posizione per tutti i piani di pavimento caricati, quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="0481c-164">Review and identify the location patterns for all uploaded floor plans, and then select **Next**.</span></span>
10. <span data-ttu-id="0481c-165">Quando si è pronti, selezionare **pubblica** per rendere ricercabile la planimetria.</span><span class="sxs-lookup"><span data-stu-id="0481c-165">When you're ready, select **Publish** to make the floor plan searchable.</span></span>

> [!Note] 
> <span data-ttu-id="0481c-166">Quando una planimetria si trova in uno stato di sformo, è incompleta.</span><span class="sxs-lookup"><span data-stu-id="0481c-166">When a floor plan is in a draft state, it's incomplete.</span></span> <span data-ttu-id="0481c-167">Una bozza consente alle parti interessate di coordinare il caricamento e la creazione di planimetrie.</span><span class="sxs-lookup"><span data-stu-id="0481c-167">A draft lets stakeholders coordinate in uploading and creating floor plans.</span></span> <span data-ttu-id="0481c-168">Consente inoltre di distribuire piani di piano in fasi.</span><span class="sxs-lookup"><span data-stu-id="0481c-168">It also allows you to deploy floor plans in stages.</span></span>

## <a name="edit-floor-plans"></a><span data-ttu-id="0481c-169">Modificare i piani di piano</span><span class="sxs-lookup"><span data-stu-id="0481c-169">Edit floor plans</span></span>

1. <span data-ttu-id="0481c-170">Nell'interfaccia di [Amministrazione](https://admin.microsoft.com), passare a **Impostazioni** > **piani**di**ricerca di Microsoft Search** > .</span><span class="sxs-lookup"><span data-stu-id="0481c-170">In the [admin center](https://admin.microsoft.com), go to **Settings** > **Microsoft Search** > **Floor plans**.</span></span> 
1. <span data-ttu-id="0481c-171">Selezionare **pubblicato** o **bozza**, selezionare la planimetria che si desidera modificare e quindi scegliere **modifica**.</span><span class="sxs-lookup"><span data-stu-id="0481c-171">Select **Published** or **Draft**, select the floor plan you want to change, and then select **Edit**.</span></span>
5. <span data-ttu-id="0481c-172">Apportare le modifiche, quindi selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="0481c-172">Make your changes, and then select **Save**.</span></span>

## <a name="troubleshoot-errors"></a><span data-ttu-id="0481c-173">Risoluzione dei problemi relativi agli errori</span><span class="sxs-lookup"><span data-stu-id="0481c-173">Troubleshoot errors</span></span>

<span data-ttu-id="0481c-174">Non è possibile passare al passaggio successivo della definizione di informazioni su piano, ala e sala finché non vengono corretti tutti gli errori.</span><span class="sxs-lookup"><span data-stu-id="0481c-174">You can't go to the next step of defining floor, wing, and room information until all errors are fixed.</span></span> <span data-ttu-id="0481c-175">Nel file di tabella seguente vengono caricati i messaggi di errore e le azioni per risolvere i problemi.</span><span class="sxs-lookup"><span data-stu-id="0481c-175">The following table file upload error messages and actions for fixing the issues.</span></span>

| <span data-ttu-id="0481c-176">Messaggio di errore</span><span class="sxs-lookup"><span data-stu-id="0481c-176">Error message</span></span>   | <span data-ttu-id="0481c-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="0481c-177">Type</span></span>    | <span data-ttu-id="0481c-178">Azione</span><span class="sxs-lookup"><span data-stu-id="0481c-178">Action</span></span>       |
|:----------------| :--------- | :-------------- |
| <span data-ttu-id="0481c-179">Impossibile leggere CC_1. dwg.</span><span class="sxs-lookup"><span data-stu-id="0481c-179">Unable to read CC_1.dwg.</span></span> <span data-ttu-id="0481c-180">Ricaricare o eliminare la planimetria.</span><span class="sxs-lookup"><span data-stu-id="0481c-180">Please re-upload or delete the floor plan.</span></span> | <span data-ttu-id="0481c-181">Errore</span><span class="sxs-lookup"><span data-stu-id="0481c-181">Error</span></span> |  <span data-ttu-id="0481c-182">Provare a caricare di nuovo il file.</span><span class="sxs-lookup"><span data-stu-id="0481c-182">Try uploading the file again.</span></span> <span data-ttu-id="0481c-183">Se non funziona, eliminare il file e quindi riprovare.</span><span class="sxs-lookup"><span data-stu-id="0481c-183">If that doesn't work, delete the file, and then try again.</span></span> |
| <span data-ttu-id="0481c-184">Sono disponibili due file denominati CC_1. dwg.</span><span class="sxs-lookup"><span data-stu-id="0481c-184">There are two files named CC_1.dwg.</span></span> <span data-ttu-id="0481c-185">Si prega di eliminare uno di essi o di ricaricare con un altro nome.</span><span class="sxs-lookup"><span data-stu-id="0481c-185">Please delete one of them or re-upload with another name.</span></span>| <span data-ttu-id="0481c-186">Errore</span><span class="sxs-lookup"><span data-stu-id="0481c-186">Error</span></span> | <span data-ttu-id="0481c-187">Se il nome del file non è corretto, rendere il nome del file univoco aggiungendo informazioni su piano o ala e quindi caricare di nuovo il file.</span><span class="sxs-lookup"><span data-stu-id="0481c-187">If the file name is incorrect, make the file name unique by adding floor or wing information, and then upload the file again.</span></span> <br><br><span data-ttu-id="0481c-188">Se lo stesso file è stato aggiunto due volte per sbaglio, è sufficiente eliminarlo.</span><span class="sxs-lookup"><span data-stu-id="0481c-188">If you accidentally added the same file twice, just delete it.</span></span> |
| <span data-ttu-id="0481c-189">Nessun dato trovato.</span><span class="sxs-lookup"><span data-stu-id="0481c-189">No data found.</span></span> | <span data-ttu-id="0481c-190">Errore</span><span class="sxs-lookup"><span data-stu-id="0481c-190">Error</span></span> | <span data-ttu-id="0481c-191">Controllare il file per assicurarsi che sia quello corretto, quindi caricarlo di nuovo oppure eliminarlo.</span><span class="sxs-lookup"><span data-stu-id="0481c-191">Check your file to make sure it's the correct one, and then upload it again, or delete it.</span></span> |
| <span data-ttu-id="0481c-192">I riferimenti esterni sono mancanti in questo file.</span><span class="sxs-lookup"><span data-stu-id="0481c-192">External references are missing in this file.</span></span> <span data-ttu-id="0481c-193">Caricare "CC_1_furniture. dwg" o eliminare il file.</span><span class="sxs-lookup"><span data-stu-id="0481c-193">Either upload "CC_1_furniture.dwg" or delete this file.</span></span> | <span data-ttu-id="0481c-194">Avviso</span><span class="sxs-lookup"><span data-stu-id="0481c-194">Warning</span></span> | <span data-ttu-id="0481c-195">Caricare i file di riferimento esterni o eliminare.</span><span class="sxs-lookup"><span data-stu-id="0481c-195">Upload external reference files or delete.</span></span>|
| <span data-ttu-id="0481c-196">Non è stato possibile leggere i numeri o i tag delle sale nel file DWG.</span><span class="sxs-lookup"><span data-stu-id="0481c-196">Could not read room numbers or tags in the DWG file.</span></span> <span data-ttu-id="0481c-197">Eliminare il file.</span><span class="sxs-lookup"><span data-stu-id="0481c-197">Please delete  this file.</span></span> | <span data-ttu-id="0481c-198">Avviso</span><span class="sxs-lookup"><span data-stu-id="0481c-198">Warning</span></span> | <span data-ttu-id="0481c-199">Controllare il file DWG per assicurarsi che siano inclusi i dati, quindi eliminare il file e riprovare.</span><span class="sxs-lookup"><span data-stu-id="0481c-199">Check your DWG file to make sure the data is included, and then delete the file and try again.</span></span> |