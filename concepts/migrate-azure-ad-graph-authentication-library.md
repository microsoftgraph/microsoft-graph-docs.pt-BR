---
title: Analisar alterações da biblioteca de autenticação do aplicativo
description: Descreve como atualizar o uso da biblioteca de autenticação para migrar um aplicativo dos aplicativos de API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77604945064565f1387553b22a26a0fa871c998d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630262"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="83af7-103">Analisar alterações da biblioteca de autenticação do aplicativo</span><span class="sxs-lookup"><span data-stu-id="83af7-103">Review app authentication library changes</span></span>

<span data-ttu-id="83af7-104">Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="83af7-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="83af7-105">A maioria dos aplicativos usa uma biblioteca de autenticação para aquire e gerenciar tokens de acesso para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="83af7-105">Most apps use an authentication library to aquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="83af7-106">A Microsoft oferece duas bibliotecas de autenticação:</span><span class="sxs-lookup"><span data-stu-id="83af7-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="83af7-107">[Biblioteca de autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) Adal</span><span class="sxs-lookup"><span data-stu-id="83af7-107">[Azure Active Directory authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="83af7-108">[Biblioteca de autenticação da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) MSAL</span><span class="sxs-lookup"><span data-stu-id="83af7-108">[Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="83af7-109">Atualizando ADAL</span><span class="sxs-lookup"><span data-stu-id="83af7-109">Updating ADAL</span></span>

<span data-ttu-id="83af7-110">Se seu aplicativo usa atualmente a ADAL, use uma abordagem de migração de dois estágios:</span><span class="sxs-lookup"><span data-stu-id="83af7-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="83af7-111">Atualize seu aplicativo para adquirir tokens de acesso para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="83af7-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="83af7-112">Continue a usar a ADAL para esta etapa.</span><span class="sxs-lookup"><span data-stu-id="83af7-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="83af7-113">Atualize o **resourceurl pela**, que contém o URI que representa a API Web de recurso, de:</span><span class="sxs-lookup"><span data-stu-id="83af7-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="83af7-114">Para:</span><span class="sxs-lookup"><span data-stu-id="83af7-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="83af7-115">Tokens adquiridos recentemente têm os mesmos escopos após essa alteração, mas a audiência dos tokens de acesso agora é o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="83af7-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="83af7-116">Após a atualização do **resourceurl pela** e verificação da funcionalidade, libere uma atualização provisória para que seus usuários sejam ativados e runnning.</span><span class="sxs-lookup"><span data-stu-id="83af7-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="83af7-117">Em seguida, comece a migrar o aplicativo para usar o MSAL, que é a biblioteca com suporte para usar a movimentação para frente.</span><span class="sxs-lookup"><span data-stu-id="83af7-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="83af7-118">Migrando para o MSAL</span><span class="sxs-lookup"><span data-stu-id="83af7-118">Migrating to MSAL</span></span>

<span data-ttu-id="83af7-119">O MSAL fornece vários benefícios sobre a ADAL, incluindo o consentimento incremental, experiências de logon único mais ricas, suporte para contas pessoais da Microsoft, uso de protocolos baseados em padrões e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="83af7-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="83af7-120">Ao mudar seu aplicativo para o MSAL, você precisará fazer algumas alterações, incluindo a configuração do parâmetro de \*\*\*\* escopos na solicitação de token Acquistion:</span><span class="sxs-lookup"><span data-stu-id="83af7-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquistion request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="83af7-121">A expressão acima limita a solicitação de escopos de permissão para aquelas configuradas durante o registro do aplicativo no portal do Azure e salva seus usuários existentes para que eles tenham de ser consentidos em seu aplicativo novamente.</span><span class="sxs-lookup"><span data-stu-id="83af7-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="83af7-122">Consulte [migraNDO Adal para MSAL](https://aka.ms/adal-net-to-msal-net) para obter ajuda direta e abrangente com o processo, incluindo solução de problemas e ajuda com erros comuns.</span><span class="sxs-lookup"><span data-stu-id="83af7-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="83af7-123">Após a migração para o MSAL, você poderá solicitar escopos adicionais dinamicamente e os usuários serão solicitados a fornecer o consentimento incremental na próxima vez que usarem seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="83af7-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="83af7-124">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="83af7-124">Next Steps</span></span>

- <span data-ttu-id="83af7-125">Saiba mais sobre as diferenças de [biblioteca de cliente .net](migrate-azure-ad-graph-client-libraries.md) entre o Azure AD e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="83af7-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="83af7-126">Explore a [migração de Adal para o MSAL](https://aka.ms/adal-net-to-msal-net) para obter ajuda mais detalhada sobre a migração para o MSAL.</span><span class="sxs-lookup"><span data-stu-id="83af7-126">Explore [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for more in-depth help on migrating to MSAL.</span></span>
- <span data-ttu-id="83af7-127">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="83af7-127">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="83af7-128">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="83af7-128">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
