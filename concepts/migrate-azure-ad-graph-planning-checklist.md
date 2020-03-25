---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59114221b91f6dc1800f9f1601cb2e2c06709ff8
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926782"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="4c488-103">Lista de verificação de planejamento de migração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="4c488-103">App migration planning checklist</span></span>

<span data-ttu-id="4c488-104">Use a lista de verificação a seguir para planejar a migração:</span><span class="sxs-lookup"><span data-stu-id="4c488-104">Use the following checklist to plan your migration:</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="4c488-105">Etapa 1: revise as diferenças entre as APIs</span><span class="sxs-lookup"><span data-stu-id="4c488-105">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="4c488-106">Em muitos aspectos, o Microsoft Graph é semelhante ao gráfico do Azure AD anterior.</span><span class="sxs-lookup"><span data-stu-id="4c488-106">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="4c488-107">Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade no seu código, e tudo deve continuar a funcionar.</span><span class="sxs-lookup"><span data-stu-id="4c488-107">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="4c488-108">No entanto, há diferenças.</span><span class="sxs-lookup"><span data-stu-id="4c488-108">Nonetheless, there are differences.</span></span> <span data-ttu-id="4c488-109">Determinados recursos, propriedades, métodos e recursos principais foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4c488-109">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="4c488-110">Especificamente, procure as diferenças nas seguintes áreas:</span><span class="sxs-lookup"><span data-stu-id="4c488-110">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="4c488-111">[Solicitar sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) entre os dois serviços</span><span class="sxs-lookup"><span data-stu-id="4c488-111">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="4c488-112">[Diferenças de recursos](migrate-azure-ad-graph-feature-differences.md), como extensões de diretório, processamento em lotes, consultas diferenciais e assim por diante</span><span class="sxs-lookup"><span data-stu-id="4c488-112">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="4c488-113">[Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos</span><span class="sxs-lookup"><span data-stu-id="4c488-113">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="4c488-114">[Propriedades](migrate-azure-ad-graph-property-differences.md) de objetos de solicitação e resposta</span><span class="sxs-lookup"><span data-stu-id="4c488-114">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="4c488-115">[Métodos](migrate-azure-ad-graph-method-differences.md), incluindo parâmetros e tipos</span><span class="sxs-lookup"><span data-stu-id="4c488-115">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="4c488-116">Etapa 2: examinar o uso da API</span><span class="sxs-lookup"><span data-stu-id="4c488-116">Step 2: Examine API use</span></span>

<span data-ttu-id="4c488-117">[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas por seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.</span><span class="sxs-lookup"><span data-stu-id="4c488-117">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="4c488-118">Verifique se as APIs de que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v 1.0 e se essas APIs funcionam da mesma maneira.</span><span class="sxs-lookup"><span data-stu-id="4c488-118">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="4c488-119">Em alguns casos, novos recursos e recursos foram projetados para substituir as abordagens anteriores.</span><span class="sxs-lookup"><span data-stu-id="4c488-119">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="4c488-120">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens.</span><span class="sxs-lookup"><span data-stu-id="4c488-120">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="4c488-121">Para obter melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para ver o que a API faz sobre conjuntos de dados importantes.</span><span class="sxs-lookup"><span data-stu-id="4c488-121">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="4c488-122">Etapa 3: examinar os detalhes do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c488-122">Step 3: Review app details</span></span>

- <span data-ttu-id="4c488-123">Alterações de consentimento e [registro de aplicativo](migrate-azure-ad-graph-app-registration.md) (que devem ser nenhuma).</span><span class="sxs-lookup"><span data-stu-id="4c488-123">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="4c488-124">Aquisição de token e [bibliotecas de autenticação](migrate-azure-ad-graph-authentication-library.md).</span><span class="sxs-lookup"><span data-stu-id="4c488-124">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="4c488-125">Para aplicativos .NET, use de [bibliotecas de cliente](migrate-azure-ad-graph-client-libraries.md).</span><span class="sxs-lookup"><span data-stu-id="4c488-125">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="4c488-126">Etapa 4: implantar, testar e estender seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c488-126">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="4c488-127">Antes de atualizar seu aplicativo para todos, assegure-se de testar cuidadosamente e preparar sua distribuição para o público do cliente.</span><span class="sxs-lookup"><span data-stu-id="4c488-127">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="4c488-128">Agora você já fez a migração para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de informações e recursos que agora estão em suas mãos.</span><span class="sxs-lookup"><span data-stu-id="4c488-128">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="4c488-129">Você pode ter uma idéia do que é possível examinando alguns [exemplos](/graph/examples).</span><span class="sxs-lookup"><span data-stu-id="4c488-129">You can get a taste of what's possible by looking at some [examples](/graph/examples).</span></span>

<span data-ttu-id="4c488-130">Se você estiver usando a [biblioteca de autenticação do AD](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (Adal), considere mudar para a biblioteca de autenticação da [Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="4c488-130">If you're currently using the [AD authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="4c488-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4c488-131">Next Steps</span></span>

- <span data-ttu-id="4c488-132">Saiba mais sobre a [sintaxe de chamada resquest](migrate-azure-ad-graph-request-differences.md) para iniciar a etapa 1: revisando as diferenças da API.</span><span class="sxs-lookup"><span data-stu-id="4c488-132">Learn about [resquest call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>
- <span data-ttu-id="4c488-133">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="4c488-133">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="4c488-134">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4c488-134">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="4c488-135">Para saber mais sobre atualizações de progresso e cronogramas, confira [Microsoft Graph ou o Azure ad Graph](https://developer.microsoft.com/en-us/graph/blogs/microsoft-graph-or-azure-ad-graph/).</span><span class="sxs-lookup"><span data-stu-id="4c488-135">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://developer.microsoft.com/en-us/graph/blogs/microsoft-graph-or-azure-ad-graph/).</span></span>
