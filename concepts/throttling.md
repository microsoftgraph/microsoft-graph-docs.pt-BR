---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: piotrci
ms.openlocfilehash: d8f0c2098c76beaae65c5d84cc82e58949a0cebd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353211"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="7d777-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7d777-105">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="7d777-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7d777-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="7d777-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="7d777-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="7d777-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="7d777-111">What happens when throttling occurs?</span></span>

<span data-ttu-id="7d777-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7d777-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="7d777-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="7d777-119">Common throttling scenarios</span></span>

<span data-ttu-id="7d777-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="7d777-120">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="7d777-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="7d777-121">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="7d777-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="7d777-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="7d777-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="7d777-123">Best practices to handle throttling</span></span>

<span data-ttu-id="7d777-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="7d777-124">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="7d777-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d777-125">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="7d777-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="7d777-126">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="7d777-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="7d777-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="7d777-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo *Retry-After* no cabeçalho de resposta. Desativar solicitações usando o atraso *Retry-After* é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="7d777-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the *Retry-After* field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="7d777-131">Aguarde o número de segundos especificado no campo *Retry-After*.</span><span class="sxs-lookup"><span data-stu-id="7d777-131">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="7d777-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d777-132">Retry the request.</span></span>
3. <span data-ttu-id="7d777-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso Retry-After recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="7d777-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="7d777-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho retry-after:</span><span class="sxs-lookup"><span data-stu-id="7d777-135">The following resources currently provide a retry-after header:</span></span>
- [<span data-ttu-id="7d777-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="7d777-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-137">Foto</span><span class="sxs-lookup"><span data-stu-id="7d777-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-138">Email</span><span class="sxs-lookup"><span data-stu-id="7d777-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="7d777-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-140">Contato</span><span class="sxs-lookup"><span data-stu-id="7d777-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="7d777-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="7d777-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="7d777-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="7d777-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="7d777-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="7d777-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)

<span data-ttu-id="7d777-145">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://msdn.microsoft.com/library/office/dn589798.aspx).</span><span class="sxs-lookup"><span data-stu-id="7d777-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://msdn.microsoft.com/library/office/dn589798.aspx).</span></span>
