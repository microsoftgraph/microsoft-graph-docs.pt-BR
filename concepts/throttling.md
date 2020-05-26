---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: d33ac4612f4fe3934c53235360626dac1393ab21
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44215784"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="ed807-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ed807-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="ed807-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ed807-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="ed807-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="ed807-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="ed807-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="ed807-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="ed807-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="ed807-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="ed807-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="ed807-119">Common throttling scenarios</span></span>

<span data-ttu-id="ed807-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="ed807-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="ed807-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="ed807-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="ed807-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="ed807-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="ed807-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="ed807-123">Best practices to handle throttling</span></span>

<span data-ttu-id="ed807-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="ed807-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="ed807-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed807-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="ed807-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="ed807-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="ed807-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="ed807-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="ed807-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="ed807-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="ed807-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="ed807-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="ed807-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed807-132">Retry the request.</span></span>
3. <span data-ttu-id="ed807-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="ed807-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="ed807-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="ed807-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="ed807-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="ed807-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-137">Foto</span><span class="sxs-lookup"><span data-stu-id="ed807-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-138">Email</span><span class="sxs-lookup"><span data-stu-id="ed807-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="ed807-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-140">Contato</span><span class="sxs-lookup"><span data-stu-id="ed807-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="ed807-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="ed807-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="ed807-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="ed807-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="ed807-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="ed807-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed807-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

<span data-ttu-id="ed807-146">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="ed807-146">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="ed807-147">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="ed807-147">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="ed807-148">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="ed807-148">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="ed807-149">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="ed807-149">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="ed807-150">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="ed807-150">Best practices to avoid throttling</span></span>

<span data-ttu-id="ed807-151">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="ed807-151">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="ed807-152">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ed807-152">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="ed807-153">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="ed807-153">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="ed807-154">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="ed807-154">Service-specific limits</span></span>

<span data-ttu-id="ed807-155">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ed807-155">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="ed807-156">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="ed807-156">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="ed807-157">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed807-157">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="ed807-158">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="ed807-158">Outlook service limits</span></span>

<span data-ttu-id="ed807-159">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ed807-159">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="ed807-160">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="ed807-160">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="ed807-161">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ed807-161">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="ed807-162">Limite</span><span class="sxs-lookup"><span data-stu-id="ed807-162">Limit</span></span>                                                      | <span data-ttu-id="ed807-163">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="ed807-163">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="ed807-164">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="ed807-164">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="ed807-165">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="ed807-165">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="ed807-166">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="ed807-166">4 concurrent requests</span></span>                                      | <span data-ttu-id="ed807-167">Ponto de extremidade Beta</span><span class="sxs-lookup"><span data-stu-id="ed807-167">Beta endpoint</span></span>   |
| <span data-ttu-id="ed807-168">carregamento de 15 megabits (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="ed807-168">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="ed807-169">Ponto de extremidade Beta</span><span class="sxs-lookup"><span data-stu-id="ed807-169">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="ed807-170">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="ed807-170">Outlook service resources</span></span>

<span data-ttu-id="ed807-171">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="ed807-171">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="ed807-172">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="ed807-172">Calendar API resources</span></span>

- [<span data-ttu-id="ed807-173">event</span><span class="sxs-lookup"><span data-stu-id="ed807-173">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="ed807-174">eventMessage</span><span class="sxs-lookup"><span data-stu-id="ed807-174">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="ed807-175">calendar</span><span class="sxs-lookup"><span data-stu-id="ed807-175">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="ed807-176">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="ed807-176">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="ed807-177">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ed807-177">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="ed807-178">attachment</span><span class="sxs-lookup"><span data-stu-id="ed807-178">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="ed807-179">place (preview)</span><span class="sxs-lookup"><span data-stu-id="ed807-179">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="ed807-180">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="ed807-180">Mail API resources</span></span>

- [<span data-ttu-id="ed807-181">message</span><span class="sxs-lookup"><span data-stu-id="ed807-181">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="ed807-182">mailFolder</span><span class="sxs-lookup"><span data-stu-id="ed807-182">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="ed807-183">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="ed807-183">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="ed807-184">messageRule</span><span class="sxs-lookup"><span data-stu-id="ed807-184">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="ed807-185">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ed807-185">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="ed807-186">attachment</span><span class="sxs-lookup"><span data-stu-id="ed807-186">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="ed807-187">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="ed807-187">Personal contacts API resources</span></span>

- [<span data-ttu-id="ed807-188">contato</span><span class="sxs-lookup"><span data-stu-id="ed807-188">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="ed807-189">contactFolder</span><span class="sxs-lookup"><span data-stu-id="ed807-189">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="ed807-190">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ed807-190">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="ed807-191">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="ed807-191">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="ed807-192">person</span><span class="sxs-lookup"><span data-stu-id="ed807-192">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="ed807-193">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="ed807-193">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="ed807-194">outlookTask</span><span class="sxs-lookup"><span data-stu-id="ed807-194">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="ed807-195">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ed807-195">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="ed807-196">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="ed807-196">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="ed807-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ed807-197">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="ed807-198">attachment</span><span class="sxs-lookup"><span data-stu-id="ed807-198">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="ed807-199">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ed807-199">Microsoft Teams service limits</span></span>

<span data-ttu-id="ed807-200">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="ed807-200">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="ed807-201">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="ed807-201">Teams request type</span></span>                                   | <span data-ttu-id="ed807-202">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="ed807-202">Limit per app per tenant</span></span>        | <span data-ttu-id="ed807-203">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="ed807-203">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="ed807-204">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ed807-204">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="ed807-205">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="ed807-205">15000 requests every 10 seconds</span></span> | <span data-ttu-id="ed807-206">n/d</span><span class="sxs-lookup"><span data-stu-id="ed807-206">n/a</span></span> |
| <span data-ttu-id="ed807-207">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="ed807-207">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="ed807-208">60 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-208">60 rps</span></span>                          | <span data-ttu-id="ed807-209">600 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-209">600 rps</span></span> |
| <span data-ttu-id="ed807-210">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="ed807-210">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="ed807-211">30 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-211">30 rps</span></span>                         | <span data-ttu-id="ed807-212">300 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-212">300 rps</span></span>  |
| <span data-ttu-id="ed807-213">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="ed807-213">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="ed807-214">30 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-214">30 rps</span></span>                         | <span data-ttu-id="ed807-215">300 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-215">300 rps</span></span>  |
| <span data-ttu-id="ed807-216">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="ed807-216">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="ed807-217">15 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-217">15 rps</span></span>                         | <span data-ttu-id="ed807-218">150 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-218">150 rps</span></span>  |
| <span data-ttu-id="ed807-219">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="ed807-219">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="ed807-220">30 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-220">30 rps</span></span>                         | <span data-ttu-id="ed807-221">300 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-221">300 rps</span></span>  |
| <span data-ttu-id="ed807-222">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="ed807-222">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="ed807-223">6 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-223">6 rps</span></span> | <span data-ttu-id="ed807-224">150 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-224">150 rps</span></span>  | 
| <span data-ttu-id="ed807-225">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="ed807-225">GET channel message</span></span>  | <span data-ttu-id="ed807-226">5 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-226">5 rps</span></span> | <span data-ttu-id="ed807-227">100 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-227">100 rps</span></span> |
| <span data-ttu-id="ed807-228">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="ed807-228">GET 1:1/group chat message</span></span>  | <span data-ttu-id="ed807-229">3 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-229">3 rps</span></span> | <span data-ttu-id="ed807-230">30 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-230">30 rps</span></span> |
| <span data-ttu-id="ed807-231">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="ed807-231">POST channel message</span></span> | <span data-ttu-id="ed807-232">2 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-232">2 rps</span></span> | <span data-ttu-id="ed807-233">20 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-233">20 rps</span></span> |
| <span data-ttu-id="ed807-234">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="ed807-234">POST 1:1/group chat message</span></span> | <span data-ttu-id="ed807-235">2 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-235">2 rps</span></span> | <span data-ttu-id="ed807-236">20 rps</span><span class="sxs-lookup"><span data-stu-id="ed807-236">20 rps</span></span> |

<span data-ttu-id="ed807-237">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="ed807-237">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="ed807-238">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="ed807-238">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="ed807-239">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="ed807-239">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="microsoft-graph-change-notifications-subscription-operations"></a><span data-ttu-id="ed807-240">Operações de notificações de mudança de assinatura do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ed807-240">Microsoft Graph change notifications subscription operations</span></span>

<span data-ttu-id="ed807-241">Os seguintes limites se aplicam a qualquer solicitação no `/subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="ed807-241">The following limits apply to any request on `/subscriptions`.</span></span>

| <span data-ttu-id="ed807-242">Operation</span><span class="sxs-lookup"><span data-stu-id="ed807-242">Operation</span></span>                 | <span data-ttu-id="ed807-243">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="ed807-243">Limit per app per tenant</span></span>     | <span data-ttu-id="ed807-244">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="ed807-244">Limit per app accross all tenants</span></span> |
|---------------------------|------------------------------|-----------------------------------|
| <span data-ttu-id="ed807-245">POSTAR, COLOCAR, EXCLUIR, PATCH</span><span class="sxs-lookup"><span data-stu-id="ed807-245">POST, PUT, DELETE, PATCH</span></span>  | <span data-ttu-id="ed807-246">1000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="ed807-246">1000 requests per 20 seconds</span></span> | <span data-ttu-id="ed807-247">2000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="ed807-247">2000 requests per 20 seconds</span></span>      |
| <span data-ttu-id="ed807-248">Todos os outros métodos HTTP</span><span class="sxs-lookup"><span data-stu-id="ed807-248">All other HTTP methods</span></span>    | <span data-ttu-id="ed807-249">5000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="ed807-249">5000 requests per 20 seconds</span></span> | <span data-ttu-id="ed807-250">10000 solicitações por 20 segundos</span><span class="sxs-lookup"><span data-stu-id="ed807-250">10000 requests per 20 seconds</span></span>     |
