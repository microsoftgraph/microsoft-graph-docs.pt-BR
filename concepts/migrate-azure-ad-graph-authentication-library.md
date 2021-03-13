---
title: Revisar alterações na biblioteca de autenticação de aplicativos
description: Descreve como atualizar o uso da biblioteca de autenticação para migrar um aplicativo de aplicativos da API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: ef49c6a3448dd63a7c933bb40748f218d6fd2db0
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760683"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="c639f-103">Revisar alterações na biblioteca de autenticação de aplicativos</span><span class="sxs-lookup"><span data-stu-id="c639f-103">Review app authentication library changes</span></span>

<span data-ttu-id="c639f-104">Este artigo faz parte da *etapa 3:* revisar detalhes do aplicativo do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="c639f-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="c639f-105">A maioria dos aplicativos usa uma biblioteca de autenticação para adquirir e gerenciar tokens de acesso para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c639f-105">Most apps use an authentication library to acquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="c639f-106">A Microsoft oferece duas bibliotecas de autenticação:</span><span class="sxs-lookup"><span data-stu-id="c639f-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="c639f-107">[Biblioteca de autenticação do Azure Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span><span class="sxs-lookup"><span data-stu-id="c639f-107">[Azure Active Directory authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="c639f-108">[Biblioteca de autenticação da Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span><span class="sxs-lookup"><span data-stu-id="c639f-108">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="c639f-109">Atualizando o ADAL</span><span class="sxs-lookup"><span data-stu-id="c639f-109">Updating ADAL</span></span>

<span data-ttu-id="c639f-110">Se o aplicativo usa atualmente o ADAL, use uma abordagem de migração de dois estágios:</span><span class="sxs-lookup"><span data-stu-id="c639f-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="c639f-111">Atualize seu aplicativo para adquirir tokens de acesso para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c639f-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="c639f-112">Continue a usar o ADAL para esta etapa.</span><span class="sxs-lookup"><span data-stu-id="c639f-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="c639f-113">Atualize **o resourceURL**, que contém o URI que representa a API da Web de recursos, a partir de:</span><span class="sxs-lookup"><span data-stu-id="c639f-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="c639f-114">Para:</span><span class="sxs-lookup"><span data-stu-id="c639f-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="c639f-115">Tokens recém-adquiridos têm os mesmos escopos após essa alteração, mas o público-alvo dos tokens de acesso agora é o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c639f-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="c639f-116">Depois de atualizar **resourceURL** e verificar a funcionalidade, libere uma atualização provisória para fazer com que os usuários se atualizem e executem.</span><span class="sxs-lookup"><span data-stu-id="c639f-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="c639f-117">Em seguida, comece a trabalhar migrando seu aplicativo para usar o MSAL, que é a biblioteca com suporte para usar o avançar, agora que o ADAL está preterido.</span><span class="sxs-lookup"><span data-stu-id="c639f-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward, now that ADAL is deprecated.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="c639f-118">Migrando para o MSAL</span><span class="sxs-lookup"><span data-stu-id="c639f-118">Migrating to MSAL</span></span>

<span data-ttu-id="c639f-119">O MSAL oferece vários benefícios sobre o ADAL, incluindo consentimento incremental, experiências de logom único mais ricas, suporte para contas pessoais da Microsoft, uso de protocolos baseados em padrões e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="c639f-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="c639f-120">Ao alternar seu aplicativo para o MSAL, você precisará fazer algumas alterações, incluindo a definição do parâmetro **scopes** na solicitação de aquisição de token:</span><span class="sxs-lookup"><span data-stu-id="c639f-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquisition request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="c639f-121">A expressão acima limita a solicitação de escopos de permissão aos configurados durante o registro do aplicativo no Portal do Azure e salva seus usuários existentes de ter que consentir com seu aplicativo novamente.</span><span class="sxs-lookup"><span data-stu-id="c639f-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="c639f-122">Consulte [Migrando o ADAL para o MSAL](https://aka.ms/adal-net-to-msal-net) para ter ajuda direta e abrangente com o processo, incluindo solução de problemas e ajuda com erros comuns.</span><span class="sxs-lookup"><span data-stu-id="c639f-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="c639f-123">Depois de migrar para o MSAL, você pode solicitar escopos adicionais dinamicamente e os usuários são solicitados a fornecer consentimento incremental na próxima vez que usarem seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c639f-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c639f-124">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c639f-124">Next Steps</span></span>

- <span data-ttu-id="c639f-125">Saiba as diferenças de biblioteca do cliente [.NET](migrate-azure-ad-graph-client-libraries.md) entre o Azure AD Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c639f-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="c639f-126">Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.</span><span class="sxs-lookup"><span data-stu-id="c639f-126">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>