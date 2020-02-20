---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 36a20e88e8755a6a38140759f3cac568efbdf18c
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108466"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="01196-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="01196-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="01196-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="01196-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="01196-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="01196-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="01196-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="01196-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="01196-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="01196-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="01196-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="01196-119">Common throttling scenarios</span></span>

<span data-ttu-id="01196-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="01196-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="01196-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="01196-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="01196-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="01196-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="01196-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="01196-123">Best practices to handle throttling</span></span>

<span data-ttu-id="01196-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="01196-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="01196-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="01196-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="01196-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="01196-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="01196-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="01196-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="01196-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="01196-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="01196-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="01196-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="01196-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="01196-132">Retry the request.</span></span>
3. <span data-ttu-id="01196-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="01196-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="01196-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="01196-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="01196-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="01196-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="01196-137">Foto</span><span class="sxs-lookup"><span data-stu-id="01196-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="01196-138">Email</span><span class="sxs-lookup"><span data-stu-id="01196-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="01196-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="01196-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="01196-140">Contato</span><span class="sxs-lookup"><span data-stu-id="01196-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="01196-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="01196-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="01196-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="01196-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="01196-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="01196-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="01196-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="01196-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)

<span data-ttu-id="01196-145">Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="01196-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="01196-146">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="01196-146">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="01196-147">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="01196-147">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span> 
> 
> <span data-ttu-id="01196-148">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="01196-148">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="01196-149">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="01196-149">Service-specific limits</span></span>

<span data-ttu-id="01196-150">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="01196-150">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="01196-151">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="01196-151">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="01196-152">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="01196-152">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="01196-153">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="01196-153">Outlook service limits</span></span>

<span data-ttu-id="01196-154">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="01196-154">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="01196-155">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="01196-155">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="01196-156">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="01196-156">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="01196-157">Limite</span><span class="sxs-lookup"><span data-stu-id="01196-157">Limit</span></span>                                                      | <span data-ttu-id="01196-158">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="01196-158">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="01196-159">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="01196-159">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="01196-160">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="01196-160">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="01196-161">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="01196-161">4 concurrent requests</span></span>                                      | <span data-ttu-id="01196-162">Ponto de extremidade Beta</span><span class="sxs-lookup"><span data-stu-id="01196-162">Beta endpoint</span></span>   |
| <span data-ttu-id="01196-163">carregamento de 15 megabits (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="01196-163">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="01196-164">Ponto de extremidade Beta</span><span class="sxs-lookup"><span data-stu-id="01196-164">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="01196-165">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="01196-165">Outlook service resources</span></span>

<span data-ttu-id="01196-166">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="01196-166">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="01196-167">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="01196-167">Calendar API resources</span></span>

- [<span data-ttu-id="01196-168">event</span><span class="sxs-lookup"><span data-stu-id="01196-168">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="01196-169">eventMessage</span><span class="sxs-lookup"><span data-stu-id="01196-169">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="01196-170">calendar</span><span class="sxs-lookup"><span data-stu-id="01196-170">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="01196-171">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="01196-171">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="01196-172">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="01196-172">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="01196-173">attachment</span><span class="sxs-lookup"><span data-stu-id="01196-173">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="01196-174">place (preview)</span><span class="sxs-lookup"><span data-stu-id="01196-174">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="01196-175">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="01196-175">Mail API resources</span></span>

- [<span data-ttu-id="01196-176">message</span><span class="sxs-lookup"><span data-stu-id="01196-176">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="01196-177">mailFolder</span><span class="sxs-lookup"><span data-stu-id="01196-177">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="01196-178">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="01196-178">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="01196-179">messageRule</span><span class="sxs-lookup"><span data-stu-id="01196-179">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="01196-180">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="01196-180">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="01196-181">attachment</span><span class="sxs-lookup"><span data-stu-id="01196-181">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="01196-182">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="01196-182">Personal contacts API resources</span></span>

- [<span data-ttu-id="01196-183">contato</span><span class="sxs-lookup"><span data-stu-id="01196-183">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="01196-184">contactFolder</span><span class="sxs-lookup"><span data-stu-id="01196-184">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="01196-185">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="01196-185">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="01196-186">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="01196-186">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="01196-187">person</span><span class="sxs-lookup"><span data-stu-id="01196-187">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="01196-188">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="01196-188">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="01196-189">outlookTask</span><span class="sxs-lookup"><span data-stu-id="01196-189">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="01196-190">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="01196-190">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="01196-191">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="01196-191">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="01196-192">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="01196-192">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="01196-193">attachment</span><span class="sxs-lookup"><span data-stu-id="01196-193">attachment</span></span>](/graph/api/resources/attachment)
