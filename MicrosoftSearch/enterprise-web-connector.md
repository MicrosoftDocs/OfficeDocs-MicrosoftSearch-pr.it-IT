---
title: Connettore siti Web Enterprise per Microsoft Search
ms.author: v-pamcn
author: monaray
manager: mnirkhe
ms.date: 11/04/2019
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
description: Configurare il connettore dei siti Web dell'organizzazione per Microsoft Search
ms.openlocfilehash: 3caca53204bfb2cca4209e048a21173f550e3d39
ms.sourcegitcommit: bfcab9d42e93addccd1e3875b41bc9cc1b6986cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949878"
---
# <a name="enterprise-websites-connector"></a><span data-ttu-id="18d31-103">Connettore siti Web Enterprise</span><span class="sxs-lookup"><span data-stu-id="18d31-103">Enterprise websites connector</span></span>

<span data-ttu-id="18d31-104">Con il connettore siti Web Enterprise, l'organizzazione può indicizzare articoli e **contenuti dai propri siti Web interni**.</span><span class="sxs-lookup"><span data-stu-id="18d31-104">With the Enterprise websites connector, your organization can index articles and **content from its internal-facing websites**.</span></span> <span data-ttu-id="18d31-105">Dopo aver configurato il connettore e aver sincronizzato il contenuto del sito Web, gli utenti finali possono cercare il contenuto proveniente da qualsiasi client di ricerca di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="18d31-105">After you configure the connector and sync content from the website, end users can search for that content from any Microsoft Search client.</span></span>

<span data-ttu-id="18d31-106">Questo articolo è per gli amministratori di Microsoft 365 o per tutti coloro che configurano, eseguono e monitorano un connettore di siti Web dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-106">This article is for Microsoft 365 administrators or anyone who configures, runs, and monitors an Enterprise websites connector.</span></span> <span data-ttu-id="18d31-107">In questo articolo viene illustrato come configurare le funzionalità di connettore e connettore, le limitazioni e le tecniche di risoluzione dei problemi.</span><span class="sxs-lookup"><span data-stu-id="18d31-107">It explains how to configure your connector and connector capabilities, limitations, and troubleshooting techniques.</span></span>  

## <a name="connect-to-a-data-source"></a><span data-ttu-id="18d31-108">Connettersi a un'origine dati</span><span class="sxs-lookup"><span data-stu-id="18d31-108">Connect to a data source</span></span> 
<span data-ttu-id="18d31-109">Per connettersi all'origine dati, è necessario l'URL radice e una forma di autenticazione (autenticazione di base o OAuth 2,0 con Azure AD).</span><span class="sxs-lookup"><span data-stu-id="18d31-109">To connect to your data source, you need your root URL and a form of authentication (Basic Authentication or OAuth 2.0 with Azure AD).</span></span>

### <a name="root-url"></a><span data-ttu-id="18d31-110">URL radice</span><span class="sxs-lookup"><span data-stu-id="18d31-110">Root URL</span></span>
<span data-ttu-id="18d31-111">L'URL radice è ciò che consente di avviare la ricerca per indicizzazione e viene utilizzato per l'autenticazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-111">The root URL is what initiates the crawl and is used for authentication.</span></span> <span data-ttu-id="18d31-112">È possibile ottenere l'URL dalla Home page del sito Web che si desidera sottoporre a ricerca per indicizzazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-112">You can get the URL from the home page of the website you want to crawl.</span></span>

### <a name="authentication"></a><span data-ttu-id="18d31-113">Autenticazione</span><span class="sxs-lookup"><span data-stu-id="18d31-113">Authentication</span></span> 
<span data-ttu-id="18d31-114">L'autenticazione di base richiede un nome utente e una password.</span><span class="sxs-lookup"><span data-stu-id="18d31-114">Basic Authentication requires a username and password.</span></span> <span data-ttu-id="18d31-115">Creare questo account bot utilizzando l'interfaccia di [amministrazione di Microsoft 365](https://admin.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="18d31-115">Create this bot account by using the [Microsoft 365 admin center](https://admin.microsoft.com).</span></span>

<span data-ttu-id="18d31-116">OAuth 2,0 con Azure AD richiede un ID tenant, un ID risorsa, un ID client e un segreto client.</span><span class="sxs-lookup"><span data-stu-id="18d31-116">OAuth 2.0 with Azure AD requires a tenant ID, resource ID, Client ID, and Client Secret.</span></span>
<span data-ttu-id="18d31-117">Per ulteriori informazioni, vedere [autorizzare l'accesso alle applicazioni Web di Azure Active Directory tramite OAuth 2,0 Code Grant Flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-oauth-code).</span><span class="sxs-lookup"><span data-stu-id="18d31-117">For more information, see [Authorize access to Azure Active Directory web applications using OAuth 2.0 code grant flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-oauth-code).</span></span> <span data-ttu-id="18d31-118">Registrarsi con i valori seguenti:</span><span class="sxs-lookup"><span data-stu-id="18d31-118">Register with the following values:</span></span>
* <span data-ttu-id="18d31-119">**Nome:** Microsoft Search</span><span class="sxs-lookup"><span data-stu-id="18d31-119">**Name:** Microsoft Search</span></span>
* <span data-ttu-id="18d31-120">**Redirect_URI:**`https://gcs.office.com/v1.0/admin/oauth/callback`</span><span class="sxs-lookup"><span data-stu-id="18d31-120">**Redirect_URI:** `https://gcs.office.com/v1.0/admin/oauth/callback`</span></span>

<span data-ttu-id="18d31-121">Per ottenere i valori per il tenant denominato, la risorsa, client_id e client_secret, passare a **utilizzare il codice di autorizzazione per richiedere un token di accesso** nella pagina Web URL di reindirizzamento.</span><span class="sxs-lookup"><span data-stu-id="18d31-121">To get the values for named tenant, resource, client_id, and client_secret, go to **Use the authorization code to request an access token** on the redirect URL webpage.</span></span>

<span data-ttu-id="18d31-122">Per ulteriori informazioni, vedere [Guida introduttiva: registrare un'applicazione con la piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="18d31-122">For even more information, see [Quickstart: Register an application with the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app).</span></span>

### <a name="reverse-proxy-url"></a><span data-ttu-id="18d31-123">URL del proxy inverso</span><span class="sxs-lookup"><span data-stu-id="18d31-123">Reverse proxy URL</span></span> 
<span data-ttu-id="18d31-124">Il connettore dei siti Web dell'organizzazione è basato sul cloud, quindi non accede ai contenuti locali.</span><span class="sxs-lookup"><span data-stu-id="18d31-124">The Enterprise websites connector is cloud-based, so it doesn't access on-premises content.</span></span> <span data-ttu-id="18d31-125">Per fornire tale accesso, installare un proxy inverso.</span><span class="sxs-lookup"><span data-stu-id="18d31-125">To provide that access, install a reverse proxy.</span></span> <span data-ttu-id="18d31-126">Un proxy inverso fornisce un accesso sicuro e affidabile ai siti Web locali.</span><span class="sxs-lookup"><span data-stu-id="18d31-126">A reverse proxy provides secure, reliable access to on-premises websites.</span></span> <span data-ttu-id="18d31-127">È consigliabile utilizzare Azure Application Proxy (AAP).</span><span class="sxs-lookup"><span data-stu-id="18d31-127">We recommend Azure Application Proxy (AAP).</span></span>

<span data-ttu-id="18d31-128">Il requisito del proxy inverso per l'URL radice e l'autenticazione è lo stesso per il contenuto basato sul cloud, tranne per il fatto che l'URL radice e l'autenticazione sono forniti dal server proxy inverso.</span><span class="sxs-lookup"><span data-stu-id="18d31-128">The reverse proxy requirement for root URL and authentication is the same as for cloud-based content except that the root URL and authentication are provided by the reverse proxy server.</span></span>

<span data-ttu-id="18d31-129">Vedere [considerazioni sulla sicurezza per l'accesso alle app in remoto con il proxy di applicazione Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-security).</span><span class="sxs-lookup"><span data-stu-id="18d31-129">See [Security considerations for accessing apps remotely with Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-security).</span></span>

## <a name="select-the-source-properties"></a><span data-ttu-id="18d31-130">Selezionare le proprietà di origine</span><span class="sxs-lookup"><span data-stu-id="18d31-130">Select the source properties</span></span> 
<span data-ttu-id="18d31-131">Le proprietà di origine sono definite in base al formato dei dati del sito Web dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-131">Source properties are defined based on the data format of the enterprise website.</span></span> <span data-ttu-id="18d31-132">Tuttavia, è possibile creare un **elenco di esclusione** che escluda che alcuni URL vengano sottoposti a ricerca per indicizzazione dal momento che il contenuto potrebbe essere sensibile o meno.</span><span class="sxs-lookup"><span data-stu-id="18d31-132">However you can create an **Exclusion list** to exclude some URLs from getting crawled since that content might be sensitive or not worth crawling.</span></span> <span data-ttu-id="18d31-133">Per creare un elenco di esclusione, passare all'URL radice.</span><span class="sxs-lookup"><span data-stu-id="18d31-133">To create an exclusion list, browse through the root URL.</span></span> <span data-ttu-id="18d31-134">È possibile aggiungere gli URL esclusi all'elenco durante il processo di configurazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-134">You have the option to add the excluded URLs to the list during the configuration process.</span></span>

## <a name="manage-search-permissions"></a><span data-ttu-id="18d31-135">Gestire le autorizzazioni di ricerca</span><span class="sxs-lookup"><span data-stu-id="18d31-135">Manage search permissions</span></span> 
<span data-ttu-id="18d31-136">Non è disponibile alcun supporto per gli elenchi di controllo di accesso (ACL).</span><span class="sxs-lookup"><span data-stu-id="18d31-136">There is no support for Access Control Lists (ACLs).</span></span> <span data-ttu-id="18d31-137">Pertanto, si consiglia di connettere solo i siti Web che sono visibili a qualsiasi utente all'interno dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-137">Thus, it is advised to connect only the websites that are visible to any user within your organization.</span></span>

## <a name="set-the-refresh-schedule"></a><span data-ttu-id="18d31-138">Impostare la pianificazione di aggiornamento</span><span class="sxs-lookup"><span data-stu-id="18d31-138">Set the refresh schedule</span></span>
<span data-ttu-id="18d31-139">Il connettore dei siti Web dell'organizzazione supporta solo una ricerca per indicizzazione completa.</span><span class="sxs-lookup"><span data-stu-id="18d31-139">The Enterprise websites connector only supports a full crawl.</span></span> <span data-ttu-id="18d31-140">Questo significa che il connettore legge tutto il contenuto del sito Web durante ogni ricerca per indicizzazione.</span><span class="sxs-lookup"><span data-stu-id="18d31-140">This means that the connector reads all the website's content during every crawl.</span></span> <span data-ttu-id="18d31-141">Per assicurarsi che il connettore abbia un tempo sufficiente per leggere il contenuto, è consigliabile impostare un intervallo di pianificazione di aggiornamento di grandi dimensioni.</span><span class="sxs-lookup"><span data-stu-id="18d31-141">To make sure the connector gets enough time to read the content, it is recommended to set a large refresh schedule interval.</span></span> <span data-ttu-id="18d31-142">È consigliabile eseguire un aggiornamento pianificato tra tre giorni e due settimane.</span><span class="sxs-lookup"><span data-stu-id="18d31-142">We recommend a scheduled refresh between three days and two weeks.</span></span>

## <a name="limitations"></a><span data-ttu-id="18d31-143">Limitazioni</span><span class="sxs-lookup"><span data-stu-id="18d31-143">Limitations</span></span> 
<span data-ttu-id="18d31-144">Il connettore dei siti Web dell'organizzazione non supporta la ricerca di dati nelle Web page dinamiche.</span><span class="sxs-lookup"><span data-stu-id="18d31-144">The Enterprise websites connector doesn't support searching data on dynamic webpages.</span></span> <span data-ttu-id="18d31-145">Esempi di tali pagine sono presenti in sistemi di gestione del contenuto, quali confluenza e Unily o database che archiviano il contenuto del sito Web.</span><span class="sxs-lookup"><span data-stu-id="18d31-145">Examples of those webpages live in content management systems like Confluence and Unily or databases that store website content.</span></span>