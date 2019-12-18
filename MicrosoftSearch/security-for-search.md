---
title: Protezione e privacy per Microsoft Search in Bing
ms.author: anfowler
author: adefowler
manager: shohara
ms.audience: Admin
ms.topic: article
ms.service: mssearch
localization_priority: Normal
search.appverid:
- BFB160
- MET150
- MOE150
description: Proteggere i dati dell'azienda e gli utenti finali fornendo informazioni agli utenti autorizzati con Microsoft Search in Bing
ms.openlocfilehash: d3d8822b68fc730885e973c0c24c52070d50eba8
ms.sourcegitcommit: f4cb37fdf85b895337caee827fb72b5b7fcaa8ad
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/12/2019
ms.locfileid: "39995388"
---
# <a name="security-and-privacy-for-microsoft-search-in-bing"></a><span data-ttu-id="cf538-103">Protezione e privacy per Microsoft Search in Bing</span><span class="sxs-lookup"><span data-stu-id="cf538-103">Security and Privacy for Microsoft Search in Bing</span></span>

<span data-ttu-id="cf538-104">Grazie alle misure di sicurezza e privacy migliorate, Microsoft Search in Bing aiuta a proteggere gli utenti e i dati sul posto di lavoro.</span><span class="sxs-lookup"><span data-stu-id="cf538-104">With enhanced privacy and security measures, Microsoft Search in Bing helps protect your users and workplace data.</span></span>

## <a name="secure-by-default"></a><span data-ttu-id="cf538-105">Sicuro per impostazione predefinita</span><span class="sxs-lookup"><span data-stu-id="cf538-105">Secure by default</span></span>

<span data-ttu-id="cf538-106">La ricerca di Microsoft nelle richieste Bing viene effettuata su HTTPS.</span><span class="sxs-lookup"><span data-stu-id="cf538-106">Microsoft Search in Bing requests are made over HTTPS.</span></span> <span data-ttu-id="cf538-107">La connessione è crittografata end-to-end per garantire una maggiore sicurezza.</span><span class="sxs-lookup"><span data-stu-id="cf538-107">The connection is encrypted end-to-end for enhanced security.</span></span>
  
## <a name="authentication-and-authorization-with-azure-active-directory"></a><span data-ttu-id="cf538-108">Autenticazione e autorizzazione con Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cf538-108">Authentication and authorization with Azure Active Directory</span></span>

<span data-ttu-id="cf538-109">L'autenticazione per la ricerca Microsoft in Bing è associata ad Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cf538-109">Authentication for Microsoft Search in Bing is tied to Azure Active Directory.</span></span> <span data-ttu-id="cf538-110">Quando gli utenti di Microsoft Search passano a Bing, l'intestazione Bing mostrerà le opzioni di accesso per un account Microsoft, nonché un account aziendale o dell'Istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="cf538-110">When Microsoft Search users go to Bing, the Bing header will show sign-in options for a Microsoft account as well as a work or school account.</span></span> <span data-ttu-id="cf538-111">Se Bing non è in grado di determinare se un utente è un partecipante idoneo, gli utenti possono accedere alla pagina [Esplora Microsoft Search](https://www.bing.com/business/explore) , in cui verranno automaticamente reindirizzati alla pagina di accesso dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="cf538-111">If Bing can't determine whether a user is an eligible participant, users can go to the [Explore Microsoft Search](https://www.bing.com/business/explore) page, where they'll be automatically redirected to your organization's sign-in page.</span></span>
 
<span data-ttu-id="cf538-p103">Gli utenti possono accedere a Microsoft Search solo con un account aziendale o dell'istituto di istruzione e con le stesse credenziali usate per accedere ai servizi di Office 365, ad esempio SharePoint o Outlook. Non è possibile accedere a Microsoft Search con un account Microsoft personale.</span><span class="sxs-lookup"><span data-stu-id="cf538-p103">Users can access Microsoft Search only through a work or school account. They need to sign in with the same credentials they use to access Office 365 services such as SharePoint or Outlook. A personal Microsoft account can't be used to sign in to Microsoft Search.</span></span>
    
## <a name="single-sign-on"></a><span data-ttu-id="cf538-115">Single Sign-On</span><span class="sxs-lookup"><span data-stu-id="cf538-115">Single sign-on</span></span>

<span data-ttu-id="cf538-116">Se un utente è già autenticato con l'account aziendale o dell'Istituto di istruzione in un altro servizio, ad esempio Outlook o SharePoint, verrà automaticamente firmato nello stesso account di lavoro o dell'Istituto di istruzione quando si accede a Bing nello stesso browser.</span><span class="sxs-lookup"><span data-stu-id="cf538-116">If a user is already authenticated with their work or school account in another service, such as Outlook or SharePoint, they'll be automatically signed into the same work or school account when they go to Bing in the same browser.</span></span> <span data-ttu-id="cf538-117">Inoltre, quando l'utente si disconnette dall'account di lavoro o dell'Istituto di istruzione, verrà automaticamente disconnesso da altri servizi di Microsoft Office nello stesso browser.</span><span class="sxs-lookup"><span data-stu-id="cf538-117">Also, when the user signs out of their work or school account, they'll be automatically signed out from other Microsoft Office services in the same browser.</span></span>
  
## <a name="communicates-with-the-microsoft-cloud-from-the-browser"></a><span data-ttu-id="cf538-118">Comunica con il cloud Microsoft dal browser</span><span class="sxs-lookup"><span data-stu-id="cf538-118">Communicates with the Microsoft cloud from the browser</span></span>

<span data-ttu-id="cf538-119">Quando un utente accede con il proprio account aziendale o dell'Istituto di istruzione, Bing scaricherà le raccolte client necessarie al browser per abilitare i risultati di ricerca di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cf538-119">When a user signs in with their work or school account, Bing will download the necessary client libraries to the browser to enable Microsoft Search results.</span></span> <span data-ttu-id="cf538-120">Successivamente, quando eseguono la ricerca, il codice in-browser chiama il cloud di Office 365 per ottenere i risultati del lavoro.</span><span class="sxs-lookup"><span data-stu-id="cf538-120">Then, when they search, the in-browser code calls the Office 365 cloud to get work results.</span></span> <span data-ttu-id="cf538-121">A tale scopo, Microsoft Search utilizza un'API dedicata che è conforme a Tier C (SOC2 Type 1) in conformità a Office 365 [Compliance Framework for Industry Standards and Regulations] (https://download.microsoft.com/download/B/2/7/B27B3EF3-8849-4C18-8BA4-5AD755728620/Compliance%20Framework_customer%20guidance.pdf) (Download PDF).</span><span class="sxs-lookup"><span data-stu-id="cf538-121">To do this, Microsoft Search uses a dedicated API that is Tier C (SOC2 Type 1) compliant pursuant to the Office 365 [Compliance Framework for Industry Standards and Regulations] (https://download.microsoft.com/download/B/2/7/B27B3EF3-8849-4C18-8BA4-5AD755728620/Compliance%20Framework_customer%20guidance.pdf) (PDF download).</span></span> <span data-ttu-id="cf538-122">Questo significa che i risultati del lavoro e i dati di lavoro non scorrono mai attraverso sistemi Bing non conformi.</span><span class="sxs-lookup"><span data-stu-id="cf538-122">This means work results and work data never flow through non-compliant Bing systems.</span></span>
  
## <a name="permissions"></a><span data-ttu-id="cf538-123">Autorizzazioni</span><span class="sxs-lookup"><span data-stu-id="cf538-123">Permissions</span></span>

<span data-ttu-id="cf538-p106">I risultati di lavoro recuperati dai carichi di lavoro di Office 365, come SharePoint e OneDrive for Business, sono limitati per la sicurezza all'origine. Gli utenti non riescono a visualizzare le risorse come i documenti Word o le presentazioni PowerPoint a cui non possono accedere né visualizzare tramite Office 365, ma vedranno solo i propri file e quelli che sono stati condivisi con loro dall'autore in modo esplicito o implicito (ad esempio, attraverso un'appartenenza al gruppo) in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cf538-p106">Work results retrieved from Office 365 workloads such as SharePoint and OneDrive for Business are security trimmed at the source. Users can't see resources such as Word documents or PowerPoint presentations they can't see and access through Office 365. They can only see their own files and files that have been shared with them by the author explicitly or implicitly (through a group membership, for example) in SharePoint.</span></span>

## <a name="microsoft-search-in-bing-protects-workplace-searches"></a><span data-ttu-id="cf538-127">Microsoft Search in Bing protegge le ricerche sul posto di lavoro</span><span class="sxs-lookup"><span data-stu-id="cf538-127">Microsoft Search in Bing protects workplace searches</span></span>

<span data-ttu-id="cf538-128">Quando un utente immette una query di ricerca in Microsoft Search in Bing, si verificano due richieste di ricerca simultanee:</span><span class="sxs-lookup"><span data-stu-id="cf538-128">When a user enters a search query in Microsoft Search in Bing, two simultaneous search requests occur:</span></span>

- <span data-ttu-id="cf538-129">Una ricerca delle risorse interne dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="cf538-129">A search of your organization’s internal resources.</span></span>
- <span data-ttu-id="cf538-130">Ricerca separata dei risultati pubblici da Bing.com.</span><span class="sxs-lookup"><span data-stu-id="cf538-130">A separate search of public results from Bing.com.</span></span>

<span data-ttu-id="cf538-131">Poiché le ricerche sul posto di lavoro possono essere sensibili, Microsoft Search ha implementato una serie di misure di attendibilità che descrivono in che modo viene gestita la ricerca separata dei risultati pubblici di Bing.com.</span><span class="sxs-lookup"><span data-stu-id="cf538-131">Because workplace searches might be sensitive, Microsoft Search has implemented a set of trust measures that describe how the separate search of public results from Bing.com is handled.</span></span>

### <a name="logging"></a><span data-ttu-id="cf538-132">Registrazione</span><span class="sxs-lookup"><span data-stu-id="cf538-132">Logging</span></span>

<Need an intro paragraph here>

- <span data-ttu-id="cf538-133">Tutti i registri di ricerca di Bing.com che si riferiscono a Microsoft Search nel traffico Bing sono dissociati dall'identità di lavoro.</span><span class="sxs-lookup"><span data-stu-id="cf538-133">All Bing.com search logs that pertain to Microsoft Search in Bing traffic are disassociated from your workplace identity.</span></span>
- <span data-ttu-id="cf538-134">Se viene soddisfatta una serie di restrizioni o soglie di frequenza che forniscono la sicurezza che la query non è specifica di una determinata organizzazione, la query viene trattata come descritto nella sezione ricerca e intelligenza artificiale dell' [informativa sulla privacy](https://privacy.microsoft.com/privacystatement).</span><span class="sxs-lookup"><span data-stu-id="cf538-134">If a set of restrictions or frequency thresholds are met which give us confidence that the query is not specific to a particular organization, the query will be treated as described in the Search and artificial intelligence section of the [Privacy Statement](https://privacy.microsoft.com/privacystatement).</span></span> <span data-ttu-id="cf538-135">Ad esempio, tali query verranno utilizzate per modellare e formare le caratteristiche pubbliche, come l'autosuggestione o le ricerche correlate.</span><span class="sxs-lookup"><span data-stu-id="cf538-135">For example, such queries will be used to model and train public features, such as autosuggest or related searches.</span></span>
- <span data-ttu-id="cf538-136">Le query che non soddisfano la serie di restrizioni o soglie di frequenza verranno archiviate separatamente dal traffico pubblico non di Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="cf538-136">Queries that do not meet the set of restrictions or frequency thresholds will be stored separately from public, non-Microsoft Search traffic.</span></span>

### <a name="advertising"></a><span data-ttu-id="cf538-137">Pubblicità</span><span class="sxs-lookup"><span data-stu-id="cf538-137">Advertising</span></span>

<span data-ttu-id="cf538-138">La pubblicità mostrata su Bing.com in connessione con le ricerche sul posto di lavoro è solo correlata al contenuto delle query di ricerca.</span><span class="sxs-lookup"><span data-stu-id="cf538-138">Advertising shown on Bing.com in connection with workplace searches is solely related to the content of the search queries.</span></span> <span data-ttu-id="cf538-139">Le inserzioni non vengono mai personalizzate in base all'identità professionale degli utenti.</span><span class="sxs-lookup"><span data-stu-id="cf538-139">Ads are never targeted to users based on their workplace identity.</span></span>
     
## <a name="gdpr"></a><span data-ttu-id="cf538-140">GDPR</span><span class="sxs-lookup"><span data-stu-id="cf538-140">GDPR</span></span>

<span data-ttu-id="cf538-141">Il [21 maggio 2018 post di Blog](https://blogs.microsoft.com/on-the-issues/2018/05/21/microsofts-commitment-to-gdpr-privacy-and-putting-customers-in-control-of-their-own-data/) di Microsoft riflette il nostro impegno per la conformità di GDPR e in che modo Microsoft aiuta le aziende e le organizzazioni con i propri obblighi di conformità a GDPR.</span><span class="sxs-lookup"><span data-stu-id="cf538-141">The [May 21, 2018, blog post](https://blogs.microsoft.com/on-the-issues/2018/05/21/microsofts-commitment-to-gdpr-privacy-and-putting-customers-in-control-of-their-own-data/) from Microsoft reflects our commitment to GDPR compliance and how Microsoft helps businesses and organizations with their own GDPR compliance obligations.</span></span> <span data-ttu-id="cf538-142">È possibile trovare ulteriori dettagli nelle [domande frequenti sul Centro protezione](https://www.microsoft.com/trustcenter/privacy/gdpr/gdpr-faqs)Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cf538-142">You can find additional detail in the Microsoft [Trust Center FAQ](https://www.microsoft.com/trustcenter/privacy/gdpr/gdpr-faqs).</span></span> 

<span data-ttu-id="cf538-143">Le query di ricerca di Microsoft eseguite sulle risorse interne del cliente e i risultati restituiti sono considerati dati dei clienti e, come tali, soddisfano anche gli impegni del processore descritti nell'articolo 28 come riflesso nelle [domande frequenti sul Centro protezione](https://www.microsoft.com/trustcenter/privacy/gdpr/gdpr-faqs).</span><span class="sxs-lookup"><span data-stu-id="cf538-143">Microsoft Search queries executed against a customer’s internal resources and results returned are considered Customer Data and, as such, also  meet the processor commitments outlined in Article 28 as reflected in the [Trust Center FAQ](https://www.microsoft.com/trustcenter/privacy/gdpr/gdpr-faqs).</span></span> <span data-ttu-id="cf538-144">Per quanto riguarda le query da Microsoft Search che passano a Bing pubblico, Microsoft è conforme ai propri obblighi GDPR come titolare del trattamento dei dati.</span><span class="sxs-lookup"><span data-stu-id="cf538-144">With respect to queries from Microsoft Search that go to public Bing, Microsoft complies with its GDPR obligations as a data controller.</span></span>
