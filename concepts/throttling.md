---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 12ae7bf122d23c6460dcbc253b1fe743768e49ba
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123712"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="85457-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="85457-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="85457-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="85457-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="85457-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="85457-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="85457-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="85457-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="85457-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="85457-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="85457-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="85457-119">Common throttling scenarios</span></span>

<span data-ttu-id="85457-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="85457-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="85457-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="85457-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="85457-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="85457-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="85457-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="85457-123">Best practices to handle throttling</span></span>

<span data-ttu-id="85457-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="85457-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="85457-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="85457-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="85457-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="85457-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="85457-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="85457-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="85457-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="85457-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="85457-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="85457-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="85457-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="85457-132">Retry the request.</span></span>
3. <span data-ttu-id="85457-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="85457-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="85457-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="85457-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="85457-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="85457-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="85457-137">Foto</span><span class="sxs-lookup"><span data-stu-id="85457-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="85457-138">Email</span><span class="sxs-lookup"><span data-stu-id="85457-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="85457-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="85457-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="85457-140">Contato</span><span class="sxs-lookup"><span data-stu-id="85457-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="85457-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="85457-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="85457-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="85457-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="85457-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="85457-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="85457-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="85457-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="85457-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85457-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="85457-146">Relatório</span><span class="sxs-lookup"><span data-stu-id="85457-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="85457-147">Assinatura</span><span class="sxs-lookup"><span data-stu-id="85457-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="85457-148">Tendência</span><span class="sxs-lookup"><span data-stu-id="85457-148">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="85457-149">Percepção utilizada</span><span class="sxs-lookup"><span data-stu-id="85457-149">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="85457-150">Percepção compartilhada</span><span class="sxs-lookup"><span data-stu-id="85457-150">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="85457-151">Configurações do usuário</span><span class="sxs-lookup"><span data-stu-id="85457-151">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="85457-152">Convite</span><span class="sxs-lookup"><span data-stu-id="85457-152">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="85457-153">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="85457-153">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="85457-154">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="85457-154">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="85457-155">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="85457-155">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="85457-156">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="85457-156">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="85457-157">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="85457-157">Best practices to avoid throttling</span></span>

<span data-ttu-id="85457-158">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="85457-158">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="85457-159">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="85457-159">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="85457-160">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="85457-160">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="85457-161">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="85457-161">Service-specific limits</span></span>

<span data-ttu-id="85457-162">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85457-162">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="85457-163">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="85457-163">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="85457-164">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="85457-164">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="85457-165">**Nota:** Nesta seção, o termo *locatário* refere-se à organização Microsoft 365 onde o aplicativo está instalado.</span><span class="sxs-lookup"><span data-stu-id="85457-165">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="85457-166">Este inquilino pode ser o mesmo onde o aplicativo foi criado, no caso de um único aplicativo de inquilino, ou pode ser diferente, no caso de [um aplicativo de vários inquilinos](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="85457-166">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="85457-167">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="85457-167">Outlook service limits</span></span>

<span data-ttu-id="85457-168">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="85457-168">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="85457-169">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="85457-169">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="85457-170">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="85457-170">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="85457-171">Os seguintes limites se aplicam à nuvem pública, bem como às [ implementações de nuvens nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="85457-171">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="85457-172">Limite</span><span class="sxs-lookup"><span data-stu-id="85457-172">Limit</span></span>                                                      | <span data-ttu-id="85457-173">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="85457-173">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="85457-174">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="85457-174">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="85457-175">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="85457-175">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="85457-176">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="85457-176">4 concurrent requests</span></span>                                      | <span data-ttu-id="85457-177">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="85457-177">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="85457-178">15 megabytes (MB) de upload (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="85457-178">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="85457-179">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="85457-179">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="85457-180">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="85457-180">Outlook service resources</span></span>

<span data-ttu-id="85457-181">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="85457-181">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="85457-182">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="85457-182">Calendar API resources</span></span>

- [<span data-ttu-id="85457-183">event</span><span class="sxs-lookup"><span data-stu-id="85457-183">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="85457-184">eventMessage</span><span class="sxs-lookup"><span data-stu-id="85457-184">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="85457-185">calendar</span><span class="sxs-lookup"><span data-stu-id="85457-185">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="85457-186">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="85457-186">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="85457-187">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="85457-187">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="85457-188">attachment</span><span class="sxs-lookup"><span data-stu-id="85457-188">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="85457-189">place (preview)</span><span class="sxs-lookup"><span data-stu-id="85457-189">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="85457-190">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="85457-190">Mail API resources</span></span>

- [<span data-ttu-id="85457-191">message</span><span class="sxs-lookup"><span data-stu-id="85457-191">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="85457-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="85457-192">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="85457-193">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="85457-193">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="85457-194">messageRule</span><span class="sxs-lookup"><span data-stu-id="85457-194">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="85457-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="85457-195">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="85457-196">attachment</span><span class="sxs-lookup"><span data-stu-id="85457-196">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="85457-197">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="85457-197">Personal contacts API resources</span></span>

- [<span data-ttu-id="85457-198">contato</span><span class="sxs-lookup"><span data-stu-id="85457-198">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="85457-199">contactFolder</span><span class="sxs-lookup"><span data-stu-id="85457-199">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="85457-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="85457-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="85457-201">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="85457-201">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="85457-202">person</span><span class="sxs-lookup"><span data-stu-id="85457-202">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="85457-203">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="85457-203">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="85457-204">outlookTask</span><span class="sxs-lookup"><span data-stu-id="85457-204">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="85457-205">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="85457-205">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="85457-206">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="85457-206">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="85457-207">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="85457-207">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="85457-208">attachment</span><span class="sxs-lookup"><span data-stu-id="85457-208">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="85457-209">Limites dos serviços de comunicação em nuvem</span><span class="sxs-lookup"><span data-stu-id="85457-209">Cloud communication service limits</span></span>

| <span data-ttu-id="85457-210">Recurso</span><span class="sxs-lookup"><span data-stu-id="85457-210">Resource</span></span>      | <span data-ttu-id="85457-211">Limites por aplicativo e por inquilino</span><span class="sxs-lookup"><span data-stu-id="85457-211">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="85457-212">Chamadas</span><span class="sxs-lookup"><span data-stu-id="85457-212">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="85457-213">10.000 chamadas/mês e 100 chamadas simultâneas</span><span class="sxs-lookup"><span data-stu-id="85457-213">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="85457-214">Informações sobre a reunião </span><span class="sxs-lookup"><span data-stu-id="85457-214">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="85457-215">2000 reuniões/usuário a cada mês</span><span class="sxs-lookup"><span data-stu-id="85457-215">2000 meetings/user each month</span></span> |
| <span data-ttu-id="85457-216">[Presença](/graph/api/resources/presence) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="85457-216">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="85457-217">2 rps</span><span class="sxs-lookup"><span data-stu-id="85457-217">2 rps</span></span> |

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="85457-218">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="85457-218">Microsoft Teams service limits</span></span>

<span data-ttu-id="85457-219">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="85457-219">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="85457-220">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="85457-220">Teams request type</span></span>                                   | <span data-ttu-id="85457-221">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="85457-221">Limit per app per tenant</span></span>        | <span data-ttu-id="85457-222">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="85457-222">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="85457-223">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="85457-223">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="85457-224">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="85457-224">15000 requests every 10 seconds</span></span> | <span data-ttu-id="85457-225">n/d</span><span class="sxs-lookup"><span data-stu-id="85457-225">n/a</span></span> |
| <span data-ttu-id="85457-226">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="85457-226">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="85457-227">60 rps</span><span class="sxs-lookup"><span data-stu-id="85457-227">60 rps</span></span>                          | <span data-ttu-id="85457-228">600 rps</span><span class="sxs-lookup"><span data-stu-id="85457-228">600 rps</span></span> |
| <span data-ttu-id="85457-229">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="85457-229">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="85457-230">30 rps</span><span class="sxs-lookup"><span data-stu-id="85457-230">30 rps</span></span>                         | <span data-ttu-id="85457-231">300 rps</span><span class="sxs-lookup"><span data-stu-id="85457-231">300 rps</span></span>  |
| <span data-ttu-id="85457-232">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="85457-232">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="85457-233">30 rps</span><span class="sxs-lookup"><span data-stu-id="85457-233">30 rps</span></span>                         | <span data-ttu-id="85457-234">300 rps</span><span class="sxs-lookup"><span data-stu-id="85457-234">300 rps</span></span>  |
| <span data-ttu-id="85457-235">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="85457-235">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="85457-236">15 rps</span><span class="sxs-lookup"><span data-stu-id="85457-236">15 rps</span></span>                         | <span data-ttu-id="85457-237">150 rps</span><span class="sxs-lookup"><span data-stu-id="85457-237">150 rps</span></span>  |
| <span data-ttu-id="85457-238">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="85457-238">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="85457-239">30 rps</span><span class="sxs-lookup"><span data-stu-id="85457-239">30 rps</span></span>                         | <span data-ttu-id="85457-240">300 rps</span><span class="sxs-lookup"><span data-stu-id="85457-240">300 rps</span></span>  |
| <span data-ttu-id="85457-241">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="85457-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="85457-242">6 rps</span><span class="sxs-lookup"><span data-stu-id="85457-242">6 rps</span></span> | <span data-ttu-id="85457-243">150 rps</span><span class="sxs-lookup"><span data-stu-id="85457-243">150 rps</span></span>  | 
| <span data-ttu-id="85457-244">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="85457-244">GET channel message</span></span>  | <span data-ttu-id="85457-245">5 rps</span><span class="sxs-lookup"><span data-stu-id="85457-245">5 rps</span></span> | <span data-ttu-id="85457-246">100 rps</span><span class="sxs-lookup"><span data-stu-id="85457-246">100 rps</span></span> |
| <span data-ttu-id="85457-247">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="85457-247">GET 1:1/group chat message</span></span>  | <span data-ttu-id="85457-248">3 rps</span><span class="sxs-lookup"><span data-stu-id="85457-248">3 rps</span></span> | <span data-ttu-id="85457-249">30 rps</span><span class="sxs-lookup"><span data-stu-id="85457-249">30 rps</span></span> |
| <span data-ttu-id="85457-250">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="85457-250">POST channel message</span></span> | <span data-ttu-id="85457-251">2 rps</span><span class="sxs-lookup"><span data-stu-id="85457-251">2 rps</span></span> | <span data-ttu-id="85457-252">20 rps</span><span class="sxs-lookup"><span data-stu-id="85457-252">20 rps</span></span> |
| <span data-ttu-id="85457-253">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="85457-253">POST 1:1/group chat message</span></span> | <span data-ttu-id="85457-254">2 rps</span><span class="sxs-lookup"><span data-stu-id="85457-254">2 rps</span></span> | <span data-ttu-id="85457-255">20 rps</span><span class="sxs-lookup"><span data-stu-id="85457-255">20 rps</span></span> |
| <span data-ttu-id="85457-256">OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="85457-256">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="85457-257">60 rps</span><span class="sxs-lookup"><span data-stu-id="85457-257">60 rps</span></span> | <span data-ttu-id="85457-258">600 rps</span><span class="sxs-lookup"><span data-stu-id="85457-258">600 rps</span></span> |
| <span data-ttu-id="85457-259">PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="85457-259">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="85457-260">30 rps</span><span class="sxs-lookup"><span data-stu-id="85457-260">30 rps</span></span> | <span data-ttu-id="85457-261">300 rps</span><span class="sxs-lookup"><span data-stu-id="85457-261">300 rps</span></span> |
| <span data-ttu-id="85457-262">APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="85457-262">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="85457-263">15 rps</span><span class="sxs-lookup"><span data-stu-id="85457-263">15 rps</span></span> | <span data-ttu-id="85457-264">150 rps</span><span class="sxs-lookup"><span data-stu-id="85457-264">150 rps</span></span> |

<span data-ttu-id="85457-265">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="85457-265">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="85457-266">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="85457-266">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="85457-267">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="85457-267">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="85457-268">Proteção da identidade e limites do serviço de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="85457-268">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="85457-269">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="85457-269">Request type</span></span> | <span data-ttu-id="85457-270">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="85457-270">Limit per tenant</span></span> |
| ------------ | ------- |
| <span data-ttu-id="85457-271">Qualquer</span><span class="sxs-lookup"><span data-stu-id="85457-271">Any</span></span> | <span data-ttu-id="85457-272">1 solicitação por segundo</span><span class="sxs-lookup"><span data-stu-id="85457-272">1 request per second</span></span> |

<span data-ttu-id="85457-273">Os limites anteriores aplicam-se aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="85457-273">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="85457-274">Detecçãoderisco, Usuárioderisco, HistóricodeItemdeUsuárioderisco, NomedoLocal, paísNomedoLocal, ipNomedoLocal, PolíticadeAcessoCondicional.</span><span class="sxs-lookup"><span data-stu-id="85457-274">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="85457-275">**Nota:** no momento, os recursos listados acima não retornam um `Retry-After` cabeçalho sobre as `429 Too Many Requests` respostas.</span><span class="sxs-lookup"><span data-stu-id="85457-275">**Note:** at the moment the resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>
### <a name="insights-service-limits"></a><span data-ttu-id="85457-276">Percepção dos limites de serviço</span><span class="sxs-lookup"><span data-stu-id="85457-276">Insights service limits</span></span>

<span data-ttu-id="85457-277">Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="85457-277">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="85457-278">Limite</span><span class="sxs-lookup"><span data-stu-id="85457-278">Limit</span></span>                                                      | <span data-ttu-id="85457-279">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="85457-279">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="85457-280">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="85457-280">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="85457-281">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="85457-281">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="85457-282">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="85457-282">4 concurrent requests</span></span>                                      | <span data-ttu-id="85457-283">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="85457-283">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="85457-284">Limites do serviço de relatórios do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="85457-284">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="85457-285">Os seguintes limites se aplicam a qualquer solicitação no `/reports`.</span><span class="sxs-lookup"><span data-stu-id="85457-285">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="85457-286">Operation</span><span class="sxs-lookup"><span data-stu-id="85457-286">Operation</span></span>                 | <span data-ttu-id="85457-287">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="85457-287">Limit per app per tenant</span></span>     | <span data-ttu-id="85457-288">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="85457-288">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="85457-289">Qualquer pedido (CSV)</span><span class="sxs-lookup"><span data-stu-id="85457-289">Any request (CSV)</span></span>         | <span data-ttu-id="85457-290">14 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="85457-290">14 requests per 10 minutes</span></span>   | <span data-ttu-id="85457-291">40 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="85457-291">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="85457-292">Qualquer solicitação (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="85457-292">Any request (JSON, beta)</span></span>  | <span data-ttu-id="85457-293">100 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="85457-293">100 requests per 10 minutes</span></span>  | <span data-ttu-id="85457-294">n/d</span><span class="sxs-lookup"><span data-stu-id="85457-294">n/a</span></span>                        |

<span data-ttu-id="85457-295">Os limites anteriores aplicam-se individualmente a cada relatório de API.</span><span class="sxs-lookup"><span data-stu-id="85457-295">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="85457-296">Por exemplo, uma solicitação de relatório da API do usuário da Microsoft Teams e uma solicitação de relatório da API do usuário do Outlook dentro de 10 minutos contará como 1 solicitação de 14 para cada API e não 2 solicitações de 14 para ambas.</span><span class="sxs-lookup"><span data-stu-id="85457-296">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="85457-297">Limites de serviço do gerenciador de convite</span><span class="sxs-lookup"><span data-stu-id="85457-297">Invitation manager service limits</span></span>

<span data-ttu-id="85457-298">Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="85457-298">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="85457-299">Operation</span><span class="sxs-lookup"><span data-stu-id="85457-299">Operation</span></span>                 | <span data-ttu-id="85457-300">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="85457-300">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="85457-301">Qualquer operação</span><span class="sxs-lookup"><span data-stu-id="85457-301">Any operation</span></span>             | <span data-ttu-id="85457-302">150 solicitações a cada 5 segundos</span><span class="sxs-lookup"><span data-stu-id="85457-302">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="85457-303">Limites do serviço de Educação</span><span class="sxs-lookup"><span data-stu-id="85457-303">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="85457-304">Limites de serviço do Excel</span><span class="sxs-lookup"><span data-stu-id="85457-304">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="85457-305">Limites do serviço de registros de auditoria de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="85457-305">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="85457-306">Limites de serviço dos fornecedores de identidade</span><span class="sxs-lookup"><span data-stu-id="85457-306">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="85457-307">Limites de serviço Intune</span><span class="sxs-lookup"><span data-stu-id="85457-307">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="85457-308">Limites do serviço Skype</span><span class="sxs-lookup"><span data-stu-id="85457-308">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="85457-309">Limites do serviço de assinatura</span><span class="sxs-lookup"><span data-stu-id="85457-309">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
