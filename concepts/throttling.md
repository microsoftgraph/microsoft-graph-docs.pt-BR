---
title: Diretrizes de limitação do Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8cf528675b0cdde108063f3fd44acdfdff418941
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038531"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="bbc47-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bbc47-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="bbc47-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="bbc47-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="bbc47-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="bbc47-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="bbc47-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="bbc47-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="bbc47-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="bbc47-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="bbc47-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="bbc47-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="bbc47-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="bbc47-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="bbc47-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="bbc47-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="bbc47-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="bbc47-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="bbc47-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="bbc47-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="bbc47-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="bbc47-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="bbc47-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="bbc47-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="bbc47-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="bbc47-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="bbc47-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="bbc47-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="bbc47-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="bbc47-119">Common throttling scenarios</span></span>

<span data-ttu-id="bbc47-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="bbc47-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="bbc47-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="bbc47-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="bbc47-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="bbc47-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="bbc47-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="bbc47-123">Best practices to handle throttling</span></span>

<span data-ttu-id="bbc47-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="bbc47-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="bbc47-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbc47-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="bbc47-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="bbc47-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="bbc47-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="bbc47-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="bbc47-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="bbc47-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="bbc47-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="bbc47-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="bbc47-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="bbc47-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="bbc47-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="bbc47-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="bbc47-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbc47-132">Retry the request.</span></span>
3. <span data-ttu-id="bbc47-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="bbc47-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="bbc47-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="bbc47-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="bbc47-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="bbc47-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="bbc47-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="bbc47-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-137">Foto</span><span class="sxs-lookup"><span data-stu-id="bbc47-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-138">Email</span><span class="sxs-lookup"><span data-stu-id="bbc47-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="bbc47-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-140">Contato</span><span class="sxs-lookup"><span data-stu-id="bbc47-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="bbc47-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="bbc47-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="bbc47-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="bbc47-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="bbc47-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="bbc47-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbc47-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="bbc47-146">Report</span><span class="sxs-lookup"><span data-stu-id="bbc47-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="bbc47-147">Assinatura</span><span class="sxs-lookup"><span data-stu-id="bbc47-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="bbc47-148">Mais Populares</span><span class="sxs-lookup"><span data-stu-id="bbc47-148">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="bbc47-149">Informações usadas</span><span class="sxs-lookup"><span data-stu-id="bbc47-149">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="bbc47-150">Informações compartilhadas</span><span class="sxs-lookup"><span data-stu-id="bbc47-150">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="bbc47-151">Configurações do usuário</span><span class="sxs-lookup"><span data-stu-id="bbc47-151">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="bbc47-152">Convite</span><span class="sxs-lookup"><span data-stu-id="bbc47-152">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="bbc47-153">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="bbc47-153">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="bbc47-154">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="bbc47-154">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="bbc47-155">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="bbc47-155">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="bbc47-156">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="bbc47-156">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="bbc47-157">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="bbc47-157">Best practices to avoid throttling</span></span>

<span data-ttu-id="bbc47-158">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="bbc47-158">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="bbc47-159">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="bbc47-159">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="bbc47-160">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="bbc47-160">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="bbc47-161">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="bbc47-161">Service-specific limits</span></span>

<span data-ttu-id="bbc47-162">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bbc47-162">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="bbc47-163">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="bbc47-163">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="bbc47-164">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bbc47-164">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="bbc47-165">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="bbc47-165">Outlook service limits</span></span>

<span data-ttu-id="bbc47-166">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="bbc47-166">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="bbc47-167">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="bbc47-167">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="bbc47-168">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="bbc47-168">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="bbc47-169">Os limites a seguir se aplicam à nuvem pública, bem como às [implantações nacionais da nuvem](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="bbc47-169">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="bbc47-170">Limite</span><span class="sxs-lookup"><span data-stu-id="bbc47-170">Limit</span></span>                                                      | <span data-ttu-id="bbc47-171">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="bbc47-171">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="bbc47-172">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="bbc47-172">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="bbc47-173">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="bbc47-173">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="bbc47-174">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="bbc47-174">4 concurrent requests</span></span>                                      | <span data-ttu-id="bbc47-175">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="bbc47-175">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="bbc47-176">15 megabytes (MB) upload (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="bbc47-176">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="bbc47-177">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="bbc47-177">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="bbc47-178">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="bbc47-178">Outlook service resources</span></span>

<span data-ttu-id="bbc47-179">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="bbc47-179">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="bbc47-180">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="bbc47-180">Calendar API resources</span></span>

- [<span data-ttu-id="bbc47-181">event</span><span class="sxs-lookup"><span data-stu-id="bbc47-181">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="bbc47-182">eventMessage</span><span class="sxs-lookup"><span data-stu-id="bbc47-182">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="bbc47-183">calendar</span><span class="sxs-lookup"><span data-stu-id="bbc47-183">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="bbc47-184">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="bbc47-184">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="bbc47-185">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bbc47-185">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="bbc47-186">attachment</span><span class="sxs-lookup"><span data-stu-id="bbc47-186">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="bbc47-187">place (preview)</span><span class="sxs-lookup"><span data-stu-id="bbc47-187">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="bbc47-188">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="bbc47-188">Mail API resources</span></span>

- [<span data-ttu-id="bbc47-189">message</span><span class="sxs-lookup"><span data-stu-id="bbc47-189">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="bbc47-190">mailFolder</span><span class="sxs-lookup"><span data-stu-id="bbc47-190">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="bbc47-191">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="bbc47-191">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="bbc47-192">messageRule</span><span class="sxs-lookup"><span data-stu-id="bbc47-192">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="bbc47-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bbc47-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="bbc47-194">attachment</span><span class="sxs-lookup"><span data-stu-id="bbc47-194">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="bbc47-195">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="bbc47-195">Personal contacts API resources</span></span>

- [<span data-ttu-id="bbc47-196">contato</span><span class="sxs-lookup"><span data-stu-id="bbc47-196">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="bbc47-197">contactFolder</span><span class="sxs-lookup"><span data-stu-id="bbc47-197">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="bbc47-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bbc47-198">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="bbc47-199">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="bbc47-199">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="bbc47-200">person</span><span class="sxs-lookup"><span data-stu-id="bbc47-200">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="bbc47-201">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="bbc47-201">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="bbc47-202">outlookTask</span><span class="sxs-lookup"><span data-stu-id="bbc47-202">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="bbc47-203">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="bbc47-203">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="bbc47-204">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="bbc47-204">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="bbc47-205">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bbc47-205">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="bbc47-206">attachment</span><span class="sxs-lookup"><span data-stu-id="bbc47-206">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="bbc47-207">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="bbc47-207">Microsoft Teams service limits</span></span>

<span data-ttu-id="bbc47-208">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="bbc47-208">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="bbc47-209">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="bbc47-209">Teams request type</span></span>                                   | <span data-ttu-id="bbc47-210">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="bbc47-210">Limit per app per tenant</span></span>        | <span data-ttu-id="bbc47-211">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="bbc47-211">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="bbc47-212">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="bbc47-212">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="bbc47-213">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="bbc47-213">15000 requests every 10 seconds</span></span> | <span data-ttu-id="bbc47-214">n/d</span><span class="sxs-lookup"><span data-stu-id="bbc47-214">n/a</span></span> |
| <span data-ttu-id="bbc47-215">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="bbc47-215">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="bbc47-216">60 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-216">60 rps</span></span>                          | <span data-ttu-id="bbc47-217">600 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-217">600 rps</span></span> |
| <span data-ttu-id="bbc47-218">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="bbc47-218">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="bbc47-219">30 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-219">30 rps</span></span>                         | <span data-ttu-id="bbc47-220">300 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-220">300 rps</span></span>  |
| <span data-ttu-id="bbc47-221">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="bbc47-221">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="bbc47-222">30 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-222">30 rps</span></span>                         | <span data-ttu-id="bbc47-223">300 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-223">300 rps</span></span>  |
| <span data-ttu-id="bbc47-224">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="bbc47-224">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="bbc47-225">15 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-225">15 rps</span></span>                         | <span data-ttu-id="bbc47-226">150 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-226">150 rps</span></span>  |
| <span data-ttu-id="bbc47-227">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="bbc47-227">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="bbc47-228">30 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-228">30 rps</span></span>                         | <span data-ttu-id="bbc47-229">300 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-229">300 rps</span></span>  |
| <span data-ttu-id="bbc47-230">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="bbc47-230">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="bbc47-231">6 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-231">6 rps</span></span> | <span data-ttu-id="bbc47-232">150 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-232">150 rps</span></span>  | 
| <span data-ttu-id="bbc47-233">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="bbc47-233">GET channel message</span></span>  | <span data-ttu-id="bbc47-234">5 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-234">5 rps</span></span> | <span data-ttu-id="bbc47-235">100 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-235">100 rps</span></span> |
| <span data-ttu-id="bbc47-236">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="bbc47-236">GET 1:1/group chat message</span></span>  | <span data-ttu-id="bbc47-237">3 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-237">3 rps</span></span> | <span data-ttu-id="bbc47-238">30 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-238">30 rps</span></span> |
| <span data-ttu-id="bbc47-239">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="bbc47-239">POST channel message</span></span> | <span data-ttu-id="bbc47-240">2 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-240">2 rps</span></span> | <span data-ttu-id="bbc47-241">20 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-241">20 rps</span></span> |
| <span data-ttu-id="bbc47-242">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="bbc47-242">POST 1:1/group chat message</span></span> | <span data-ttu-id="bbc47-243">2 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-243">2 rps</span></span> | <span data-ttu-id="bbc47-244">20 rps</span><span class="sxs-lookup"><span data-stu-id="bbc47-244">20 rps</span></span> |

<span data-ttu-id="bbc47-245">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="bbc47-245">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="bbc47-246">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="bbc47-246">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="bbc47-247">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="bbc47-247">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="bbc47-248">Limites de serviço do insights</span><span class="sxs-lookup"><span data-stu-id="bbc47-248">Insights service limits</span></span>

<span data-ttu-id="bbc47-249">Os seguintes limites se aplicam a qualquer solicitação no `me/insights` ou no `users/{id}/insights` .</span><span class="sxs-lookup"><span data-stu-id="bbc47-249">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="bbc47-250">Limite</span><span class="sxs-lookup"><span data-stu-id="bbc47-250">Limit</span></span>                                                      | <span data-ttu-id="bbc47-251">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="bbc47-251">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="bbc47-252">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="bbc47-252">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="bbc47-253">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="bbc47-253">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="bbc47-254">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="bbc47-254">4 concurrent requests</span></span>                                      | <span data-ttu-id="bbc47-255">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="bbc47-255">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="bbc47-256">Limites do serviço de relatórios do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bbc47-256">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="bbc47-257">Os seguintes limites se aplicam a qualquer solicitação no `/reports`.</span><span class="sxs-lookup"><span data-stu-id="bbc47-257">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="bbc47-258">Operation</span><span class="sxs-lookup"><span data-stu-id="bbc47-258">Operation</span></span>                 | <span data-ttu-id="bbc47-259">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="bbc47-259">Limit per app per tenant</span></span>     | <span data-ttu-id="bbc47-260">Limite por locatário</span><span class="sxs-lookup"><span data-stu-id="bbc47-260">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="bbc47-261">Qualquer solicitação (CSV)</span><span class="sxs-lookup"><span data-stu-id="bbc47-261">Any request (CSV)</span></span>         | <span data-ttu-id="bbc47-262">14 solicitações por 10 minutos</span><span class="sxs-lookup"><span data-stu-id="bbc47-262">14 requests per 10 minutes</span></span>   | <span data-ttu-id="bbc47-263">40 solicitações por 10 minutos</span><span class="sxs-lookup"><span data-stu-id="bbc47-263">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="bbc47-264">Qualquer solicitação (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="bbc47-264">Any request (JSON, beta)</span></span>  | <span data-ttu-id="bbc47-265">100 solicitações por 10 minutos</span><span class="sxs-lookup"><span data-stu-id="bbc47-265">100 requests per 10 minutes</span></span>  | <span data-ttu-id="bbc47-266">n/d</span><span class="sxs-lookup"><span data-stu-id="bbc47-266">n/a</span></span>                        |

<span data-ttu-id="bbc47-267">Os limites anteriores se aplicam individualmente a cada API de relatório.</span><span class="sxs-lookup"><span data-stu-id="bbc47-267">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="bbc47-268">Por exemplo, uma solicitação para a API do relatório de atividades do usuário do Microsoft Teams e uma solicitação para a API do relatório de atividades do usuário do Outlook em 10 minutos contarão como 1 solicitação de 14 para cada API, não 2 solicitações de 14 para ambos.</span><span class="sxs-lookup"><span data-stu-id="bbc47-268">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="bbc47-269">Limites do serviço Gerenciador de convites</span><span class="sxs-lookup"><span data-stu-id="bbc47-269">Invitation manager service limits</span></span>

<span data-ttu-id="bbc47-270">Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="bbc47-270">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="bbc47-271">Operation</span><span class="sxs-lookup"><span data-stu-id="bbc47-271">Operation</span></span>                 | <span data-ttu-id="bbc47-272">Limite por locatário</span><span class="sxs-lookup"><span data-stu-id="bbc47-272">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="bbc47-273">Qualquer operação</span><span class="sxs-lookup"><span data-stu-id="bbc47-273">Any operation</span></span>             | <span data-ttu-id="bbc47-274">150 solicitações por 5 segundos</span><span class="sxs-lookup"><span data-stu-id="bbc47-274">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a><span data-ttu-id="bbc47-275">Limites do serviço de educação</span><span class="sxs-lookup"><span data-stu-id="bbc47-275">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="bbc47-276">Limites do serviço do Excel</span><span class="sxs-lookup"><span data-stu-id="bbc47-276">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="bbc47-277">Limites de serviço de logs de auditoria de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="bbc47-277">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="bbc47-278">Limites de serviço de provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="bbc47-278">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="bbc47-279">Limites de serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="bbc47-279">Intune service limits</span></span>

[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="skype-service-limits"></a><span data-ttu-id="bbc47-280">Limites do serviço Skype</span><span class="sxs-lookup"><span data-stu-id="bbc47-280">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="bbc47-281">Limites do serviço de assinatura</span><span class="sxs-lookup"><span data-stu-id="bbc47-281">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
