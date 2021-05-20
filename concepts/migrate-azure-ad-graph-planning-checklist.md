---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 84d486cd64d838a00998179a25dbba3ea35738eb
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546928"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="378f6-103">Lista de verificação de planejamento de migração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="378f6-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="378f6-104">A API do Azure AD Graph está preterida.</span><span class="sxs-lookup"><span data-stu-id="378f6-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="378f6-105">Continuaremos fornecendo suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.</span><span class="sxs-lookup"><span data-stu-id="378f6-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="378f6-106">A partir de 30 de junho de 2022, encerraremos o suporte ao Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="378f6-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="378f6-107">Os aplicativos que usam o Azure AD Graph depois desse tempo não receberão mais respostas do ponto de extremidade do Azure AD Graph ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="378f6-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="378f6-108">Use a lista de verificação a seguir para planejar sua migração.</span><span class="sxs-lookup"><span data-stu-id="378f6-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="378f6-109">Etapa 1: Analisar as diferenças entre as APIs</span><span class="sxs-lookup"><span data-stu-id="378f6-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="378f6-110">Em muitos aspectos, o microsoft Graph é semelhante ao Azure AD anterior Graph.</span><span class="sxs-lookup"><span data-stu-id="378f6-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="378f6-111">Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade em seu código e tudo deve continuar a funcionar.</span><span class="sxs-lookup"><span data-stu-id="378f6-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="378f6-112">No entanto, há diferenças.</span><span class="sxs-lookup"><span data-stu-id="378f6-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="378f6-113">Determinados recursos, propriedades, métodos e recursos principais foram alterados.</span><span class="sxs-lookup"><span data-stu-id="378f6-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="378f6-114">Especificamente, procure diferenças nas seguintes áreas:</span><span class="sxs-lookup"><span data-stu-id="378f6-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="378f6-115">[Solicitar sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) entre os dois serviços</span><span class="sxs-lookup"><span data-stu-id="378f6-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="378f6-116">[Diferenças de](migrate-azure-ad-graph-feature-differences.md)recursos , como extensões de diretório, lotes, consultas diferenciais e assim por diante</span><span class="sxs-lookup"><span data-stu-id="378f6-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="378f6-117">[Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos</span><span class="sxs-lookup"><span data-stu-id="378f6-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="378f6-118">[Propriedades](migrate-azure-ad-graph-property-differences.md) de objetos de solicitação e resposta</span><span class="sxs-lookup"><span data-stu-id="378f6-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="378f6-119">[Métodos](migrate-azure-ad-graph-method-differences.md), incluindo parâmetros e tipos</span><span class="sxs-lookup"><span data-stu-id="378f6-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="378f6-120">Etapa 2: Examinar o uso da API</span><span class="sxs-lookup"><span data-stu-id="378f6-120">Step 2: Examine API use</span></span>

<span data-ttu-id="378f6-121">[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas pelo seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.</span><span class="sxs-lookup"><span data-stu-id="378f6-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="378f6-122">Verifique se as APIs que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v1.0 e se essas APIs funcionam da mesma maneira.</span><span class="sxs-lookup"><span data-stu-id="378f6-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="378f6-123">Em alguns casos, novos recursos e recursos são projetados para substituir abordagens anteriores.</span><span class="sxs-lookup"><span data-stu-id="378f6-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="378f6-124">Use o [Graph Explorer para](https://aka.ms/ge) experimentar novas chamadas e desenvolver novas abordagens.</span><span class="sxs-lookup"><span data-stu-id="378f6-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="378f6-125">Para melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para que você veja o que a API faz em conjuntos de dados importantes.</span><span class="sxs-lookup"><span data-stu-id="378f6-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="378f6-126">Etapa 3: Revisar detalhes do aplicativo</span><span class="sxs-lookup"><span data-stu-id="378f6-126">Step 3: Review app details</span></span>

- <span data-ttu-id="378f6-127">[Alterações de registro e](migrate-azure-ad-graph-app-registration.md) consentimento do aplicativo (que não devem ser nenhuma).</span><span class="sxs-lookup"><span data-stu-id="378f6-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="378f6-128">Bibliotecas de autenticação e aquisição [de tokens.](migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="378f6-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="378f6-129">Para aplicativos .NET, use [bibliotecas de clientes.](migrate-azure-ad-graph-client-libraries.md)</span><span class="sxs-lookup"><span data-stu-id="378f6-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="378f6-130">Etapa 4: Implantar, testar e estender seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="378f6-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="378f6-131">Antes de atualizar seu aplicativo para todos, verifique se você testou completamente e estágiou sua lançamento para o público-alvo.</span><span class="sxs-lookup"><span data-stu-id="378f6-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="378f6-132">Agora que você alternou para o Microsoft Graph, nunca foi mais fácil desbloquear muitos mais conjuntos de dados e recursos que agora estão à sua ponta dos dedos.</span><span class="sxs-lookup"><span data-stu-id="378f6-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="378f6-133">Você pode obter uma amostra do que é possível analisando alguns dos principais serviços e recursos no [Microsoft Graph](./overview-major-services.md).</span><span class="sxs-lookup"><span data-stu-id="378f6-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="378f6-134">[A biblioteca de autenticação](/azure/active-directory/develop/reference-v2-libraries) da Microsoft (MSAL) agora é a biblioteca de autenticação recomendada para uso com a plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="378f6-134">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL) is now the recommended authentication library for use with the Microsoft identity platform.</span></span> <span data-ttu-id="378f6-135">Se você estiver usando a biblioteca de autenticação [do AD (ADAL),](/azure/active-directory/develop/active-directory-authentication-libraries) planeje alternar para MSAL.</span><span class="sxs-lookup"><span data-stu-id="378f6-135">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), plan to switch to MSAL.</span></span> <span data-ttu-id="378f6-136">Consulte mais orientações para migrar aplicativos para a Biblioteca de Autenticação [da Microsoft (MSAL).](/azure/active-directory/develop/msal-migration)</span><span class="sxs-lookup"><span data-stu-id="378f6-136">See further guidance to [migrate applications to the Microsoft Authentication Library (MSAL)](/azure/active-directory/develop/msal-migration).</span></span>

## <a name="next-steps"></a><span data-ttu-id="378f6-137">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="378f6-137">Next Steps</span></span>

- <span data-ttu-id="378f6-138">Saiba mais [sobre a sintaxe de chamada de](migrate-azure-ad-graph-request-differences.md) solicitação para iniciar a etapa 1: analisar as diferenças de API.</span><span class="sxs-lookup"><span data-stu-id="378f6-138">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>