---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 71bb61a6bb2a72cc3e2cc4192e1a6d218ab4c3b4
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589176"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="77187-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="77187-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="77187-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="77187-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="77187-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="77187-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="77187-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="77187-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="77187-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="77187-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="77187-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="77187-119">Common throttling scenarios</span></span>

<span data-ttu-id="77187-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="77187-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="77187-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="77187-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="77187-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="77187-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="77187-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="77187-123">Best practices to handle throttling</span></span>

<span data-ttu-id="77187-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="77187-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="77187-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="77187-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="77187-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="77187-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="77187-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="77187-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="77187-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="77187-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="77187-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="77187-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="77187-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="77187-132">Retry the request.</span></span>
3. <span data-ttu-id="77187-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="77187-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="77187-135">Todos os recursos e as APIs descritos na seção [limites específicos do serviço](#service-specific-limits) fornecem um `Retry-After`cabeçalho, exceto sob ressalva.</span><span class="sxs-lookup"><span data-stu-id="77187-135">All the resources and APIs described in the [Service-specific limits](#service-specific-limits) section provide a `Retry-After` header except when noted.</span></span>

<span data-ttu-id="77187-136">Para uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="77187-136">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="77187-137">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="77187-137">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="77187-138">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="77187-138">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="77187-139">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="77187-139">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="77187-140">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="77187-140">Best practices to avoid throttling</span></span>

<span data-ttu-id="77187-141">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="77187-141">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="77187-142">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="77187-142">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="77187-143">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="77187-143">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="77187-144">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="77187-144">Service-specific limits</span></span>

<span data-ttu-id="77187-145">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77187-145">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="77187-146">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="77187-146">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="77187-147">Qualquer solicitação poderá ser avaliada em relação a vários limites, dependendo do escopo do limite (por aplicativo em todos os locatários, por locatário para todos os aplicativos, por aplicativo por locatário, e assim por diante), do tipo de solicitação (GET, POST, PATCH e assim por diante) e de outros fatores.</span><span class="sxs-lookup"><span data-stu-id="77187-147">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="77187-148">O primeiro limite a ser alcançado dispara o comportamento de limitação.</span><span class="sxs-lookup"><span data-stu-id="77187-148">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="77187-149">Além dos limites de serviço específicos descritos na seção, os seguintes limites globais se aplicam:</span><span class="sxs-lookup"><span data-stu-id="77187-149">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="77187-150">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="77187-150">Request type</span></span> | <span data-ttu-id="77187-151">Por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="77187-151">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="77187-152">Qualquer</span><span class="sxs-lookup"><span data-stu-id="77187-152">Any</span></span>          | <span data-ttu-id="77187-153">2000 solicitações por segundo</span><span class="sxs-lookup"><span data-stu-id="77187-153">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="77187-154">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="77187-154">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="77187-155">**Nota:** Nesta seção, o termo *locatário* refere-se à organização Microsoft 365 onde o aplicativo está instalado.</span><span class="sxs-lookup"><span data-stu-id="77187-155">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="77187-156">Este inquilino pode ser o mesmo onde o aplicativo foi criado, no caso de um único aplicativo de inquilino, ou pode ser diferente, no caso de [um aplicativo de vários inquilinos](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="77187-156">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="77187-157">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="77187-157">Outlook service limits</span></span>

<span data-ttu-id="77187-158">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77187-158">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="77187-159">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="77187-159">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="77187-160">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77187-160">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="77187-161">Os seguintes limites se aplicam à nuvem pública, bem como às [ implementações de nuvens nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="77187-161">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="77187-162">Limite</span><span class="sxs-lookup"><span data-stu-id="77187-162">Limit</span></span>                                                      | <span data-ttu-id="77187-163">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="77187-163">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="77187-164">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="77187-164">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="77187-165">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="77187-165">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="77187-166">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-166">4 concurrent requests</span></span>                                      | <span data-ttu-id="77187-167">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="77187-167">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="77187-168">15 megabytes (MB) de upload (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="77187-168">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="77187-169">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="77187-169">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="77187-170">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="77187-170">Outlook service resources</span></span>

<span data-ttu-id="77187-171">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="77187-171">The following resources are provided by the Outlook service.</span></span>

##### <a name="search-api-resources-preview"></a><span data-ttu-id="77187-172">Pesquisar recursos da API (visualização)</span><span class="sxs-lookup"><span data-stu-id="77187-172">Search API resources (preview)</span></span>

- [<span data-ttu-id="77187-173">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77187-173">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a><span data-ttu-id="77187-174">Recursos da API de perfil</span><span class="sxs-lookup"><span data-stu-id="77187-174">Profile API resources</span></span>

- [<span data-ttu-id="77187-175">Foto</span><span class="sxs-lookup"><span data-stu-id="77187-175">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a><span data-ttu-id="77187-176">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="77187-176">Calendar API resources</span></span>

- [<span data-ttu-id="77187-177">event</span><span class="sxs-lookup"><span data-stu-id="77187-177">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="77187-178">eventMessage</span><span class="sxs-lookup"><span data-stu-id="77187-178">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="77187-179">calendar</span><span class="sxs-lookup"><span data-stu-id="77187-179">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="77187-180">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="77187-180">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="77187-181">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77187-181">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="77187-182">attachment</span><span class="sxs-lookup"><span data-stu-id="77187-182">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="77187-183">place (preview)</span><span class="sxs-lookup"><span data-stu-id="77187-183">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="77187-184">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="77187-184">Mail API resources</span></span>

- [<span data-ttu-id="77187-185">message</span><span class="sxs-lookup"><span data-stu-id="77187-185">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="77187-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="77187-186">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="77187-187">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="77187-187">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="77187-188">messageRule</span><span class="sxs-lookup"><span data-stu-id="77187-188">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="77187-189">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77187-189">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="77187-190">attachment</span><span class="sxs-lookup"><span data-stu-id="77187-190">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="77187-191">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="77187-191">Personal contacts API resources</span></span>

- [<span data-ttu-id="77187-192">contato</span><span class="sxs-lookup"><span data-stu-id="77187-192">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="77187-193">contactFolder</span><span class="sxs-lookup"><span data-stu-id="77187-193">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="77187-194">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77187-194">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="77187-195">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="77187-195">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="77187-196">person</span><span class="sxs-lookup"><span data-stu-id="77187-196">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="77187-197">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="77187-197">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="77187-198">outlookTask</span><span class="sxs-lookup"><span data-stu-id="77187-198">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="77187-199">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="77187-199">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="77187-200">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="77187-200">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="77187-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77187-201">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="77187-202">attachment</span><span class="sxs-lookup"><span data-stu-id="77187-202">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="77187-203">Limites dos serviços de comunicação em nuvem</span><span class="sxs-lookup"><span data-stu-id="77187-203">Cloud communication service limits</span></span>

| <span data-ttu-id="77187-204">Recurso</span><span class="sxs-lookup"><span data-stu-id="77187-204">Resource</span></span>      | <span data-ttu-id="77187-205">Limites por aplicativo e por inquilino</span><span class="sxs-lookup"><span data-stu-id="77187-205">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="77187-206">Chamadas</span><span class="sxs-lookup"><span data-stu-id="77187-206">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="77187-207">10.000 chamadas/mês e 100 chamadas simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-207">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="77187-208">Informações sobre a reunião </span><span class="sxs-lookup"><span data-stu-id="77187-208">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="77187-209">2000 reuniões/usuário a cada mês</span><span class="sxs-lookup"><span data-stu-id="77187-209">2000 meetings/user each month</span></span> |
| <span data-ttu-id="77187-210">[Presença](/graph/api/resources/presence) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="77187-210">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="77187-211">2 rps</span><span class="sxs-lookup"><span data-stu-id="77187-211">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="77187-212">Limites do serviço OneNote</span><span class="sxs-lookup"><span data-stu-id="77187-212">OneNote service limits</span></span>

| <span data-ttu-id="77187-213">Tipo de limite</span><span class="sxs-lookup"><span data-stu-id="77187-213">Limit type</span></span> | <span data-ttu-id="77187-214">Limitar por aplicativo por usuário (contexto delegado)</span><span class="sxs-lookup"><span data-stu-id="77187-214">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="77187-215">Limite por aplicativo (contexto somente de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="77187-215">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="77187-216">Taxa de solicitações</span><span class="sxs-lookup"><span data-stu-id="77187-216">Requests rate</span></span> | <span data-ttu-id="77187-217">120 solicitações por 1 minuto e 400 por 1 hora</span><span class="sxs-lookup"><span data-stu-id="77187-217">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="77187-218">240 solicitações por 1 minuto e 800 por 1 hora</span><span class="sxs-lookup"><span data-stu-id="77187-218">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="77187-219">Solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-219">Concurrent requests</span></span> | <span data-ttu-id="77187-220">5 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-220">5 concurrent requests</span></span> | <span data-ttu-id="77187-221">20 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-221">20 concurrent requests</span></span> |

<span data-ttu-id="77187-222">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-222">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77187-223">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="77187-223">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="77187-224">Você pode encontrar informações adicionais sobre as práticas recomendadas no [limitação da API do OneNote e como evitá-la](https://developer.microsoft.com/pt-BR/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span><span class="sxs-lookup"><span data-stu-id="77187-224">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/pt-BR/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="77187-225">**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="77187-225">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="77187-226">Limites de serviços do Project Rome</span><span class="sxs-lookup"><span data-stu-id="77187-226">Project Rome service limits</span></span>

| <span data-ttu-id="77187-227">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="77187-227">Request type</span></span> | <span data-ttu-id="77187-228">Limitar por usuário a todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="77187-228">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="77187-229">OBTER</span><span class="sxs-lookup"><span data-stu-id="77187-229">GET</span></span>          | <span data-ttu-id="77187-230">400 solicitações a cada 5 minutos e 12000 solicitações por dia</span><span class="sxs-lookup"><span data-stu-id="77187-230">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="77187-231">POSTAR, COLOCAR, CORRIGIR, EXCLUIR</span><span class="sxs-lookup"><span data-stu-id="77187-231">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="77187-232">100 solicitações a cada 5 minutos e 8000 solicitações por dia</span><span class="sxs-lookup"><span data-stu-id="77187-232">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="77187-233">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-233">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77187-234">activityHistoryItem, userActivity</span><span class="sxs-lookup"><span data-stu-id="77187-234">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="77187-235">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="77187-235">Microsoft Teams service limits</span></span>

<span data-ttu-id="77187-236">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="77187-236">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="77187-237">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="77187-237">Teams request type</span></span>                                   | <span data-ttu-id="77187-238">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="77187-238">Limit per app per tenant</span></span>        | <span data-ttu-id="77187-239">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="77187-239">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="77187-240">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="77187-240">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="77187-241">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="77187-241">15000 requests every 10 seconds</span></span> | <span data-ttu-id="77187-242">n/d</span><span class="sxs-lookup"><span data-stu-id="77187-242">n/a</span></span> |
| <span data-ttu-id="77187-243">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77187-243">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="77187-244">60 rps</span><span class="sxs-lookup"><span data-stu-id="77187-244">60 rps</span></span>                          | <span data-ttu-id="77187-245">600 rps</span><span class="sxs-lookup"><span data-stu-id="77187-245">600 rps</span></span> |
| <span data-ttu-id="77187-246">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77187-246">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="77187-247">30 rps</span><span class="sxs-lookup"><span data-stu-id="77187-247">30 rps</span></span>                         | <span data-ttu-id="77187-248">300 rps</span><span class="sxs-lookup"><span data-stu-id="77187-248">300 rps</span></span>  |
| <span data-ttu-id="77187-249">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77187-249">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="77187-250">30 rps</span><span class="sxs-lookup"><span data-stu-id="77187-250">30 rps</span></span>                         | <span data-ttu-id="77187-251">300 rps</span><span class="sxs-lookup"><span data-stu-id="77187-251">300 rps</span></span>  |
| <span data-ttu-id="77187-252">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77187-252">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="77187-253">15 rps</span><span class="sxs-lookup"><span data-stu-id="77187-253">15 rps</span></span>                         | <span data-ttu-id="77187-254">150 rps</span><span class="sxs-lookup"><span data-stu-id="77187-254">150 rps</span></span>  |
| <span data-ttu-id="77187-255">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="77187-255">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="77187-256">30 rps</span><span class="sxs-lookup"><span data-stu-id="77187-256">30 rps</span></span>                         | <span data-ttu-id="77187-257">300 rps</span><span class="sxs-lookup"><span data-stu-id="77187-257">300 rps</span></span>  |
| <span data-ttu-id="77187-258">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="77187-258">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="77187-259">6 rps</span><span class="sxs-lookup"><span data-stu-id="77187-259">6 rps</span></span> | <span data-ttu-id="77187-260">150 rps</span><span class="sxs-lookup"><span data-stu-id="77187-260">150 rps</span></span>  | 
| <span data-ttu-id="77187-261">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="77187-261">GET channel message</span></span>  | <span data-ttu-id="77187-262">5 rps</span><span class="sxs-lookup"><span data-stu-id="77187-262">5 rps</span></span> | <span data-ttu-id="77187-263">100 rps</span><span class="sxs-lookup"><span data-stu-id="77187-263">100 rps</span></span> |
| <span data-ttu-id="77187-264">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="77187-264">GET 1:1/group chat message</span></span>  | <span data-ttu-id="77187-265">3 rps</span><span class="sxs-lookup"><span data-stu-id="77187-265">3 rps</span></span> | <span data-ttu-id="77187-266">30 rps</span><span class="sxs-lookup"><span data-stu-id="77187-266">30 rps</span></span> |
| <span data-ttu-id="77187-267">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="77187-267">POST channel message</span></span> | <span data-ttu-id="77187-268">2 rps</span><span class="sxs-lookup"><span data-stu-id="77187-268">2 rps</span></span> | <span data-ttu-id="77187-269">20 rps</span><span class="sxs-lookup"><span data-stu-id="77187-269">20 rps</span></span> |
| <span data-ttu-id="77187-270">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="77187-270">POST 1:1/group chat message</span></span> | <span data-ttu-id="77187-271">2 rps</span><span class="sxs-lookup"><span data-stu-id="77187-271">2 rps</span></span> | <span data-ttu-id="77187-272">20 rps</span><span class="sxs-lookup"><span data-stu-id="77187-272">20 rps</span></span> |
| <span data-ttu-id="77187-273">OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="77187-273">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="77187-274">60 rps</span><span class="sxs-lookup"><span data-stu-id="77187-274">60 rps</span></span> | <span data-ttu-id="77187-275">600 rps</span><span class="sxs-lookup"><span data-stu-id="77187-275">600 rps</span></span> |
| <span data-ttu-id="77187-276">PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="77187-276">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="77187-277">30 rps</span><span class="sxs-lookup"><span data-stu-id="77187-277">30 rps</span></span> | <span data-ttu-id="77187-278">300 rps</span><span class="sxs-lookup"><span data-stu-id="77187-278">300 rps</span></span> |
| <span data-ttu-id="77187-279">APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="77187-279">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="77187-280">15 rps</span><span class="sxs-lookup"><span data-stu-id="77187-280">15 rps</span></span> | <span data-ttu-id="77187-281">150 rps</span><span class="sxs-lookup"><span data-stu-id="77187-281">150 rps</span></span> |

<span data-ttu-id="77187-282">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="77187-282">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="77187-283">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="77187-283">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="77187-284">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="77187-284">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

<span data-ttu-id="77187-285">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-285">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77187-286">aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.</span><span class="sxs-lookup"><span data-stu-id="77187-286">aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.</span></span>

### <a name="information-protection"></a><span data-ttu-id="77187-287">Proteção de informações</span><span class="sxs-lookup"><span data-stu-id="77187-287">Information protection</span></span>

<span data-ttu-id="77187-288">Os seguintes limites se aplicam a qualquer solicitação no `/informationProtection`.</span><span class="sxs-lookup"><span data-stu-id="77187-288">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="77187-289">Operation</span><span class="sxs-lookup"><span data-stu-id="77187-289">Operation</span></span>                 | <span data-ttu-id="77187-290">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="77187-290">Limit per tenant</span></span>                                            | <span data-ttu-id="77187-291">Limite por recurso (email, URL, arquivo)</span><span class="sxs-lookup"><span data-stu-id="77187-291">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="77187-292">POST</span><span class="sxs-lookup"><span data-stu-id="77187-292">POST</span></span>                      | <span data-ttu-id="77187-293">150 solicitações a cada 15 minutos e 10000 solicitações a cada 24 horas</span><span class="sxs-lookup"><span data-stu-id="77187-293">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="77187-294">1 solicitação a cada 15 minutos e 3 solicitações a cada 24 horas</span><span class="sxs-lookup"><span data-stu-id="77187-294">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="77187-295">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-295">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77187-296">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span><span class="sxs-lookup"><span data-stu-id="77187-296">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="77187-297">Proteção da identidade e limites do serviço de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="77187-297">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="77187-298">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="77187-298">Request type</span></span> | <span data-ttu-id="77187-299">Limitar por locatário para todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="77187-299">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="77187-300">Qualquer</span><span class="sxs-lookup"><span data-stu-id="77187-300">Any</span></span> | <span data-ttu-id="77187-301">1 solicitação por segundo</span><span class="sxs-lookup"><span data-stu-id="77187-301">1 request per second</span></span> |

<span data-ttu-id="77187-302">Os limites anteriores aplicam-se aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-302">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77187-303">Detecçãoderisco, Usuárioderisco, HistóricodeItemdeUsuárioderisco, NomedoLocal, paísNomedoLocal, ipNomedoLocal, PolíticadeAcessoCondicional.</span><span class="sxs-lookup"><span data-stu-id="77187-303">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="77187-304">**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="77187-304">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="77187-305">Percepção dos limites de serviço</span><span class="sxs-lookup"><span data-stu-id="77187-305">Insights service limits</span></span>

<span data-ttu-id="77187-306">Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="77187-306">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="77187-307">Limite</span><span class="sxs-lookup"><span data-stu-id="77187-307">Limit</span></span>                                                      | <span data-ttu-id="77187-308">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="77187-308">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="77187-309">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="77187-309">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="77187-310">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="77187-310">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="77187-311">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-311">4 concurrent requests</span></span>                                      | <span data-ttu-id="77187-312">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="77187-312">v1.0 and beta endpoints</span></span>   |

<span data-ttu-id="77187-313">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-313">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77187-314">pessoas, tendências, usedinsight, sharedInsight.</span><span class="sxs-lookup"><span data-stu-id="77187-314">people, trending, usedinsight, sharedInsight.</span></span>

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="77187-315">Limites do serviço de relatórios do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="77187-315">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="77187-316">Os seguintes limites se aplicam a qualquer solicitação no `/reports`.</span><span class="sxs-lookup"><span data-stu-id="77187-316">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="77187-317">Operation</span><span class="sxs-lookup"><span data-stu-id="77187-317">Operation</span></span>                 | <span data-ttu-id="77187-318">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="77187-318">Limit per app per tenant</span></span>     | <span data-ttu-id="77187-319">Limitar por locatário para todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="77187-319">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="77187-320">Qualquer pedido (CSV)</span><span class="sxs-lookup"><span data-stu-id="77187-320">Any request (CSV)</span></span>         | <span data-ttu-id="77187-321">14 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="77187-321">14 requests per 10 minutes</span></span>   | <span data-ttu-id="77187-322">40 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="77187-322">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="77187-323">Qualquer solicitação (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="77187-323">Any request (JSON, beta)</span></span>  | <span data-ttu-id="77187-324">100 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="77187-324">100 requests per 10 minutes</span></span>  | <span data-ttu-id="77187-325">n/d</span><span class="sxs-lookup"><span data-stu-id="77187-325">n/a</span></span>                        |

<span data-ttu-id="77187-326">Os limites anteriores aplicam-se individualmente a cada relatório de API.</span><span class="sxs-lookup"><span data-stu-id="77187-326">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="77187-327">Por exemplo, uma solicitação da API do relatório de atividades do usuário do Microsoft Teams e uma solicitação de relatório da API do usuário do Outlook dentro de 10 minutos contará como uma solicitação entre 14 para cada API e não duas solicitações entre 14 para ambas.</span><span class="sxs-lookup"><span data-stu-id="77187-327">For example, a request to the Microsoft Teams user activity report API and a request to the Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

<span data-ttu-id="77187-328">Os limites anteriores se aplicam aos seguintes recursos de **relatório**.</span><span class="sxs-lookup"><span data-stu-id="77187-328">The preceding limits apply to the **report** resource.</span></span>  

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="77187-329">Limites de serviço do gerenciador de convite</span><span class="sxs-lookup"><span data-stu-id="77187-329">Invitation manager service limits</span></span>

<span data-ttu-id="77187-330">Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="77187-330">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="77187-331">Operation</span><span class="sxs-lookup"><span data-stu-id="77187-331">Operation</span></span>                 | <span data-ttu-id="77187-332">Limitar por locatário para todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="77187-332">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="77187-333">Qualquer operação</span><span class="sxs-lookup"><span data-stu-id="77187-333">Any operation</span></span>             | <span data-ttu-id="77187-334">150 solicitações a cada 5 segundos</span><span class="sxs-lookup"><span data-stu-id="77187-334">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="77187-335">Limites de serviços de detecção de segurança e incidentes</span><span class="sxs-lookup"><span data-stu-id="77187-335">Security detections and incidents service limits</span></span>

<span data-ttu-id="77187-336">Os seguintes limites se aplicam a qualquer solicitação no `/security`.</span><span class="sxs-lookup"><span data-stu-id="77187-336">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="77187-337">Operation</span><span class="sxs-lookup"><span data-stu-id="77187-337">Operation</span></span>                  | <span data-ttu-id="77187-338">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="77187-338">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="77187-339">Qualquer operação em `alert`, `securityActions`,  `secureScore`</span><span class="sxs-lookup"><span data-stu-id="77187-339">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="77187-340">150 solicitações por minuto</span><span class="sxs-lookup"><span data-stu-id="77187-340">150 requests per minute</span></span>      |
| <span data-ttu-id="77187-341">Qualquer operação em `tiIndicator`</span><span class="sxs-lookup"><span data-stu-id="77187-341">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="77187-342">1000 solicitações por minuto</span><span class="sxs-lookup"><span data-stu-id="77187-342">1000 requests per minute</span></span> |
| <span data-ttu-id="77187-343">Qualquer operação em `secureScore` ou `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="77187-343">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="77187-344">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="77187-344">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="77187-345">Qualquer operação em `secureScore` ou `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="77187-345">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="77187-346">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="77187-346">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="77187-347">Limitações de serviços à extensões de esquema e abertas</span><span class="sxs-lookup"><span data-stu-id="77187-347">Open and schema extensions service limits</span></span>

| <span data-ttu-id="77187-348">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="77187-348">Request type</span></span> | <span data-ttu-id="77187-349">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="77187-349">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="77187-350">Qualquer</span><span class="sxs-lookup"><span data-stu-id="77187-350">Any</span></span>          | <span data-ttu-id="77187-351">455 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="77187-351">455 requests per 10 seconds</span></span> |

<span data-ttu-id="77187-352">Os limites acima se aplicam aos seguintes recursos: openTypeExtension, schemaExtension, administrativeUnit, contato, dispositivo, evento, grupo, mensagem, organização, postagem e usuário.</span><span class="sxs-lookup"><span data-stu-id="77187-352">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

### <a name="files-and-lists-service-limits"></a><span data-ttu-id="77187-353">Limites de serviço dos arquivos e listas</span><span class="sxs-lookup"><span data-stu-id="77187-353">Files and lists service limits</span></span>

<span data-ttu-id="77187-354">Os limites de serviço do OneDrive, OneDrive for Business e SharePoint Online não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="77187-354">Service limits for OneDrive, OneDrive for Business, and SharePoint Online are not available.</span></span> <span data-ttu-id="77187-355">Para mais informações, confira [Por que não é possível saber o limites exatos?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span><span class="sxs-lookup"><span data-stu-id="77187-355">For more information, see [why can't you just tell me the exact throttling limits?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span></span>

<span data-ttu-id="77187-356">As informações anteriores aplicam-se aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-356">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="77187-357">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, List, listItem, listItemVersion, permission, sharedDriveItem, site e thumbnailSet.</span><span class="sxs-lookup"><span data-stu-id="77187-357">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site, and thumbnailSet.</span></span>

### <a name="tasks-and-plans-service-limits"></a><span data-ttu-id="77187-358">Limites de serviços de tarefas e planos</span><span class="sxs-lookup"><span data-stu-id="77187-358">Tasks and plans service limits</span></span>

<span data-ttu-id="77187-359">Os limites de serviço do Planner não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="77187-359">Service limits for Planner are not available.</span></span>

<span data-ttu-id="77187-360">As informações anteriores aplicam-se aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="77187-360">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="77187-361">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, e plannerUser.</span><span class="sxs-lookup"><span data-stu-id="77187-361">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, and plannerUser.</span></span>

### <a name="identity-and-access-data-policy-operation-service-limits"></a><span data-ttu-id="77187-362">Limites de operação de serviços de política de dados de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="77187-362">Identity and access data policy operation service limits</span></span>

| <span data-ttu-id="77187-363">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="77187-363">Request type</span></span> | <span data-ttu-id="77187-364">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="77187-364">Limit per tenant</span></span> |
| ------------ | ---------------- |
| <span data-ttu-id="77187-365">Postar no `exportPersonalData`</span><span class="sxs-lookup"><span data-stu-id="77187-365">POST on `exportPersonalData`</span></span> | <span data-ttu-id="77187-366">1.000 solicitações por dia para todos os assuntos e 100 por assunto por dia</span><span class="sxs-lookup"><span data-stu-id="77187-366">1000 requests per day for any subject and 100 per subject per day</span></span> |
| <span data-ttu-id="77187-367">Qualquer outra solicitação</span><span class="sxs-lookup"><span data-stu-id="77187-367">Any other request</span></span> | <span data-ttu-id="77187-368">10.000 solicitações por minuto</span><span class="sxs-lookup"><span data-stu-id="77187-368">10000 requests per hour</span></span> |

<span data-ttu-id="77187-369">Os limites anteriores se aplicam aos seguintes recursos: dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="77187-369">The preceding limits apply to the following resources: dataPolicyOperation.</span></span>

> <span data-ttu-id="77187-370">**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` nas respostas `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="77187-370">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="77187-371">Limites do serviço de Educação</span><span class="sxs-lookup"><span data-stu-id="77187-371">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="77187-372">Limites de serviço do Excel</span><span class="sxs-lookup"><span data-stu-id="77187-372">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="77187-373">Limites do serviço de registros de auditoria de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="77187-373">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="77187-374">Limites de serviço dos fornecedores de identidade</span><span class="sxs-lookup"><span data-stu-id="77187-374">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="77187-375">Limites de serviço Intune</span><span class="sxs-lookup"><span data-stu-id="77187-375">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="77187-376">Limites do serviço Skype</span><span class="sxs-lookup"><span data-stu-id="77187-376">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="77187-377">Limites do serviço de assinatura</span><span class="sxs-lookup"><span data-stu-id="77187-377">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
