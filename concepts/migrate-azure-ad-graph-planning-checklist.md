---
title: Lista de verificação de planejamento de migração de aplicativos
description: Lista de verificação para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 5470366e3b61cde18b52246483a46485f3f00c68
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288661"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="3f508-103">Lista de verificação de planejamento de migração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="3f508-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="3f508-104">A API do Azure AD Graph já foi preterida.</span><span class="sxs-lookup"><span data-stu-id="3f508-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="3f508-105">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas não fornecerá mais atualizações de recurso.</span><span class="sxs-lookup"><span data-stu-id="3f508-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="3f508-106">A partir de 30 de junho de 2022, encerraremos o suporte para o Azure AD Graph e não fornecerá mais suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="3f508-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="3f508-107">Os aplicativos que usam o Azure AD Graph após esse momento não receberão mais respostas do ponto de extremidade do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="3f508-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="3f508-108">Use a lista de verificação a seguir para planejar sua migração.</span><span class="sxs-lookup"><span data-stu-id="3f508-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="3f508-109">Etapa 1: revise as diferenças entre as APIs</span><span class="sxs-lookup"><span data-stu-id="3f508-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="3f508-110">Em muitos aspectos, o Microsoft Graph é semelhante ao gráfico do Azure AD anterior.</span><span class="sxs-lookup"><span data-stu-id="3f508-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="3f508-111">Em muitos casos, basta alterar o nome e a versão do serviço de ponto de extremidade no seu código, e tudo deve continuar a funcionar.</span><span class="sxs-lookup"><span data-stu-id="3f508-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="3f508-112">No entanto, há diferenças.</span><span class="sxs-lookup"><span data-stu-id="3f508-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="3f508-113">Determinados recursos, propriedades, métodos e recursos principais foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3f508-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="3f508-114">Especificamente, procure as diferenças nas seguintes áreas:</span><span class="sxs-lookup"><span data-stu-id="3f508-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="3f508-115">[Solicitar sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) entre os dois serviços</span><span class="sxs-lookup"><span data-stu-id="3f508-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="3f508-116">[Diferenças de recursos](migrate-azure-ad-graph-feature-differences.md), como extensões de diretório, processamento em lotes, consultas diferenciais e assim por diante</span><span class="sxs-lookup"><span data-stu-id="3f508-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="3f508-117">[Nomes de recursos de entidade](migrate-azure-ad-graph-resource-differences.md) e seus tipos</span><span class="sxs-lookup"><span data-stu-id="3f508-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="3f508-118">[Propriedades](migrate-azure-ad-graph-property-differences.md) de objetos de solicitação e resposta</span><span class="sxs-lookup"><span data-stu-id="3f508-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="3f508-119">[Métodos](migrate-azure-ad-graph-method-differences.md), incluindo parâmetros e tipos</span><span class="sxs-lookup"><span data-stu-id="3f508-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="3f508-120">Etapa 2: examinar o uso da API</span><span class="sxs-lookup"><span data-stu-id="3f508-120">Step 2: Examine API use</span></span>

<span data-ttu-id="3f508-121">[Examine as APIs](migrate-azure-ad-graph-audit-api-use.md) usadas por seu aplicativo, as permissões necessárias e compare com a lista de diferenças conhecidas.</span><span class="sxs-lookup"><span data-stu-id="3f508-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="3f508-122">Verifique se as APIs de que seu aplicativo precisa estão geralmente disponíveis no Microsoft Graph v 1.0 e se essas APIs funcionam da mesma maneira.</span><span class="sxs-lookup"><span data-stu-id="3f508-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="3f508-123">Em alguns casos, novos recursos e recursos foram projetados para substituir as abordagens anteriores.</span><span class="sxs-lookup"><span data-stu-id="3f508-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="3f508-124">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar novas chamadas e desenvolver novas abordagens.</span><span class="sxs-lookup"><span data-stu-id="3f508-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="3f508-125">Para obter melhores resultados, entre usando as credenciais de um usuário de teste em um locatário de teste para ver o que a API faz sobre conjuntos de dados importantes.</span><span class="sxs-lookup"><span data-stu-id="3f508-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="3f508-126">Etapa 3: examinar os detalhes do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f508-126">Step 3: Review app details</span></span>

- <span data-ttu-id="3f508-127">Alterações de consentimento e [registro de aplicativo](migrate-azure-ad-graph-app-registration.md) (que devem ser nenhuma).</span><span class="sxs-lookup"><span data-stu-id="3f508-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="3f508-128">Aquisição de token e [bibliotecas de autenticação](migrate-azure-ad-graph-authentication-library.md).</span><span class="sxs-lookup"><span data-stu-id="3f508-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="3f508-129">Para aplicativos .NET, use de [bibliotecas de cliente](migrate-azure-ad-graph-client-libraries.md).</span><span class="sxs-lookup"><span data-stu-id="3f508-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="3f508-130">Etapa 4: implantar, testar e estender seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f508-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="3f508-131">Antes de atualizar seu aplicativo para todos, assegure-se de testar cuidadosamente e preparar sua distribuição para o público do cliente.</span><span class="sxs-lookup"><span data-stu-id="3f508-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="3f508-132">Agora você já fez a migração para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de informações e recursos que agora estão em suas mãos.</span><span class="sxs-lookup"><span data-stu-id="3f508-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="3f508-133">Você pode ter uma idéia do que é possível examinando alguns [exemplos](/graph/examples).</span><span class="sxs-lookup"><span data-stu-id="3f508-133">You can get a taste of what's possible by looking at some [examples](/graph/examples).</span></span>

<span data-ttu-id="3f508-134">Se você estiver usando a [biblioteca de autenticação do AD](/azure/active-directory/develop/active-directory-authentication-libraries) (Adal), considere mudar para a biblioteca de autenticação da [Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="3f508-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="3f508-135">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3f508-135">Next Steps</span></span>

- <span data-ttu-id="3f508-136">Saiba mais sobre a [solicitação de sintaxe de chamada](migrate-azure-ad-graph-request-differences.md) para iniciar a etapa 1: revisando as diferenças da API.</span><span class="sxs-lookup"><span data-stu-id="3f508-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>