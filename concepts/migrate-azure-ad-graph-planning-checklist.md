---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: f8e231166fdb39676ce2778b369c6962cae70cb0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882742"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="73cd4-103">Lista de verificação de planejamento de migração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="73cd4-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="73cd4-104">A API do Azure AD Graph agora foi preterida.</span><span class="sxs-lookup"><span data-stu-id="73cd4-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="73cd4-105">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.</span><span class="sxs-lookup"><span data-stu-id="73cd4-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="73cd4-106">A partir de 30 de junho de 2022, encerraremos o suporte ao Azure AD Graph e não forneceremos mais suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="73cd4-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="73cd4-107">Os aplicativos que usam o Azure AD Graph após esse período não receberão mais respostas do ponto de extremidade do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="73cd4-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="73cd4-108">Use a lista de verificação a seguir para planejar sua migração.</span><span class="sxs-lookup"><span data-stu-id="73cd4-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="73cd4-109">Etapa 1: Revise as diferenças entre as APIs</span><span class="sxs-lookup"><span data-stu-id="73cd4-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="73cd4-110">Em muitos aspectos, o Microsoft Graph é semelhante ao Azure AD Graph anterior.</span><span class="sxs-lookup"><span data-stu-id="73cd4-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="73cd4-111">Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade em seu código, e tudo deve continuar a funcionar.</span><span class="sxs-lookup"><span data-stu-id="73cd4-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="73cd4-112">No entanto, há diferenças.</span><span class="sxs-lookup"><span data-stu-id="73cd4-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="73cd4-113">Determinados recursos, propriedades, métodos e recursos principais foram alterados.</span><span class="sxs-lookup"><span data-stu-id="73cd4-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="73cd4-114">Especificamente, procure diferenças nas seguintes áreas:</span><span class="sxs-lookup"><span data-stu-id="73cd4-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="73cd4-115">[Sintaxe de chamada de solicitação](migrate-azure-ad-graph-request-differences.md) entre os dois serviços</span><span class="sxs-lookup"><span data-stu-id="73cd4-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="73cd4-116">[Diferenças de](migrate-azure-ad-graph-feature-differences.md)recursos, como extensões de diretório, processamento em lotes, consultas diferenciais e assim por diante</span><span class="sxs-lookup"><span data-stu-id="73cd4-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="73cd4-117">[Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos</span><span class="sxs-lookup"><span data-stu-id="73cd4-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="73cd4-118">[Propriedades de](migrate-azure-ad-graph-property-differences.md) objetos de solicitação e resposta</span><span class="sxs-lookup"><span data-stu-id="73cd4-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="73cd4-119">[Métodos,](migrate-azure-ad-graph-method-differences.md)incluindo parâmetros e tipos</span><span class="sxs-lookup"><span data-stu-id="73cd4-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="73cd4-120">Etapa 2: Examinar o uso da API</span><span class="sxs-lookup"><span data-stu-id="73cd4-120">Step 2: Examine API use</span></span>

<span data-ttu-id="73cd4-121">[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas pelo seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.</span><span class="sxs-lookup"><span data-stu-id="73cd4-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="73cd4-122">Verifique se as APIs de que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v1.0 e se essas APIs funcionam da mesma maneira.</span><span class="sxs-lookup"><span data-stu-id="73cd4-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="73cd4-123">Em alguns casos, novos recursos são projetados para substituir abordagens anteriores.</span><span class="sxs-lookup"><span data-stu-id="73cd4-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="73cd4-124">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens.</span><span class="sxs-lookup"><span data-stu-id="73cd4-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="73cd4-125">Para melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para que você veja o que a API faz em conjuntos de dados importantes.</span><span class="sxs-lookup"><span data-stu-id="73cd4-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="73cd4-126">Etapa 3: Analisar detalhes do aplicativo</span><span class="sxs-lookup"><span data-stu-id="73cd4-126">Step 3: Review app details</span></span>

- <span data-ttu-id="73cd4-127">[Alterações de registro e](migrate-azure-ad-graph-app-registration.md) consentimento do aplicativo (que não devem ser nenhuma).</span><span class="sxs-lookup"><span data-stu-id="73cd4-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="73cd4-128">Bibliotecas de [aquisição e autenticação de tokens.](migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="73cd4-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="73cd4-129">Para aplicativos .NET, uso de [bibliotecas de cliente.](migrate-azure-ad-graph-client-libraries.md)</span><span class="sxs-lookup"><span data-stu-id="73cd4-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="73cd4-130">Etapa 4: Implantar, testar e estender seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="73cd4-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="73cd4-131">Antes de atualizar seu aplicativo para todos, teste exaustivamente e teste sua lançamento para o público-alvo.</span><span class="sxs-lookup"><span data-stu-id="73cd4-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="73cd4-132">Agora que você alternou para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de dados e recursos que agora estão ao seu alcance.</span><span class="sxs-lookup"><span data-stu-id="73cd4-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="73cd4-133">Você pode ter uma amostra do que é possível observando alguns dos principais serviços [e recursos do Microsoft Graph.](./overview-major-services.md)</span><span class="sxs-lookup"><span data-stu-id="73cd4-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="73cd4-134">Se você estiver usando a biblioteca de autenticação do [AD (ADAL),](/azure/active-directory/develop/active-directory-authentication-libraries) considere mudar para a biblioteca de autenticação da [Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="73cd4-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="73cd4-135">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="73cd4-135">Next Steps</span></span>

- <span data-ttu-id="73cd4-136">Saiba mais sobre [a sintaxe de chamada de](migrate-azure-ad-graph-request-differences.md) solicitação para iniciar a etapa 1: analisar as diferenças da API.</span><span class="sxs-lookup"><span data-stu-id="73cd4-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>