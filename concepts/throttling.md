---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 96592654fffb3111a398178d807da702c398e0d2
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165111"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="da350-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="da350-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="da350-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="da350-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="da350-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="da350-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="da350-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="da350-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="da350-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="da350-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="da350-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="da350-119">Common throttling scenarios</span></span>

<span data-ttu-id="da350-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="da350-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="da350-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="da350-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="da350-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="da350-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="da350-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="da350-123">Best practices to handle throttling</span></span>

<span data-ttu-id="da350-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="da350-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="da350-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="da350-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="da350-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="da350-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="da350-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="da350-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="da350-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="da350-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="da350-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="da350-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="da350-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="da350-132">Retry the request.</span></span>
3. <span data-ttu-id="da350-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="da350-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="da350-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="da350-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="da350-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="da350-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="da350-137">Foto</span><span class="sxs-lookup"><span data-stu-id="da350-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="da350-138">Email</span><span class="sxs-lookup"><span data-stu-id="da350-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="da350-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="da350-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="da350-140">Contato</span><span class="sxs-lookup"><span data-stu-id="da350-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="da350-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="da350-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="da350-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="da350-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="da350-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="da350-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="da350-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="da350-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="da350-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da350-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="da350-146">Relatório</span><span class="sxs-lookup"><span data-stu-id="da350-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="da350-147">Assinatura</span><span class="sxs-lookup"><span data-stu-id="da350-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="da350-148">Solicitação de avaliação de ameaças</span><span class="sxs-lookup"><span data-stu-id="da350-148">Threat assessment request</span></span>](/graph/api/resources/threatassessmentrequest)
- [<span data-ttu-id="da350-149">Solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="da350-149">Mail assessment request</span></span>](/graph/api/resources/mailassessmentrequest)
- [<span data-ttu-id="da350-150">Solicitação de avaliação de arquivo de email</span><span class="sxs-lookup"><span data-stu-id="da350-150">Email file assessment request</span></span>](/graph/api/resources/emailfileassessmentrequest)
- [<span data-ttu-id="da350-151">Solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="da350-151">File assessment request</span></span>](/graph/api/resources/fileassessmentrequest)
- [<span data-ttu-id="da350-152">Solicitação de avaliação de URL</span><span class="sxs-lookup"><span data-stu-id="da350-152">URL assessment request</span></span>](/graph/api/resources/urlassessmentrequest)
- [<span data-ttu-id="da350-153">Resultado da avaliação de ameaças</span><span class="sxs-lookup"><span data-stu-id="da350-153">Threat assessment result</span></span>](/graph/api/resources/threatassessmentresult)
- [<span data-ttu-id="da350-154">Tendência</span><span class="sxs-lookup"><span data-stu-id="da350-154">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="da350-155">Percepção utilizada</span><span class="sxs-lookup"><span data-stu-id="da350-155">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="da350-156">Percepção compartilhada</span><span class="sxs-lookup"><span data-stu-id="da350-156">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="da350-157">Configurações do usuário</span><span class="sxs-lookup"><span data-stu-id="da350-157">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="da350-158">Convite</span><span class="sxs-lookup"><span data-stu-id="da350-158">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="da350-159">Para uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="da350-159">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="da350-160">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="da350-160">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="da350-161">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="da350-161">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="da350-162">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="da350-162">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="da350-163">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="da350-163">Best practices to avoid throttling</span></span>

<span data-ttu-id="da350-164">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="da350-164">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="da350-165">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="da350-165">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="da350-166">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="da350-166">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="da350-167">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="da350-167">Service-specific limits</span></span>

<span data-ttu-id="da350-168">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="da350-168">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="da350-169">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="da350-169">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="da350-170">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="da350-170">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="da350-171">**Nota:** Nesta seção, o termo *locatário* refere-se à organização Microsoft 365 onde o aplicativo está instalado.</span><span class="sxs-lookup"><span data-stu-id="da350-171">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="da350-172">Este inquilino pode ser o mesmo onde o aplicativo foi criado, no caso de um único aplicativo de inquilino, ou pode ser diferente, no caso de [um aplicativo de vários inquilinos](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="da350-172">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="da350-173">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="da350-173">Outlook service limits</span></span>

<span data-ttu-id="da350-174">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="da350-174">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="da350-175">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="da350-175">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="da350-176">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="da350-176">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="da350-177">Os seguintes limites se aplicam à nuvem pública, bem como às [ implementações de nuvens nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="da350-177">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="da350-178">Limite</span><span class="sxs-lookup"><span data-stu-id="da350-178">Limit</span></span>                                                      | <span data-ttu-id="da350-179">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="da350-179">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="da350-180">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="da350-180">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="da350-181">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="da350-181">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="da350-182">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="da350-182">4 concurrent requests</span></span>                                      | <span data-ttu-id="da350-183">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="da350-183">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="da350-184">15 megabytes (MB) de upload (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="da350-184">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="da350-185">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="da350-185">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="da350-186">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="da350-186">Outlook service resources</span></span>

<span data-ttu-id="da350-187">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="da350-187">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="da350-188">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="da350-188">Calendar API resources</span></span>

- [<span data-ttu-id="da350-189">event</span><span class="sxs-lookup"><span data-stu-id="da350-189">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="da350-190">eventMessage</span><span class="sxs-lookup"><span data-stu-id="da350-190">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="da350-191">calendar</span><span class="sxs-lookup"><span data-stu-id="da350-191">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="da350-192">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="da350-192">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="da350-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="da350-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="da350-194">attachment</span><span class="sxs-lookup"><span data-stu-id="da350-194">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="da350-195">place (preview)</span><span class="sxs-lookup"><span data-stu-id="da350-195">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="da350-196">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="da350-196">Mail API resources</span></span>

- [<span data-ttu-id="da350-197">message</span><span class="sxs-lookup"><span data-stu-id="da350-197">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="da350-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="da350-198">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="da350-199">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="da350-199">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="da350-200">messageRule</span><span class="sxs-lookup"><span data-stu-id="da350-200">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="da350-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="da350-201">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="da350-202">attachment</span><span class="sxs-lookup"><span data-stu-id="da350-202">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="da350-203">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="da350-203">Personal contacts API resources</span></span>

- [<span data-ttu-id="da350-204">contato</span><span class="sxs-lookup"><span data-stu-id="da350-204">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="da350-205">contactFolder</span><span class="sxs-lookup"><span data-stu-id="da350-205">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="da350-206">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="da350-206">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="da350-207">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="da350-207">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="da350-208">person</span><span class="sxs-lookup"><span data-stu-id="da350-208">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="da350-209">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="da350-209">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="da350-210">outlookTask</span><span class="sxs-lookup"><span data-stu-id="da350-210">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="da350-211">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="da350-211">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="da350-212">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="da350-212">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="da350-213">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="da350-213">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="da350-214">attachment</span><span class="sxs-lookup"><span data-stu-id="da350-214">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="da350-215">Limites dos serviços de comunicação em nuvem</span><span class="sxs-lookup"><span data-stu-id="da350-215">Cloud communication service limits</span></span>

| <span data-ttu-id="da350-216">Recurso</span><span class="sxs-lookup"><span data-stu-id="da350-216">Resource</span></span>      | <span data-ttu-id="da350-217">Limites por aplicativo e por inquilino</span><span class="sxs-lookup"><span data-stu-id="da350-217">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="da350-218">Chamadas</span><span class="sxs-lookup"><span data-stu-id="da350-218">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="da350-219">10.000 chamadas/mês e 100 chamadas simultâneas</span><span class="sxs-lookup"><span data-stu-id="da350-219">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="da350-220">Informações sobre a reunião </span><span class="sxs-lookup"><span data-stu-id="da350-220">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="da350-221">2000 reuniões/usuário a cada mês</span><span class="sxs-lookup"><span data-stu-id="da350-221">2000 meetings/user each month</span></span> |
| <span data-ttu-id="da350-222">[Presença](/graph/api/resources/presence) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="da350-222">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="da350-223">2 rps</span><span class="sxs-lookup"><span data-stu-id="da350-223">2 rps</span></span> |

### <a name="project-rome-service-limits"></a><span data-ttu-id="da350-224">Limites de serviços do Project Rome</span><span class="sxs-lookup"><span data-stu-id="da350-224">Project Rome service limits</span></span>

<span data-ttu-id="da350-225">| Tipo de solicitação | Limite por usuário a todos os aplicativos | | OBTENHA          | 400 solicitações a cada 5 minutos e 12000 solicitações por dia | | POSTAR, COLOCAR, CORRIGIR, EXCLUIR | 100 solicitações a cada 5 minutos e 8000 solicitações por dia |</span><span class="sxs-lookup"><span data-stu-id="da350-225">| Request type | Limit per user for all apps | | GET          | 400 requests per 5 minutes and 12000 requests per 1 day | | POST, PUT, PATCH, DELETE | 100 requests per 5 minutes and 8000 requests per 1 day |</span></span>

<span data-ttu-id="da350-226">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="da350-226">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="da350-227">activityHistoryItem, userActivity</span><span class="sxs-lookup"><span data-stu-id="da350-227">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="da350-228">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="da350-228">Microsoft Teams service limits</span></span>

<span data-ttu-id="da350-229">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="da350-229">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="da350-230">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="da350-230">Teams request type</span></span>                                   | <span data-ttu-id="da350-231">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="da350-231">Limit per app per tenant</span></span>        | <span data-ttu-id="da350-232">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="da350-232">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="da350-233">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="da350-233">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="da350-234">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="da350-234">15000 requests every 10 seconds</span></span> | <span data-ttu-id="da350-235">n/d</span><span class="sxs-lookup"><span data-stu-id="da350-235">n/a</span></span> |
| <span data-ttu-id="da350-236">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="da350-236">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="da350-237">60 rps</span><span class="sxs-lookup"><span data-stu-id="da350-237">60 rps</span></span>                          | <span data-ttu-id="da350-238">600 rps</span><span class="sxs-lookup"><span data-stu-id="da350-238">600 rps</span></span> |
| <span data-ttu-id="da350-239">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="da350-239">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="da350-240">30 rps</span><span class="sxs-lookup"><span data-stu-id="da350-240">30 rps</span></span>                         | <span data-ttu-id="da350-241">300 rps</span><span class="sxs-lookup"><span data-stu-id="da350-241">300 rps</span></span>  |
| <span data-ttu-id="da350-242">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="da350-242">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="da350-243">30 rps</span><span class="sxs-lookup"><span data-stu-id="da350-243">30 rps</span></span>                         | <span data-ttu-id="da350-244">300 rps</span><span class="sxs-lookup"><span data-stu-id="da350-244">300 rps</span></span>  |
| <span data-ttu-id="da350-245">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="da350-245">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="da350-246">15 rps</span><span class="sxs-lookup"><span data-stu-id="da350-246">15 rps</span></span>                         | <span data-ttu-id="da350-247">150 rps</span><span class="sxs-lookup"><span data-stu-id="da350-247">150 rps</span></span>  |
| <span data-ttu-id="da350-248">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="da350-248">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="da350-249">30 rps</span><span class="sxs-lookup"><span data-stu-id="da350-249">30 rps</span></span>                         | <span data-ttu-id="da350-250">300 rps</span><span class="sxs-lookup"><span data-stu-id="da350-250">300 rps</span></span>  |
| <span data-ttu-id="da350-251">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="da350-251">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="da350-252">6 rps</span><span class="sxs-lookup"><span data-stu-id="da350-252">6 rps</span></span> | <span data-ttu-id="da350-253">150 rps</span><span class="sxs-lookup"><span data-stu-id="da350-253">150 rps</span></span>  | 
| <span data-ttu-id="da350-254">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="da350-254">GET channel message</span></span>  | <span data-ttu-id="da350-255">5 rps</span><span class="sxs-lookup"><span data-stu-id="da350-255">5 rps</span></span> | <span data-ttu-id="da350-256">100 rps</span><span class="sxs-lookup"><span data-stu-id="da350-256">100 rps</span></span> |
| <span data-ttu-id="da350-257">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="da350-257">GET 1:1/group chat message</span></span>  | <span data-ttu-id="da350-258">3 rps</span><span class="sxs-lookup"><span data-stu-id="da350-258">3 rps</span></span> | <span data-ttu-id="da350-259">30 rps</span><span class="sxs-lookup"><span data-stu-id="da350-259">30 rps</span></span> |
| <span data-ttu-id="da350-260">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="da350-260">POST channel message</span></span> | <span data-ttu-id="da350-261">2 rps</span><span class="sxs-lookup"><span data-stu-id="da350-261">2 rps</span></span> | <span data-ttu-id="da350-262">20 rps</span><span class="sxs-lookup"><span data-stu-id="da350-262">20 rps</span></span> |
| <span data-ttu-id="da350-263">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="da350-263">POST 1:1/group chat message</span></span> | <span data-ttu-id="da350-264">2 rps</span><span class="sxs-lookup"><span data-stu-id="da350-264">2 rps</span></span> | <span data-ttu-id="da350-265">20 rps</span><span class="sxs-lookup"><span data-stu-id="da350-265">20 rps</span></span> |
| <span data-ttu-id="da350-266">OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="da350-266">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="da350-267">60 rps</span><span class="sxs-lookup"><span data-stu-id="da350-267">60 rps</span></span> | <span data-ttu-id="da350-268">600 rps</span><span class="sxs-lookup"><span data-stu-id="da350-268">600 rps</span></span> |
| <span data-ttu-id="da350-269">PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="da350-269">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="da350-270">30 rps</span><span class="sxs-lookup"><span data-stu-id="da350-270">30 rps</span></span> | <span data-ttu-id="da350-271">300 rps</span><span class="sxs-lookup"><span data-stu-id="da350-271">300 rps</span></span> |
| <span data-ttu-id="da350-272">APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="da350-272">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="da350-273">15 rps</span><span class="sxs-lookup"><span data-stu-id="da350-273">15 rps</span></span> | <span data-ttu-id="da350-274">150 rps</span><span class="sxs-lookup"><span data-stu-id="da350-274">150 rps</span></span> |

<span data-ttu-id="da350-275">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="da350-275">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="da350-276">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="da350-276">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="da350-277">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="da350-277">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="information-protection"></a><span data-ttu-id="da350-278">Proteção de informações</span><span class="sxs-lookup"><span data-stu-id="da350-278">Information protection</span></span>

<span data-ttu-id="da350-279">Os seguintes limites se aplicam a qualquer solicitação no `/informationProtection`.</span><span class="sxs-lookup"><span data-stu-id="da350-279">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="da350-280">Operation</span><span class="sxs-lookup"><span data-stu-id="da350-280">Operation</span></span>                 | <span data-ttu-id="da350-281">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="da350-281">Limit per tenant</span></span>                                            | <span data-ttu-id="da350-282">Limite por recurso (email, URL, arquivo)</span><span class="sxs-lookup"><span data-stu-id="da350-282">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="da350-283">POST</span><span class="sxs-lookup"><span data-stu-id="da350-283">POST</span></span>                      | <span data-ttu-id="da350-284">150 solicitações a cada 15 minutos e 10000 solicitações a cada 24 horas</span><span class="sxs-lookup"><span data-stu-id="da350-284">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="da350-285">1 solicitação a cada 15 minutos e 3 solicitações a cada 24 horas</span><span class="sxs-lookup"><span data-stu-id="da350-285">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="da350-286">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="da350-286">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="da350-287">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span><span class="sxs-lookup"><span data-stu-id="da350-287">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="da350-288">Proteção da identidade e limites do serviço de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="da350-288">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="da350-289">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="da350-289">Request type</span></span> | <span data-ttu-id="da350-290">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="da350-290">Limit per tenant</span></span> |
| ------------ | ------- |
| <span data-ttu-id="da350-291">Qualquer</span><span class="sxs-lookup"><span data-stu-id="da350-291">Any</span></span> | <span data-ttu-id="da350-292">1 solicitação por segundo</span><span class="sxs-lookup"><span data-stu-id="da350-292">1 request per second</span></span> |

<span data-ttu-id="da350-293">Os limites anteriores aplicam-se aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="da350-293">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="da350-294">Detecçãoderisco, Usuárioderisco, HistóricodeItemdeUsuárioderisco, NomedoLocal, paísNomedoLocal, ipNomedoLocal, PolíticadeAcessoCondicional.</span><span class="sxs-lookup"><span data-stu-id="da350-294">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="da350-295">**Nota:** no momento, os recursos listados acima não retornam um `Retry-After` cabeçalho sobre as `429 Too Many Requests` respostas.</span><span class="sxs-lookup"><span data-stu-id="da350-295">**Note:** at the moment the resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="da350-296">Percepção dos limites de serviço</span><span class="sxs-lookup"><span data-stu-id="da350-296">Insights service limits</span></span>

<span data-ttu-id="da350-297">Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="da350-297">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="da350-298">Limite</span><span class="sxs-lookup"><span data-stu-id="da350-298">Limit</span></span>                                                      | <span data-ttu-id="da350-299">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="da350-299">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="da350-300">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="da350-300">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="da350-301">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="da350-301">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="da350-302">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="da350-302">4 concurrent requests</span></span>                                      | <span data-ttu-id="da350-303">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="da350-303">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="da350-304">Limites do serviço de relatórios do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="da350-304">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="da350-305">Os seguintes limites se aplicam a qualquer solicitação no `/reports`.</span><span class="sxs-lookup"><span data-stu-id="da350-305">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="da350-306">Operation</span><span class="sxs-lookup"><span data-stu-id="da350-306">Operation</span></span>                 | <span data-ttu-id="da350-307">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="da350-307">Limit per app per tenant</span></span>     | <span data-ttu-id="da350-308">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="da350-308">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="da350-309">Qualquer pedido (CSV)</span><span class="sxs-lookup"><span data-stu-id="da350-309">Any request (CSV)</span></span>         | <span data-ttu-id="da350-310">14 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="da350-310">14 requests per 10 minutes</span></span>   | <span data-ttu-id="da350-311">40 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="da350-311">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="da350-312">Qualquer solicitação (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="da350-312">Any request (JSON, beta)</span></span>  | <span data-ttu-id="da350-313">100 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="da350-313">100 requests per 10 minutes</span></span>  | <span data-ttu-id="da350-314">n/d</span><span class="sxs-lookup"><span data-stu-id="da350-314">n/a</span></span>                        |

<span data-ttu-id="da350-315">Os limites anteriores aplicam-se individualmente a cada relatório de API.</span><span class="sxs-lookup"><span data-stu-id="da350-315">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="da350-316">Por exemplo, uma solicitação de relatório da API do usuário da Microsoft Teams e uma solicitação de relatório da API do usuário do Outlook dentro de 10 minutos contará como 1 solicitação de 14 para cada API e não 2 solicitações de 14 para ambas.</span><span class="sxs-lookup"><span data-stu-id="da350-316">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="da350-317">Limites de serviço do gerenciador de convite</span><span class="sxs-lookup"><span data-stu-id="da350-317">Invitation manager service limits</span></span>

<span data-ttu-id="da350-318">Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="da350-318">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="da350-319">Operation</span><span class="sxs-lookup"><span data-stu-id="da350-319">Operation</span></span>                 | <span data-ttu-id="da350-320">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="da350-320">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="da350-321">Qualquer operação</span><span class="sxs-lookup"><span data-stu-id="da350-321">Any operation</span></span>             | <span data-ttu-id="da350-322">150 solicitações a cada 5 segundos</span><span class="sxs-lookup"><span data-stu-id="da350-322">150 requests per 5 seconds</span></span>   |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="da350-323">Limitações de serviços à extensões de esquema e abertas</span><span class="sxs-lookup"><span data-stu-id="da350-323">Open and schema extensions service limits</span></span>

| <span data-ttu-id="da350-324">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="da350-324">Request type</span></span> | <span data-ttu-id="da350-325">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="da350-325">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="da350-326">Qualquer</span><span class="sxs-lookup"><span data-stu-id="da350-326">Any</span></span>          | <span data-ttu-id="da350-327">455 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="da350-327">455 requests per 10 seconds</span></span> |

<span data-ttu-id="da350-328">Os limites acima se aplicam aos seguintes recursos: openTypeExtension, schemaExtension, administrativeUnit, contato, dispositivo, evento, grupo, mensagem, organização, postagem e usuário.</span><span class="sxs-lookup"><span data-stu-id="da350-328">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="da350-329">Limites do serviço de Educação</span><span class="sxs-lookup"><span data-stu-id="da350-329">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="da350-330">Limites de serviço do Excel</span><span class="sxs-lookup"><span data-stu-id="da350-330">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="da350-331">Limites do serviço de registros de auditoria de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="da350-331">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="da350-332">Limites de serviço dos fornecedores de identidade</span><span class="sxs-lookup"><span data-stu-id="da350-332">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="da350-333">Limites de serviço Intune</span><span class="sxs-lookup"><span data-stu-id="da350-333">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="da350-334">Limites do serviço Skype</span><span class="sxs-lookup"><span data-stu-id="da350-334">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="da350-335">Limites do serviço de assinatura</span><span class="sxs-lookup"><span data-stu-id="da350-335">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
