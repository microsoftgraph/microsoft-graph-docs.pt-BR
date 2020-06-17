---
title: Diretrizes de limitação do Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: f2acb34994f0877a051d31e276feb22b2d47179c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682037"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="2e7c4-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7c4-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="2e7c4-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="2e7c4-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="2e7c4-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="2e7c4-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="2e7c4-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="2e7c4-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="2e7c4-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="2e7c4-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="2e7c4-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="2e7c4-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="2e7c4-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="2e7c4-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="2e7c4-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="2e7c4-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="2e7c4-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="2e7c4-119">Common throttling scenarios</span></span>

<span data-ttu-id="2e7c4-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="2e7c4-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="2e7c4-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="2e7c4-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="2e7c4-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="2e7c4-123">Best practices to handle throttling</span></span>

<span data-ttu-id="2e7c4-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="2e7c4-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="2e7c4-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="2e7c4-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="2e7c4-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="2e7c4-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="2e7c4-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="2e7c4-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="2e7c4-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="2e7c4-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-132">Retry the request.</span></span>
3. <span data-ttu-id="2e7c4-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="2e7c4-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="2e7c4-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="2e7c4-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="2e7c4-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="2e7c4-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-137">Foto</span><span class="sxs-lookup"><span data-stu-id="2e7c4-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-138">Email</span><span class="sxs-lookup"><span data-stu-id="2e7c4-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="2e7c4-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-140">Contato</span><span class="sxs-lookup"><span data-stu-id="2e7c4-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="2e7c4-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="2e7c4-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="2e7c4-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="2e7c4-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="2e7c4-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="2e7c4-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e7c4-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="2e7c4-146">Assinatura</span><span class="sxs-lookup"><span data-stu-id="2e7c4-146">Subscription</span></span>](/graph/api/resources/subscription)

<span data-ttu-id="2e7c4-147">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="2e7c4-147">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="2e7c4-148">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-148">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="2e7c4-149">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-149">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="2e7c4-150">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-150">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="2e7c4-151">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="2e7c4-151">Best practices to avoid throttling</span></span>

<span data-ttu-id="2e7c4-152">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-152">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="2e7c4-153">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-153">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="2e7c4-154">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-154">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="2e7c4-155">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="2e7c4-155">Service-specific limits</span></span>

<span data-ttu-id="2e7c4-156">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-156">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="2e7c4-157">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-157">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="2e7c4-158">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-158">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="2e7c4-159">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="2e7c4-159">Outlook service limits</span></span>

<span data-ttu-id="2e7c4-160">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-160">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="2e7c4-161">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="2e7c4-161">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="2e7c4-162">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-162">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="2e7c4-163">Limite</span><span class="sxs-lookup"><span data-stu-id="2e7c4-163">Limit</span></span>                                                      | <span data-ttu-id="2e7c4-164">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="2e7c4-164">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="2e7c4-165">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-165">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="2e7c4-166">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="2e7c4-166">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="2e7c4-167">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="2e7c4-167">4 concurrent requests</span></span>                                      | <span data-ttu-id="2e7c4-168">Ponto de extremidade Beta</span><span class="sxs-lookup"><span data-stu-id="2e7c4-168">Beta endpoint</span></span>   |
| <span data-ttu-id="2e7c4-169">carregamento de 15 megabits (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-169">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="2e7c4-170">Ponto de extremidade Beta</span><span class="sxs-lookup"><span data-stu-id="2e7c4-170">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="2e7c4-171">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="2e7c4-171">Outlook service resources</span></span>

<span data-ttu-id="2e7c4-172">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-172">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="2e7c4-173">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="2e7c4-173">Calendar API resources</span></span>

- [<span data-ttu-id="2e7c4-174">event</span><span class="sxs-lookup"><span data-stu-id="2e7c4-174">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="2e7c4-175">eventMessage</span><span class="sxs-lookup"><span data-stu-id="2e7c4-175">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="2e7c4-176">calendar</span><span class="sxs-lookup"><span data-stu-id="2e7c4-176">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="2e7c4-177">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2e7c4-177">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="2e7c4-178">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="2e7c4-178">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="2e7c4-179">attachment</span><span class="sxs-lookup"><span data-stu-id="2e7c4-179">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="2e7c4-180">place (preview)</span><span class="sxs-lookup"><span data-stu-id="2e7c4-180">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="2e7c4-181">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="2e7c4-181">Mail API resources</span></span>

- [<span data-ttu-id="2e7c4-182">message</span><span class="sxs-lookup"><span data-stu-id="2e7c4-182">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="2e7c4-183">mailFolder</span><span class="sxs-lookup"><span data-stu-id="2e7c4-183">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="2e7c4-184">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="2e7c4-184">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="2e7c4-185">messageRule</span><span class="sxs-lookup"><span data-stu-id="2e7c4-185">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="2e7c4-186">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="2e7c4-186">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="2e7c4-187">attachment</span><span class="sxs-lookup"><span data-stu-id="2e7c4-187">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="2e7c4-188">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="2e7c4-188">Personal contacts API resources</span></span>

- [<span data-ttu-id="2e7c4-189">contato</span><span class="sxs-lookup"><span data-stu-id="2e7c4-189">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="2e7c4-190">contactFolder</span><span class="sxs-lookup"><span data-stu-id="2e7c4-190">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="2e7c4-191">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="2e7c4-191">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="2e7c4-192">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="2e7c4-192">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="2e7c4-193">person</span><span class="sxs-lookup"><span data-stu-id="2e7c4-193">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="2e7c4-194">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="2e7c4-194">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="2e7c4-195">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2e7c4-195">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="2e7c4-196">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="2e7c4-196">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="2e7c4-197">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="2e7c4-197">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="2e7c4-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="2e7c4-198">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="2e7c4-199">attachment</span><span class="sxs-lookup"><span data-stu-id="2e7c4-199">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="2e7c4-200">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2e7c4-200">Microsoft Teams service limits</span></span>

<span data-ttu-id="2e7c4-201">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="2e7c4-201">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="2e7c4-202">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="2e7c4-202">Teams request type</span></span>                                   | <span data-ttu-id="2e7c4-203">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="2e7c4-203">Limit per app per tenant</span></span>        | <span data-ttu-id="2e7c4-204">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="2e7c4-204">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="2e7c4-205">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2e7c4-205">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="2e7c4-206">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-206">15000 requests every 10 seconds</span></span> | <span data-ttu-id="2e7c4-207">n/d</span><span class="sxs-lookup"><span data-stu-id="2e7c4-207">n/a</span></span> |
| <span data-ttu-id="2e7c4-208">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="2e7c4-208">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="2e7c4-209">60 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-209">60 rps</span></span>                          | <span data-ttu-id="2e7c4-210">600 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-210">600 rps</span></span> |
| <span data-ttu-id="2e7c4-211">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="2e7c4-211">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="2e7c4-212">30 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-212">30 rps</span></span>                         | <span data-ttu-id="2e7c4-213">300 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-213">300 rps</span></span>  |
| <span data-ttu-id="2e7c4-214">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="2e7c4-214">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="2e7c4-215">30 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-215">30 rps</span></span>                         | <span data-ttu-id="2e7c4-216">300 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-216">300 rps</span></span>  |
| <span data-ttu-id="2e7c4-217">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="2e7c4-217">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="2e7c4-218">15 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-218">15 rps</span></span>                         | <span data-ttu-id="2e7c4-219">150 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-219">150 rps</span></span>  |
| <span data-ttu-id="2e7c4-220">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="2e7c4-220">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="2e7c4-221">30 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-221">30 rps</span></span>                         | <span data-ttu-id="2e7c4-222">300 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-222">300 rps</span></span>  |
| <span data-ttu-id="2e7c4-223">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="2e7c4-223">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="2e7c4-224">6 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-224">6 rps</span></span> | <span data-ttu-id="2e7c4-225">150 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-225">150 rps</span></span>  | 
| <span data-ttu-id="2e7c4-226">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="2e7c4-226">GET channel message</span></span>  | <span data-ttu-id="2e7c4-227">5 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-227">5 rps</span></span> | <span data-ttu-id="2e7c4-228">100 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-228">100 rps</span></span> |
| <span data-ttu-id="2e7c4-229">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="2e7c4-229">GET 1:1/group chat message</span></span>  | <span data-ttu-id="2e7c4-230">3 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-230">3 rps</span></span> | <span data-ttu-id="2e7c4-231">30 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-231">30 rps</span></span> |
| <span data-ttu-id="2e7c4-232">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="2e7c4-232">POST channel message</span></span> | <span data-ttu-id="2e7c4-233">2 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-233">2 rps</span></span> | <span data-ttu-id="2e7c4-234">20 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-234">20 rps</span></span> |
| <span data-ttu-id="2e7c4-235">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="2e7c4-235">POST 1:1/group chat message</span></span> | <span data-ttu-id="2e7c4-236">2 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-236">2 rps</span></span> | <span data-ttu-id="2e7c4-237">20 rps</span><span class="sxs-lookup"><span data-stu-id="2e7c4-237">20 rps</span></span> |

<span data-ttu-id="2e7c4-238">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-238">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="2e7c4-239">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-239">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="2e7c4-240">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="2e7c4-240">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="microsoft-graph-change-notifications-subscription-operations"></a><span data-ttu-id="2e7c4-241">Operações de notificações de mudança de assinatura do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e7c4-241">Microsoft Graph change notifications subscription operations</span></span>

<span data-ttu-id="2e7c4-242">Os seguintes limites se aplicam a qualquer solicitação no `/subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="2e7c4-242">The following limits apply to any request on `/subscriptions`.</span></span>

| <span data-ttu-id="2e7c4-243">Operation</span><span class="sxs-lookup"><span data-stu-id="2e7c4-243">Operation</span></span>                 | <span data-ttu-id="2e7c4-244">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="2e7c4-244">Limit per app per tenant</span></span>     | <span data-ttu-id="2e7c4-245">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="2e7c4-245">Limit per app accross all tenants</span></span> |
|---------------------------|------------------------------|-----------------------------------|
| <span data-ttu-id="2e7c4-246">POSTAR, COLOCAR, EXCLUIR, PATCH</span><span class="sxs-lookup"><span data-stu-id="2e7c4-246">POST, PUT, DELETE, PATCH</span></span>  | <span data-ttu-id="2e7c4-247">1000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-247">1000 requests per 20 seconds</span></span> | <span data-ttu-id="2e7c4-248">2000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-248">2000 requests per 20 seconds</span></span>      |
| <span data-ttu-id="2e7c4-249">Todos os outros métodos HTTP</span><span class="sxs-lookup"><span data-stu-id="2e7c4-249">All other HTTP methods</span></span>    | <span data-ttu-id="2e7c4-250">5000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-250">5000 requests per 20 seconds</span></span> | <span data-ttu-id="2e7c4-251">10000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="2e7c4-251">10000 requests per 20 seconds</span></span>     |
