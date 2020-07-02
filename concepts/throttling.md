---
title: Diretrizes de limitação do Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7678b364855381eaf5a138b42d6172a6cbd233f4
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989839"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="db804-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="db804-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="db804-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="db804-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="db804-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="db804-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="db804-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="db804-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="db804-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="db804-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="db804-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="db804-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="db804-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="db804-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="db804-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="db804-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="db804-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="db804-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="db804-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="db804-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="db804-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="db804-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="db804-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="db804-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="db804-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="db804-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="db804-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="db804-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="db804-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="db804-119">Common throttling scenarios</span></span>

<span data-ttu-id="db804-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="db804-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="db804-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="db804-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="db804-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="db804-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="db804-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="db804-123">Best practices to handle throttling</span></span>

<span data-ttu-id="db804-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="db804-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="db804-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="db804-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="db804-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="db804-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="db804-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="db804-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="db804-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="db804-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="db804-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="db804-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="db804-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="db804-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="db804-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="db804-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="db804-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="db804-132">Retry the request.</span></span>
3. <span data-ttu-id="db804-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="db804-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="db804-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="db804-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="db804-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="db804-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="db804-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="db804-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="db804-137">Foto</span><span class="sxs-lookup"><span data-stu-id="db804-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="db804-138">Email</span><span class="sxs-lookup"><span data-stu-id="db804-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="db804-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="db804-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="db804-140">Contato</span><span class="sxs-lookup"><span data-stu-id="db804-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="db804-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="db804-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="db804-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="db804-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="db804-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="db804-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="db804-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="db804-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="db804-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db804-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="db804-146">Assinatura</span><span class="sxs-lookup"><span data-stu-id="db804-146">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="db804-147">Convite</span><span class="sxs-lookup"><span data-stu-id="db804-147">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="db804-148">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="db804-148">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="db804-149">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="db804-149">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="db804-150">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="db804-150">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="db804-151">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="db804-151">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="db804-152">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="db804-152">Best practices to avoid throttling</span></span>

<span data-ttu-id="db804-153">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="db804-153">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="db804-154">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="db804-154">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="db804-155">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="db804-155">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="db804-156">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="db804-156">Service-specific limits</span></span>

<span data-ttu-id="db804-157">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="db804-157">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="db804-158">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="db804-158">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="db804-159">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="db804-159">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="db804-160">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="db804-160">Outlook service limits</span></span>

<span data-ttu-id="db804-161">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="db804-161">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="db804-162">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="db804-162">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="db804-163">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="db804-163">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="db804-164">Os limites a seguir se aplicam à nuvem pública, bem como às [implantações nacionais da nuvem](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="db804-164">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="db804-165">Limite</span><span class="sxs-lookup"><span data-stu-id="db804-165">Limit</span></span>                                                      | <span data-ttu-id="db804-166">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="db804-166">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="db804-167">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="db804-167">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="db804-168">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="db804-168">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="db804-169">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="db804-169">4 concurrent requests</span></span>                                      | <span data-ttu-id="db804-170">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="db804-170">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="db804-171">carregamento de 15 megabits (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="db804-171">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="db804-172">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="db804-172">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="db804-173">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="db804-173">Outlook service resources</span></span>

<span data-ttu-id="db804-174">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="db804-174">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="db804-175">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="db804-175">Calendar API resources</span></span>

- [<span data-ttu-id="db804-176">event</span><span class="sxs-lookup"><span data-stu-id="db804-176">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="db804-177">eventMessage</span><span class="sxs-lookup"><span data-stu-id="db804-177">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="db804-178">calendar</span><span class="sxs-lookup"><span data-stu-id="db804-178">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="db804-179">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="db804-179">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="db804-180">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="db804-180">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="db804-181">attachment</span><span class="sxs-lookup"><span data-stu-id="db804-181">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="db804-182">place (preview)</span><span class="sxs-lookup"><span data-stu-id="db804-182">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="db804-183">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="db804-183">Mail API resources</span></span>

- [<span data-ttu-id="db804-184">message</span><span class="sxs-lookup"><span data-stu-id="db804-184">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="db804-185">mailFolder</span><span class="sxs-lookup"><span data-stu-id="db804-185">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="db804-186">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="db804-186">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="db804-187">messageRule</span><span class="sxs-lookup"><span data-stu-id="db804-187">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="db804-188">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="db804-188">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="db804-189">attachment</span><span class="sxs-lookup"><span data-stu-id="db804-189">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="db804-190">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="db804-190">Personal contacts API resources</span></span>

- [<span data-ttu-id="db804-191">contato</span><span class="sxs-lookup"><span data-stu-id="db804-191">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="db804-192">contactFolder</span><span class="sxs-lookup"><span data-stu-id="db804-192">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="db804-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="db804-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="db804-194">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="db804-194">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="db804-195">person</span><span class="sxs-lookup"><span data-stu-id="db804-195">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="db804-196">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="db804-196">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="db804-197">outlookTask</span><span class="sxs-lookup"><span data-stu-id="db804-197">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="db804-198">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="db804-198">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="db804-199">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="db804-199">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="db804-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="db804-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="db804-201">attachment</span><span class="sxs-lookup"><span data-stu-id="db804-201">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="db804-202">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="db804-202">Microsoft Teams service limits</span></span>

<span data-ttu-id="db804-203">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="db804-203">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="db804-204">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="db804-204">Teams request type</span></span>                                   | <span data-ttu-id="db804-205">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="db804-205">Limit per app per tenant</span></span>        | <span data-ttu-id="db804-206">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="db804-206">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="db804-207">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="db804-207">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="db804-208">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="db804-208">15000 requests every 10 seconds</span></span> | <span data-ttu-id="db804-209">n/d</span><span class="sxs-lookup"><span data-stu-id="db804-209">n/a</span></span> |
| <span data-ttu-id="db804-210">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="db804-210">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="db804-211">60 rps</span><span class="sxs-lookup"><span data-stu-id="db804-211">60 rps</span></span>                          | <span data-ttu-id="db804-212">600 rps</span><span class="sxs-lookup"><span data-stu-id="db804-212">600 rps</span></span> |
| <span data-ttu-id="db804-213">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="db804-213">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="db804-214">30 rps</span><span class="sxs-lookup"><span data-stu-id="db804-214">30 rps</span></span>                         | <span data-ttu-id="db804-215">300 rps</span><span class="sxs-lookup"><span data-stu-id="db804-215">300 rps</span></span>  |
| <span data-ttu-id="db804-216">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="db804-216">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="db804-217">30 rps</span><span class="sxs-lookup"><span data-stu-id="db804-217">30 rps</span></span>                         | <span data-ttu-id="db804-218">300 rps</span><span class="sxs-lookup"><span data-stu-id="db804-218">300 rps</span></span>  |
| <span data-ttu-id="db804-219">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="db804-219">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="db804-220">15 rps</span><span class="sxs-lookup"><span data-stu-id="db804-220">15 rps</span></span>                         | <span data-ttu-id="db804-221">150 rps</span><span class="sxs-lookup"><span data-stu-id="db804-221">150 rps</span></span>  |
| <span data-ttu-id="db804-222">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="db804-222">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="db804-223">30 rps</span><span class="sxs-lookup"><span data-stu-id="db804-223">30 rps</span></span>                         | <span data-ttu-id="db804-224">300 rps</span><span class="sxs-lookup"><span data-stu-id="db804-224">300 rps</span></span>  |
| <span data-ttu-id="db804-225">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="db804-225">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="db804-226">6 rps</span><span class="sxs-lookup"><span data-stu-id="db804-226">6 rps</span></span> | <span data-ttu-id="db804-227">150 rps</span><span class="sxs-lookup"><span data-stu-id="db804-227">150 rps</span></span>  | 
| <span data-ttu-id="db804-228">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="db804-228">GET channel message</span></span>  | <span data-ttu-id="db804-229">5 rps</span><span class="sxs-lookup"><span data-stu-id="db804-229">5 rps</span></span> | <span data-ttu-id="db804-230">100 rps</span><span class="sxs-lookup"><span data-stu-id="db804-230">100 rps</span></span> |
| <span data-ttu-id="db804-231">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="db804-231">GET 1:1/group chat message</span></span>  | <span data-ttu-id="db804-232">3 rps</span><span class="sxs-lookup"><span data-stu-id="db804-232">3 rps</span></span> | <span data-ttu-id="db804-233">30 rps</span><span class="sxs-lookup"><span data-stu-id="db804-233">30 rps</span></span> |
| <span data-ttu-id="db804-234">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="db804-234">POST channel message</span></span> | <span data-ttu-id="db804-235">2 rps</span><span class="sxs-lookup"><span data-stu-id="db804-235">2 rps</span></span> | <span data-ttu-id="db804-236">20 rps</span><span class="sxs-lookup"><span data-stu-id="db804-236">20 rps</span></span> |
| <span data-ttu-id="db804-237">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="db804-237">POST 1:1/group chat message</span></span> | <span data-ttu-id="db804-238">2 rps</span><span class="sxs-lookup"><span data-stu-id="db804-238">2 rps</span></span> | <span data-ttu-id="db804-239">20 rps</span><span class="sxs-lookup"><span data-stu-id="db804-239">20 rps</span></span> |

<span data-ttu-id="db804-240">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="db804-240">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="db804-241">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="db804-241">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="db804-242">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="db804-242">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="db804-243">Limites do serviço Gerenciador de convites</span><span class="sxs-lookup"><span data-stu-id="db804-243">Invitation manager service limits</span></span>

<span data-ttu-id="db804-244">Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="db804-244">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="db804-245">Operation</span><span class="sxs-lookup"><span data-stu-id="db804-245">Operation</span></span>                 | <span data-ttu-id="db804-246">Limite por locatário</span><span class="sxs-lookup"><span data-stu-id="db804-246">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="db804-247">Qualquer operação</span><span class="sxs-lookup"><span data-stu-id="db804-247">Any operation</span></span>             | <span data-ttu-id="db804-248">150 solicitações por 5 segundos</span><span class="sxs-lookup"><span data-stu-id="db804-248">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a><span data-ttu-id="db804-249">Limites do serviço de educação</span><span class="sxs-lookup"><span data-stu-id="db804-249">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="db804-250">Limites do serviço do Excel</span><span class="sxs-lookup"><span data-stu-id="db804-250">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="db804-251">Limites de serviço de logs de auditoria de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="db804-251">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="db804-252">Limites de serviço de provedores de identidade</span><span class="sxs-lookup"><span data-stu-id="db804-252">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="db804-253">Limites de serviço do Intune</span><span class="sxs-lookup"><span data-stu-id="db804-253">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="db804-254">Limites do serviço Skype</span><span class="sxs-lookup"><span data-stu-id="db804-254">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="db804-255">Limites do serviço de assinatura</span><span class="sxs-lookup"><span data-stu-id="db804-255">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
