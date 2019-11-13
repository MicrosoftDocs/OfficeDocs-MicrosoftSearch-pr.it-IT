---
title: Configurare il connettore Microsoft-built per Microsoft Search
ms.author: v-pamcn
author: monaray
manager: shohara
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
description: Configurare il connettore Microsoft-built per Microsoft Search
ms.openlocfilehash: aee7c142e8cf04349076030cdedde0cea7344906
ms.sourcegitcommit: bfcab9d42e93addccd1e3875b41bc9cc1b6986cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949860"
---
# <a name="set-up-your-microsoft-built-connector-for-microsoft-search"></a><span data-ttu-id="30972-103">Configurare il connettore Microsoft-built per Microsoft Search</span><span class="sxs-lookup"><span data-stu-id="30972-103">Set up your Microsoft-built connector for Microsoft Search</span></span>

<span data-ttu-id="30972-104">In questo articolo vengono illustrati i passaggi per la configurazione di un connettore basato su Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30972-104">This article guides you through the steps of configuring a Microsoft-built connector.</span></span> <span data-ttu-id="30972-105">Descrive il flusso di configurazione di una connessione nell'interfaccia di amministrazione di [Microsoft 365](https://admin.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="30972-105">It outlines the flow of setting up a connection in the [Microsoft 365 admin center](https://admin.microsoft.com).</span></span> <span data-ttu-id="30972-106">Per ulteriori informazioni su come configurare connettori basati su Microsoft specifici, vedere gli articoli seguenti:</span><span class="sxs-lookup"><span data-stu-id="30972-106">For more details on how to set up specific Microsoft-built connectors, see these articles:</span></span>
* [<span data-ttu-id="30972-107">Gen2 di archiviazione di Azure Data Lake</span><span class="sxs-lookup"><span data-stu-id="30972-107">Azure Data Lake Storage Gen2</span></span>](azure-data-lake-connector.md)
* [<span data-ttu-id="30972-108">Siti Web aziendali</span><span class="sxs-lookup"><span data-stu-id="30972-108">Enterprise websites</span></span>](enterprise-web-connector.md)
* [<span data-ttu-id="30972-109">Condivisione file</span><span class="sxs-lookup"><span data-stu-id="30972-109">File share</span></span>](file-share-connector.md)
* [<span data-ttu-id="30972-110">MediaWiki</span><span class="sxs-lookup"><span data-stu-id="30972-110">MediaWiki</span></span>](mediawiki-connector.md)
* [<span data-ttu-id="30972-111">Microsoft SQL Server</span><span class="sxs-lookup"><span data-stu-id="30972-111">Microsoft SQL server</span></span>](MSSQL-connector.md)
* [<span data-ttu-id="30972-112">ServiceNow</span><span class="sxs-lookup"><span data-stu-id="30972-112">ServiceNow</span></span>](servicenow-connector.md)

## <a name="set-up"></a><span data-ttu-id="30972-113">Configurazione</span><span class="sxs-lookup"><span data-stu-id="30972-113">Set up</span></span>
<span data-ttu-id="30972-114">Per configurare uno qualsiasi dei connettori Microsoft-built, accedere all'interfaccia di [amministrazione di microsoft 365](https://admin.microsoft.com):</span><span class="sxs-lookup"><span data-stu-id="30972-114">To configure any of the Microsoft-built connectors, go to the [Microsoft 365 admin center](https://admin.microsoft.com):</span></span>
1. <span data-ttu-id="30972-115">Accedere al proprio account con le credenziali per il tenant di testing di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="30972-115">Sign in to your account with the credentials for your Microsoft 365 test tenant.</span></span>
2. <span data-ttu-id="30972-116">Passare a **Impostazioni** > \*\*\*\* > **connettori**di ricerca di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30972-116">Go to **Settings** > **Microsoft Search** > **Connectors**.</span></span>
3. <span data-ttu-id="30972-117">Selezionare **Aggiungi un connettore**.</span><span class="sxs-lookup"><span data-stu-id="30972-117">Select **Add a connector**.</span></span>
4. <span data-ttu-id="30972-118">Nell'elenco dei connettori disponibili, selezionare il connettore desiderato.</span><span class="sxs-lookup"><span data-stu-id="30972-118">From the list of available connectors, select the connector of your choice.</span></span>

![](media/addconnector_final.png)

### <a name="name-the-connector"></a><span data-ttu-id="30972-119">Assegnare un nome al connettore</span><span class="sxs-lookup"><span data-stu-id="30972-119">Name the connector</span></span>
<span data-ttu-id="30972-120">Per creare una connessione, specificare innanzitutto gli attributi seguenti:</span><span class="sxs-lookup"><span data-stu-id="30972-120">To create a connection, first specify these attributes:</span></span>
1. <span data-ttu-id="30972-121">Nome della connessione</span><span class="sxs-lookup"><span data-stu-id="30972-121">Name of the connection</span></span>
2. <span data-ttu-id="30972-122">ID connessione</span><span class="sxs-lookup"><span data-stu-id="30972-122">Connection ID</span></span>
3. <span data-ttu-id="30972-123">Descrizione (facoltativa)</span><span class="sxs-lookup"><span data-stu-id="30972-123">Description (optional)</span></span>

<span data-ttu-id="30972-124">L'ID di connessione crea proprietà implicite per il connettore.</span><span class="sxs-lookup"><span data-stu-id="30972-124">The connection ID creates implicit properties for your connector.</span></span> <span data-ttu-id="30972-125">Deve contenere solo caratteri alfanumerici e avere un massimo di 32 caratteri.</span><span class="sxs-lookup"><span data-stu-id="30972-125">It must contain only alphanumeric characters and be a maximum of 32 characters.</span></span>

### <a name="connect-to-a-data-source"></a><span data-ttu-id="30972-126">Connettersi a un'origine dati</span><span class="sxs-lookup"><span data-stu-id="30972-126">Connect to a data source</span></span>
<span data-ttu-id="30972-127">Il processo di connessione dati varia in base al tipo di connettore.</span><span class="sxs-lookup"><span data-stu-id="30972-127">The data connection process varies based on the type of connector.</span></span> <span data-ttu-id="30972-128">Per ulteriori informazioni sulla connessione all'origine dati locale, vedere [Install an on-premises Data Gateway](https://aka.ms/configuregateway).</span><span class="sxs-lookup"><span data-stu-id="30972-128">To learn more about connecting to your on-premises data source, see [Install an on-premises data gateway](https://aka.ms/configuregateway).</span></span>

### <a name="select-source-properties"></a><span data-ttu-id="30972-129">Selezionare le proprietà di origine</span><span class="sxs-lookup"><span data-stu-id="30972-129">Select source properties</span></span>
<span data-ttu-id="30972-130">I campi dati impostati dall'origine dati di terze parti come proprietà di origine vengono indicizzati in Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="30972-130">The data fields set by your third-party data source as source properties are indexed into Microsoft Search.</span></span> <span data-ttu-id="30972-131">Per modificare queste proprietà, selezionare **modifica proprietà** nella barra laterale a destra della pagina **connettori** .</span><span class="sxs-lookup"><span data-stu-id="30972-131">To modify these properties, select **Edit properties** in the side bar on the right of the **Connectors** page.</span></span> <span data-ttu-id="30972-132">È possibile selezionare **fino a 64 proprietà di origine**.</span><span class="sxs-lookup"><span data-stu-id="30972-132">You can select **up to 64 source properties**.</span></span>

###  <a name="manage-the-search-schema"></a><span data-ttu-id="30972-133">Gestire lo schema di ricerca</span><span class="sxs-lookup"><span data-stu-id="30972-133">Manage the search schema</span></span> 
<span data-ttu-id="30972-134">Gli amministratori possono impostare gli attributi dello schema di ricerca per controllare la funzionalità di ricerca di ogni proprietà di origine.</span><span class="sxs-lookup"><span data-stu-id="30972-134">Admins can set the search schema attributes to control search functionality of each source property.</span></span> <span data-ttu-id="30972-135">Uno schema di ricerca consente di determinare quali risultati vengono visualizzati nella pagina dei risultati di ricerca e quali informazioni possono essere visualizzate e accessibili dagli utenti finali.</span><span class="sxs-lookup"><span data-stu-id="30972-135">A search schema helps determine what results display on the search results page and what information end users can view and access.</span></span>

<span data-ttu-id="30972-136">Gli attributi dello schema di ricerca includono **ricercabili**, **Queryable**e **recuperabili**.</span><span class="sxs-lookup"><span data-stu-id="30972-136">Search schema attributes include **searchable**, **queryable**, and **retrievable**.</span></span> <span data-ttu-id="30972-137">Nella tabella seguente sono elencati tutti gli attributi supportati da Microsoft Graph e vengono illustrate le loro funzioni.</span><span class="sxs-lookup"><span data-stu-id="30972-137">The following table lists each of the attributes that Microsoft Graph connectors support and explains their functions.</span></span>

<span data-ttu-id="30972-138">**Attributo dello schema di ricerca**</span><span class="sxs-lookup"><span data-stu-id="30972-138">**Search schema attribute**</span></span> | <span data-ttu-id="30972-139">**Funzione**</span><span class="sxs-lookup"><span data-stu-id="30972-139">**Function**</span></span> | <span data-ttu-id="30972-140">**Esempio**</span><span class="sxs-lookup"><span data-stu-id="30972-140">**Example**</span></span>
--- | --- | ---
<span data-ttu-id="30972-141">RICERCHE</span><span class="sxs-lookup"><span data-stu-id="30972-141">SEARCHABLE</span></span> | <span data-ttu-id="30972-142">Consente di eseguire ricerche nel contenuto del testo di una proprietà.</span><span class="sxs-lookup"><span data-stu-id="30972-142">Makes the text content of a property searchable.</span></span> <span data-ttu-id="30972-143">Il contenuto della proprietà è incluso nell'indice full-text.</span><span class="sxs-lookup"><span data-stu-id="30972-143">Property contents are included in the full-text index.</span></span> | <span data-ttu-id="30972-144">Se la proprietà è "title", una query per "Enterprise" restituirà risposte che contengono la parola "Enterprise" in qualsiasi testo o titolo.</span><span class="sxs-lookup"><span data-stu-id="30972-144">If the property is "title," a query for "Enterprise" returns answers that contain the word "Enterprise" in any text or title.</span></span>
<span data-ttu-id="30972-145">QUERY</span><span class="sxs-lookup"><span data-stu-id="30972-145">QUERYABLE</span></span> | <span data-ttu-id="30972-146">Esegue una ricerca in base alla query per una corrispondenza per una proprietà specifica.</span><span class="sxs-lookup"><span data-stu-id="30972-146">Searches by query for a match for a particular property.</span></span> <span data-ttu-id="30972-147">Il nome della proprietà può quindi essere specificato nella query a livello di programmazione o Verbatim.</span><span class="sxs-lookup"><span data-stu-id="30972-147">The property name can then be specified in the query either programmatically or verbatim.</span></span> |  <span data-ttu-id="30972-148">Se la proprietà "title" è Queryable, la query "title: Enterprise" è supportata.</span><span class="sxs-lookup"><span data-stu-id="30972-148">If the "Title" property is queryable, then the query  “Title: Enterprise” is supported.</span></span>
<span data-ttu-id="30972-149">RECUPERATE</span><span class="sxs-lookup"><span data-stu-id="30972-149">RETRIEVABLE</span></span> | <span data-ttu-id="30972-150">È possibile utilizzare solo le proprietà recuperabili nel tipo di risultato e visualizzabili nei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="30972-150">Only retrievable properties can be used in result type and displayable in the search result.</span></span> | 

<span data-ttu-id="30972-151">Per tutti i connettori, ad eccezione del connettore di condivisione file, è necessario impostare manualmente i tipi personalizzati.</span><span class="sxs-lookup"><span data-stu-id="30972-151">For all connectors except the file share connector, custom types must be set manually.</span></span> <span data-ttu-id="30972-152">Per attivare le funzionalità di ricerca per ogni campo, è necessario uno schema di ricerca mappato a un elenco di proprietà.</span><span class="sxs-lookup"><span data-stu-id="30972-152">To activate search capabilities for each field, you need a search schema mapped to a list of properties.</span></span> <span data-ttu-id="30972-153">La procedura guidata consente di selezionare automaticamente uno schema di ricerca basato sul set di proprietà di origine che si desidera scegliere.</span><span class="sxs-lookup"><span data-stu-id="30972-153">The connection wizard automatically selects a search schema based on the set of source properties you choose.</span></span> <span data-ttu-id="30972-154">È possibile modificare questo schema facendo clic sulle caselle di controllo per ogni proprietà e attributo nella pagina schema di ricerca.</span><span class="sxs-lookup"><span data-stu-id="30972-154">You can modify this schema by clicking the check boxes for each property and attribute in the search schema page.</span></span>

![Lo schema per un connettore può essere personalizzato aggiungendo o rimuovendo le funzioni query, Search e retrieve.](media/manageschema.png)

<span data-ttu-id="30972-156">Queste restrizioni e suggerimenti si applicano alle impostazioni dello schema di ricerca:</span><span class="sxs-lookup"><span data-stu-id="30972-156">These restrictions and recommendations apply to search schema settings:</span></span>
* <span data-ttu-id="30972-157">Per i connettori che indicino tipi personalizzati, è consigliabile **non** contrassegnare il campo che contiene il contenuto principale **recuperabile**.</span><span class="sxs-lookup"><span data-stu-id="30972-157">For connectors that index custom types, we recommend that you **do not** mark the field that contains the main content **retrievable**.</span></span> <span data-ttu-id="30972-158">Quando i risultati della ricerca eseguono il rendering con quell'attributo di ricerca, si verificano problemi significativi.</span><span class="sxs-lookup"><span data-stu-id="30972-158">Significant performance issues occur when search results render with that search attribute.</span></span> <span data-ttu-id="30972-159">Un esempio è il campo di contenuto di **testo** per un articolo della Knowledge base di ServiceNow.</span><span class="sxs-lookup"><span data-stu-id="30972-159">An example is the **Text** content field for a ServiceNow knowledge-base article.</span></span>
* <span data-ttu-id="30972-160">Solo le proprietà contrassegnate come rendering recuperabili nei risultati della ricerca possono essere utilizzate per creare i tipi di risultati moderni (MRTs).</span><span class="sxs-lookup"><span data-stu-id="30972-160">Only properties marked as retrievable render in the search results and can be used to create modern result types (MRTs).</span></span>
* <span data-ttu-id="30972-161">Solo le proprietà della stringa possono essere contrassegnate come ricercabili.</span><span class="sxs-lookup"><span data-stu-id="30972-161">Only string properties can be marked searchable.</span></span>

> [!Note]
> <span data-ttu-id="30972-162">Dopo aver creato una connessione, **non è possibile** modificare lo schema.</span><span class="sxs-lookup"><span data-stu-id="30972-162">After you create a connection, you **can't** modify the schema.</span></span> <span data-ttu-id="30972-163">A tale scopo, è necessario eliminare la connessione e crearne uno nuovo.</span><span class="sxs-lookup"><span data-stu-id="30972-163">To do that, you need to delete your connection and create a new one.</span></span>

###  <a name="manage-search-permissions"></a><span data-ttu-id="30972-164">Gestire le autorizzazioni di ricerca</span><span class="sxs-lookup"><span data-stu-id="30972-164">Manage search permissions</span></span>
<span data-ttu-id="30972-165">Gli elenchi di controllo di accesso (ACL, Access Control List) determinano gli utenti dell'organizzazione che possono accedere a ogni elemento di dati.</span><span class="sxs-lookup"><span data-stu-id="30972-165">Access Control Lists (ACLs) determine which users in your organization can access each item of data.</span></span> <span data-ttu-id="30972-166">Il connettore di condivisione file supporta solo gli elenchi ACL che è possibile mappare a [Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="30972-166">The file share connector supports only ACLs that can be mapped to [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/).</span></span> <span data-ttu-id="30972-167">Tutti gli altri connettori supportano le autorizzazioni di ricerca che sono visibili a tutti gli utenti.</span><span class="sxs-lookup"><span data-stu-id="30972-167">All the other connectors support search permissions that are visible to all users.</span></span>

### <a name="set-the-refresh-schedule"></a><span data-ttu-id="30972-168">Impostare la pianificazione di aggiornamento</span><span class="sxs-lookup"><span data-stu-id="30972-168">Set the refresh schedule</span></span>
<span data-ttu-id="30972-169">La pianificazione di aggiornamento determina la frequenza con cui i dati vengono sincronizzati con l'indice in Microsoft Graph e Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="30972-169">The refresh schedule determines how often your data is synced with the index in Microsoft Graph and Microsoft Search.</span></span> <span data-ttu-id="30972-170">È possibile pianificare l'aggiornamento in due modi: ricerca per indicizzazione completa o ricerca per indicizzazione incrementale.</span><span class="sxs-lookup"><span data-stu-id="30972-170">You can schedule the refresh in two ways: full crawl or incremental crawl.</span></span>

<span data-ttu-id="30972-171">Con una ricerca per indicizzazione **completa**, il motore di ricerca elabora e indicizza tutti gli elementi nell'origine di contenuto, indipendentemente dalle ricerche per indicizzazione precedenti.</span><span class="sxs-lookup"><span data-stu-id="30972-171">With a **full crawl**, the search engine processes and indexes every item in the content source, regardless of previous crawls.</span></span> <span data-ttu-id="30972-172">La ricerca per indicizzazione completa funziona meglio in queste situazioni:</span><span class="sxs-lookup"><span data-stu-id="30972-172">Full crawl works best in these situations:</span></span>
* <span data-ttu-id="30972-173">È necessario rilevare le eliminazioni di dati.</span><span class="sxs-lookup"><span data-stu-id="30972-173">You need to detect deletions of data.</span></span>
* <span data-ttu-id="30972-174">La ricerca per indicizzazione incrementale non è riuscita a eseguire la ricerca per errori.</span><span class="sxs-lookup"><span data-stu-id="30972-174">The incremental crawl failed to crawl content for errors.</span></span>
* <span data-ttu-id="30972-175">È necessario un aggiornamento software per Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="30972-175">A software update for Microsoft Search is required.</span></span> <span data-ttu-id="30972-176">Gli aggiornamenti modificano lo schema di ricerca.</span><span class="sxs-lookup"><span data-stu-id="30972-176">Updates modify the search schema.</span></span>
* <span data-ttu-id="30972-177">Gli elenchi ACL sono stati modificati.</span><span class="sxs-lookup"><span data-stu-id="30972-177">ACLs were modified.</span></span>
* <span data-ttu-id="30972-178">Sono state modificate regole di ricerca per indicizzazione.</span><span class="sxs-lookup"><span data-stu-id="30972-178">Crawl rules were modified.</span></span>

<span data-ttu-id="30972-179">Con una ricerca per **indicizzazione incrementale**, è possibile elaborare e indicizzare solo gli elementi che sono stati creati o modificati dopo l'ultima ricerca per indicizzazione riuscita.</span><span class="sxs-lookup"><span data-stu-id="30972-179">With an **incremental crawl**, the search engine can process and index only the items that were created or modified since the last successful crawl.</span></span> <span data-ttu-id="30972-180">Pertanto, non tutti i dati nell'origine di contenuto vengono reindicizzati.</span><span class="sxs-lookup"><span data-stu-id="30972-180">Therefore, not all the data in the content source is re-indexed.</span></span> <span data-ttu-id="30972-181">Le ricerche per indicizzazione incrementali funzionano meglio per rilevare contenuti, metadati, autorizzazioni e altri aggiornamenti.</span><span class="sxs-lookup"><span data-stu-id="30972-181">Incremental crawls works best to detect content, metadata, permission, and other updates.</span></span>

<span data-ttu-id="30972-182">Le ricerche per indicizzazione incrementali sono molto più veloci delle ricerche per indicizzazione complete perché non vengono elaborati elementi non modificati.</span><span class="sxs-lookup"><span data-stu-id="30972-182">Incremental crawls are much faster than full crawls because unchanged items aren’t processed.</span></span> <span data-ttu-id="30972-183">Per mantenere una sincronizzazione accurata dei dati tra l'origine di contenuto e l'indice di ricerca, è necessario eseguire periodicamente entrambe le ricerche per indicizzazione.</span><span class="sxs-lookup"><span data-stu-id="30972-183">To maintain an accurate data sync between the content source and the search index, you need to run both crawls periodically.</span></span>

<span data-ttu-id="30972-184">Ogni connettore avrà un insieme ottimale di pianificazioni di aggiornamento in base alla frequenza con cui i dati vengono modificati e al tipo di modifica.</span><span class="sxs-lookup"><span data-stu-id="30972-184">Each connector will have a different optimal set of refresh schedules based on how often data is modified and the type of modifications.</span></span>

![Impostazioni di ricerca per indicizzazione incrementali e intere per la ricerca per indicizzazione con incremento a 15 minuti e ricerca per indicizzazione completa](media/refreshschedule.png)

### <a name="review-connector-settings"></a><span data-ttu-id="30972-186">Esaminare le impostazioni del connettore</span><span class="sxs-lookup"><span data-stu-id="30972-186">Review connector settings</span></span>
<span data-ttu-id="30972-187">Dopo aver configurato il connettore, l'interfaccia di [amministrazione di Microsoft 365](https://admin.microsoft.com) porta a una pagina in cui è possibile rivedere le impostazioni.</span><span class="sxs-lookup"><span data-stu-id="30972-187">After you configure your connector, the [Microsoft 365 admin center](https://admin.microsoft.com) takes you to a page where you can review your settings.</span></span> <span data-ttu-id="30972-188">È possibile tornare indietro nel processo di configurazione per modificare le impostazioni prima di confermare la connessione.</span><span class="sxs-lookup"><span data-stu-id="30972-188">You can go back through the configuration process to edit any setting before you confirm the connection.</span></span> <span data-ttu-id="30972-189">Per ulteriori informazioni, vedere [gestire il connettore](manage-connector.md).</span><span class="sxs-lookup"><span data-stu-id="30972-189">To learn more, see [Manage your connector](manage-connector.md).</span></span>

## <a name="next-steps-customize-the-search-results-page"></a><span data-ttu-id="30972-190">Passaggi successivi: personalizzare la pagina dei risultati di ricerca</span><span class="sxs-lookup"><span data-stu-id="30972-190">Next steps: Customize the search results page</span></span>
<span data-ttu-id="30972-191">Con l'interfaccia utente di Microsoft Search (UI), gli utenti finali possono ricercare contenuto dalle app di produttività Microsoft 365 e dall'ecosistema Microsoft più ampio.</span><span class="sxs-lookup"><span data-stu-id="30972-191">With the Microsoft Search user interface (UI), your end users can search content from your Microsoft 365 productivity apps and the broader Microsoft ecosystem.</span></span> <span data-ttu-id="30972-192">Un verticale di ricerca si riferisce alle schede visualizzate quando un utente Visualizza i risultati della ricerca in SharePoint, Office.com e Microsoft Search in Bing.</span><span class="sxs-lookup"><span data-stu-id="30972-192">A search vertical refers to the tabs that are shown when a user views their search results in SharePoint, Office.com, and Microsoft Search in Bing.</span></span> <span data-ttu-id="30972-193">È possibile personalizzare i verticali di ricerca per limitare i risultati in modo che venga visualizzato solo un determinato tipo di risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="30972-193">You can customize search verticals to narrow down results so that only a certain type of search results is displayed.</span></span> <span data-ttu-id="30972-194">Tali verticali vengono visualizzate come una tabulazione nella parte superiore della pagina dei risultati di ricerca.</span><span class="sxs-lookup"><span data-stu-id="30972-194">These verticals appear as a tab on the top of the search results page.</span></span> <span data-ttu-id="30972-195">Un tipo di risultato moderno (MRT) è l'interfaccia utente che designa il modo in cui vengono presentati i risultati.</span><span class="sxs-lookup"><span data-stu-id="30972-195">A modern result type (MRT) is the UI that designates how results are presented.</span></span>

<span data-ttu-id="30972-196">È necessario creare i propri tipi di verticali e di risultati, in modo che gli utenti finali possano visualizzare i risultati della ricerca dalle nuove connessioni.</span><span class="sxs-lookup"><span data-stu-id="30972-196">You must create your own verticals and result types, so end users can view search results from new connections.</span></span> <span data-ttu-id="30972-197">Senza questo passaggio, i dati della connessione non verranno visualizzati nella pagina dei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="30972-197">Without this step, data from your connection won’t show up on the search results page.</span></span>

<span data-ttu-id="30972-198">Per ulteriori informazioni su come creare i verticali e MRTs, vedere Personalizzazione della [pagina dei risultati di ricerca](customize-search-page.md).</span><span class="sxs-lookup"><span data-stu-id="30972-198">To learn more about how to create your verticals and MRTs, see [Search results page customization](customize-search-page.md).</span></span>

## <a name="how-do-i-know-this-worked"></a><span data-ttu-id="30972-199">Come verificare se l'operazione ha avuto esito positivo?</span><span class="sxs-lookup"><span data-stu-id="30972-199">How do I know this worked?</span></span>
<span data-ttu-id="30972-200">Passare all'elenco delle connessioni pubblicate sotto la scheda **connettori** nell'interfaccia di [amministrazione di Microsoft 365](https://admin.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="30972-200">Go to the list of your published connections under the **Connectors** tab in the [Microsoft 365 admin center](https://admin.microsoft.com).</span></span> <span data-ttu-id="30972-201">Per informazioni su come effettuare aggiornamenti ed eliminazioni, vedere [gestire il connettore](manage-connector.md).</span><span class="sxs-lookup"><span data-stu-id="30972-201">To learn how to make updates and deletions, see [Manage your connector](manage-connector.md).</span></span>