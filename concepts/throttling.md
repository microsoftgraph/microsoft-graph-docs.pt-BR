---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: a62b88927f33b12f9e9738f8b8ba299a22f6d099
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197062"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="5f3d8-105">Diretrizes de limitação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5f3d8-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="5f3d8-p102">Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="5f3d8-p103">Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="5f3d8-111">O que acontece quando a limitação ocorre?</span><span class="sxs-lookup"><span data-stu-id="5f3d8-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="5f3d8-p104">Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="5f3d8-119">Cenários comuns de limitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-119">Common throttling scenarios</span></span>

<span data-ttu-id="5f3d8-120">As causas mais comuns de limitação dos clientes incluem:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="5f3d8-121">Um grande número de solicitações em todos os aplicativos em um locatário.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="5f3d8-122">Um grande número de solicitações de um aplicativo específico entre todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="5f3d8-123">Práticas recomendadas para lidar com a limitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-123">Best practices to handle throttling</span></span>

<span data-ttu-id="5f3d8-124">Estas são as práticas recomendadas para lidar com a limitação:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="5f3d8-125">Reduza o número de operações por solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="5f3d8-126">Reduza a frequência de chamadas.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="5f3d8-127">Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="5f3d8-p105">Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="5f3d8-131">Aguarde o número de segundos especificado no cabeçalho `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="5f3d8-132">Repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-132">Retry the request.</span></span>
3. <span data-ttu-id="5f3d8-p106">Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="5f3d8-135">Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="5f3d8-136">Usuário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-137">Foto</span><span class="sxs-lookup"><span data-stu-id="5f3d8-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-138">Email</span><span class="sxs-lookup"><span data-stu-id="5f3d8-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-139">Calendário (usuários e grupos)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-140">Contato</span><span class="sxs-lookup"><span data-stu-id="5f3d8-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-141">Anexo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-142">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-143">Pessoas e social</span><span class="sxs-lookup"><span data-stu-id="5f3d8-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="5f3d8-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="5f3d8-145">Item externo (Pesquisa da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="5f3d8-146">Relatório</span><span class="sxs-lookup"><span data-stu-id="5f3d8-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="5f3d8-147">Assinatura</span><span class="sxs-lookup"><span data-stu-id="5f3d8-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="5f3d8-148">Solicitação de avaliação de ameaças</span><span class="sxs-lookup"><span data-stu-id="5f3d8-148">Threat assessment request</span></span>](/graph/api/resources/threatassessmentrequest)
- [<span data-ttu-id="5f3d8-149">Solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="5f3d8-149">Mail assessment request</span></span>](/graph/api/resources/mailassessmentrequest)
- [<span data-ttu-id="5f3d8-150">Solicitação de avaliação de arquivo de email</span><span class="sxs-lookup"><span data-stu-id="5f3d8-150">Email file assessment request</span></span>](/graph/api/resources/emailfileassessmentrequest)
- [<span data-ttu-id="5f3d8-151">Solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-151">File assessment request</span></span>](/graph/api/resources/fileassessmentrequest)
- [<span data-ttu-id="5f3d8-152">Solicitação de avaliação de URL</span><span class="sxs-lookup"><span data-stu-id="5f3d8-152">URL assessment request</span></span>](/graph/api/resources/urlassessmentrequest)
- [<span data-ttu-id="5f3d8-153">Resultado da avaliação de ameaças</span><span class="sxs-lookup"><span data-stu-id="5f3d8-153">Threat assessment result</span></span>](/graph/api/resources/threatassessmentresult)
- [<span data-ttu-id="5f3d8-154">Tendência</span><span class="sxs-lookup"><span data-stu-id="5f3d8-154">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="5f3d8-155">Percepção utilizada</span><span class="sxs-lookup"><span data-stu-id="5f3d8-155">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="5f3d8-156">Percepção compartilhada</span><span class="sxs-lookup"><span data-stu-id="5f3d8-156">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="5f3d8-157">Configurações do usuário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-157">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="5f3d8-158">Convite</span><span class="sxs-lookup"><span data-stu-id="5f3d8-158">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="5f3d8-159">Para uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-159">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="5f3d8-160">Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-160">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="5f3d8-161">Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-161">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="5f3d8-162">Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-162">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="5f3d8-163">Práticas recomendadas para evitar a limitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-163">Best practices to avoid throttling</span></span>

<span data-ttu-id="5f3d8-164">Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-164">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="5f3d8-165">Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-165">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="5f3d8-166">[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-166">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="5f3d8-167">Limites específicos do serviço</span><span class="sxs-lookup"><span data-stu-id="5f3d8-167">Service-specific limits</span></span>

<span data-ttu-id="5f3d8-168">O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-168">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="5f3d8-169">Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-169">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="5f3d8-170">Qualquer solicitação poderá ser avaliada em relação a vários limites, dependendo do escopo do limite (por aplicativo em todos os locatários, por locatário para todos os aplicativos, por aplicativo por locatário, e assim por diante), do tipo de solicitação (GET, POST, PATCH e assim por diante) e de outros fatores.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-170">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="5f3d8-171">O primeiro limite a ser alcançado dispara o comportamento de limitação.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-171">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="5f3d8-172">Além dos limites de serviço específicos descritos na seção, os seguintes limites globais se aplicam:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-172">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="5f3d8-173">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-173">Request type</span></span> | <span data-ttu-id="5f3d8-174">Por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="5f3d8-174">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="5f3d8-175">Qualquer</span><span class="sxs-lookup"><span data-stu-id="5f3d8-175">Any</span></span>          | <span data-ttu-id="5f3d8-176">2000 solicitações por segundo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-176">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="5f3d8-177">Os limites específicos descritos aqui estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-177">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="5f3d8-178">**Nota:** Nesta seção, o termo *locatário* refere-se à organização Microsoft 365 onde o aplicativo está instalado.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-178">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="5f3d8-179">Este inquilino pode ser o mesmo onde o aplicativo foi criado, no caso de um único aplicativo de inquilino, ou pode ser diferente, no caso de [um aplicativo de vários inquilinos](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-179">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="5f3d8-180">Limites de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="5f3d8-180">Outlook service limits</span></span>

<span data-ttu-id="5f3d8-181">Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-181">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="5f3d8-182">Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-182">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="5f3d8-183">Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-183">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="5f3d8-184">Os seguintes limites se aplicam à nuvem pública, bem como às [ implementações de nuvens nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-184">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="5f3d8-185">Limite</span><span class="sxs-lookup"><span data-stu-id="5f3d8-185">Limit</span></span>                                                      | <span data-ttu-id="5f3d8-186">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="5f3d8-186">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="5f3d8-187">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-187">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="5f3d8-188">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="5f3d8-188">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="5f3d8-189">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-189">4 concurrent requests</span></span>                                      | <span data-ttu-id="5f3d8-190">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="5f3d8-190">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="5f3d8-191">15 megabytes (MB) de upload (PATCH, POST, PUT) em um período de 30 segundos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-191">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="5f3d8-192">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="5f3d8-192">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="5f3d8-193">Recursos de serviço do Outlook</span><span class="sxs-lookup"><span data-stu-id="5f3d8-193">Outlook service resources</span></span>

<span data-ttu-id="5f3d8-194">Os recursos a seguir são fornecidos pelo serviço do Outlook.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-194">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="5f3d8-195">Recursos da API do calendário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-195">Calendar API resources</span></span>

- [<span data-ttu-id="5f3d8-196">event</span><span class="sxs-lookup"><span data-stu-id="5f3d8-196">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="5f3d8-197">eventMessage</span><span class="sxs-lookup"><span data-stu-id="5f3d8-197">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="5f3d8-198">calendar</span><span class="sxs-lookup"><span data-stu-id="5f3d8-198">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="5f3d8-199">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="5f3d8-199">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="5f3d8-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="5f3d8-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="5f3d8-201">attachment</span><span class="sxs-lookup"><span data-stu-id="5f3d8-201">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="5f3d8-202">place (preview)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-202">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="5f3d8-203">Recursos da API do email</span><span class="sxs-lookup"><span data-stu-id="5f3d8-203">Mail API resources</span></span>

- [<span data-ttu-id="5f3d8-204">message</span><span class="sxs-lookup"><span data-stu-id="5f3d8-204">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="5f3d8-205">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5f3d8-205">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="5f3d8-206">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5f3d8-206">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="5f3d8-207">messageRule</span><span class="sxs-lookup"><span data-stu-id="5f3d8-207">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="5f3d8-208">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="5f3d8-208">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="5f3d8-209">attachment</span><span class="sxs-lookup"><span data-stu-id="5f3d8-209">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="5f3d8-210">Recursos da API de contatos pessoais</span><span class="sxs-lookup"><span data-stu-id="5f3d8-210">Personal contacts API resources</span></span>

- [<span data-ttu-id="5f3d8-211">contato</span><span class="sxs-lookup"><span data-stu-id="5f3d8-211">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="5f3d8-212">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5f3d8-212">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="5f3d8-213">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="5f3d8-213">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="5f3d8-214">Recursos da inteligência social e do local de trabalho </span><span class="sxs-lookup"><span data-stu-id="5f3d8-214">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="5f3d8-215">person</span><span class="sxs-lookup"><span data-stu-id="5f3d8-215">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="5f3d8-216">Recursos da API de tarefas pendentes (visualização)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-216">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="5f3d8-217">outlookTask</span><span class="sxs-lookup"><span data-stu-id="5f3d8-217">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="5f3d8-218">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="5f3d8-218">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="5f3d8-219">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="5f3d8-219">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="5f3d8-220">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="5f3d8-220">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="5f3d8-221">attachment</span><span class="sxs-lookup"><span data-stu-id="5f3d8-221">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="5f3d8-222">Limites dos serviços de comunicação em nuvem</span><span class="sxs-lookup"><span data-stu-id="5f3d8-222">Cloud communication service limits</span></span>

| <span data-ttu-id="5f3d8-223">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3d8-223">Resource</span></span>      | <span data-ttu-id="5f3d8-224">Limites por aplicativo e por inquilino</span><span class="sxs-lookup"><span data-stu-id="5f3d8-224">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="5f3d8-225">Chamadas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-225">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="5f3d8-226">10.000 chamadas/mês e 100 chamadas simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-226">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="5f3d8-227">Informações sobre a reunião </span><span class="sxs-lookup"><span data-stu-id="5f3d8-227">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="5f3d8-228">2000 reuniões/usuário a cada mês</span><span class="sxs-lookup"><span data-stu-id="5f3d8-228">2000 meetings/user each month</span></span> |
| <span data-ttu-id="5f3d8-229">[Presença](/graph/api/resources/presence) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-229">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="5f3d8-230">2 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-230">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="5f3d8-231">Limites do serviço OneNote</span><span class="sxs-lookup"><span data-stu-id="5f3d8-231">OneNote service limits</span></span>

| <span data-ttu-id="5f3d8-232">Tipo de limite</span><span class="sxs-lookup"><span data-stu-id="5f3d8-232">Limit type</span></span> | <span data-ttu-id="5f3d8-233">Limitar por aplicativo por usuário (contexto delegado)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-233">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="5f3d8-234">Limite por aplicativo (contexto somente de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-234">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="5f3d8-235">Taxa de solicitações</span><span class="sxs-lookup"><span data-stu-id="5f3d8-235">Requests rate</span></span> | <span data-ttu-id="5f3d8-236">120 solicitações por 1 minuto e 400 por 1 hora</span><span class="sxs-lookup"><span data-stu-id="5f3d8-236">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="5f3d8-237">240 solicitações por 1 minuto e 800 por 1 hora</span><span class="sxs-lookup"><span data-stu-id="5f3d8-237">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="5f3d8-238">Solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-238">Concurrent requests</span></span> | <span data-ttu-id="5f3d8-239">5 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-239">5 concurrent requests</span></span> | <span data-ttu-id="5f3d8-240">20 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-240">20 concurrent requests</span></span> |

<span data-ttu-id="5f3d8-241">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-241">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="5f3d8-242">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="5f3d8-242">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="5f3d8-243">Você pode encontrar informações adicionais sobre as práticas recomendadas no [limitação da API do OneNote e como evitá-la](https://developer.microsoft.com/pt-BR/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-243">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/pt-BR/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="5f3d8-244">**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-244">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="5f3d8-245">Limites de serviços do Project Rome</span><span class="sxs-lookup"><span data-stu-id="5f3d8-245">Project Rome service limits</span></span>

| <span data-ttu-id="5f3d8-246">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-246">Request type</span></span> | <span data-ttu-id="5f3d8-247">Limitar por usuário a todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-247">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="5f3d8-248">OBTER</span><span class="sxs-lookup"><span data-stu-id="5f3d8-248">GET</span></span>          | <span data-ttu-id="5f3d8-249">400 solicitações a cada 5 minutos e 12000 solicitações por dia</span><span class="sxs-lookup"><span data-stu-id="5f3d8-249">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="5f3d8-250">POSTAR, COLOCAR, CORRIGIR, EXCLUIR</span><span class="sxs-lookup"><span data-stu-id="5f3d8-250">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="5f3d8-251">100 solicitações a cada 5 minutos e 8000 solicitações por dia</span><span class="sxs-lookup"><span data-stu-id="5f3d8-251">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="5f3d8-252">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-252">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="5f3d8-253">activityHistoryItem, userActivity</span><span class="sxs-lookup"><span data-stu-id="5f3d8-253">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="5f3d8-254">Limites do serviço do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5f3d8-254">Microsoft Teams service limits</span></span>

<span data-ttu-id="5f3d8-255">Os limites são expressos como solicitações por segundo (rps).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-255">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="5f3d8-256">Tipo de solicitação do Teams</span><span class="sxs-lookup"><span data-stu-id="5f3d8-256">Teams request type</span></span>                                   | <span data-ttu-id="5f3d8-257">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-257">Limit per app per tenant</span></span>        | <span data-ttu-id="5f3d8-258">Limitar por aplicativo em todos os locatários</span><span class="sxs-lookup"><span data-stu-id="5f3d8-258">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="5f3d8-259">Todas as chamadas de API do Graph para o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5f3d8-259">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="5f3d8-260">15000 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-260">15000 requests every 10 seconds</span></span> | <span data-ttu-id="5f3d8-261">n/d</span><span class="sxs-lookup"><span data-stu-id="5f3d8-261">n/a</span></span> |
| <span data-ttu-id="5f3d8-262">OBTER equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="5f3d8-262">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="5f3d8-263">60 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-263">60 rps</span></span>                          | <span data-ttu-id="5f3d8-264">600 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-264">600 rps</span></span> |
| <span data-ttu-id="5f3d8-265">Canal POST/PUT, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="5f3d8-265">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="5f3d8-266">30 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-266">30 rps</span></span>                         | <span data-ttu-id="5f3d8-267">300 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-267">300 rps</span></span>  |
| <span data-ttu-id="5f3d8-268">PATCH da equipe, canal, guia, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="5f3d8-268">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="5f3d8-269">30 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-269">30 rps</span></span>                         | <span data-ttu-id="5f3d8-270">300 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-270">300 rps</span></span>  |
| <span data-ttu-id="5f3d8-271">EXCLUIR canal, Tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="5f3d8-271">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="5f3d8-272">15 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-272">15 rps</span></span>                         | <span data-ttu-id="5f3d8-273">150 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-273">150 rps</span></span>  |
| <span data-ttu-id="5f3d8-274">OBTER /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="5f3d8-274">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="5f3d8-275">30 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-275">30 rps</span></span>                         | <span data-ttu-id="5f3d8-276">300 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-276">300 rps</span></span>  |
| <span data-ttu-id="5f3d8-277">POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="5f3d8-277">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="5f3d8-278">6 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-278">6 rps</span></span> | <span data-ttu-id="5f3d8-279">150 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-279">150 rps</span></span>  | 
| <span data-ttu-id="5f3d8-280">OBTER mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="5f3d8-280">GET channel message</span></span>  | <span data-ttu-id="5f3d8-281">5 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-281">5 rps</span></span> | <span data-ttu-id="5f3d8-282">100 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-282">100 rps</span></span> |
| <span data-ttu-id="5f3d8-283">OBTER 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-283">GET 1:1/group chat message</span></span>  | <span data-ttu-id="5f3d8-284">3 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-284">3 rps</span></span> | <span data-ttu-id="5f3d8-285">30 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-285">30 rps</span></span> |
| <span data-ttu-id="5f3d8-286">POSTAR mensagem do canal</span><span class="sxs-lookup"><span data-stu-id="5f3d8-286">POST channel message</span></span> | <span data-ttu-id="5f3d8-287">2 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-287">2 rps</span></span> | <span data-ttu-id="5f3d8-288">20 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-288">20 rps</span></span> |
| <span data-ttu-id="5f3d8-289">POSTAR 1:1/mensagem de chat do grupo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-289">POST 1:1/group chat message</span></span> | <span data-ttu-id="5f3d8-290">2 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-290">2 rps</span></span> | <span data-ttu-id="5f3d8-291">20 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-291">20 rps</span></span> |
| <span data-ttu-id="5f3d8-292">OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="5f3d8-292">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="5f3d8-293">60 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-293">60 rps</span></span> | <span data-ttu-id="5f3d8-294">600 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-294">600 rps</span></span> |
| <span data-ttu-id="5f3d8-295">PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="5f3d8-295">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="5f3d8-296">30 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-296">30 rps</span></span> | <span data-ttu-id="5f3d8-297">300 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-297">300 rps</span></span> |
| <span data-ttu-id="5f3d8-298">APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho</span><span class="sxs-lookup"><span data-stu-id="5f3d8-298">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="5f3d8-299">15 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-299">15 rps</span></span> | <span data-ttu-id="5f3d8-300">150 rps</span><span class="sxs-lookup"><span data-stu-id="5f3d8-300">150 rps</span></span> |

<span data-ttu-id="5f3d8-301">É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-301">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="5f3d8-302">Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-302">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="5f3d8-303">Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="5f3d8-303">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="information-protection"></a><span data-ttu-id="5f3d8-304">Proteção de informações</span><span class="sxs-lookup"><span data-stu-id="5f3d8-304">Information protection</span></span>

<span data-ttu-id="5f3d8-305">Os seguintes limites se aplicam a qualquer solicitação no `/informationProtection`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-305">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="5f3d8-306">Operation</span><span class="sxs-lookup"><span data-stu-id="5f3d8-306">Operation</span></span>                 | <span data-ttu-id="5f3d8-307">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="5f3d8-307">Limit per tenant</span></span>                                            | <span data-ttu-id="5f3d8-308">Limite por recurso (email, URL, arquivo)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-308">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="5f3d8-309">POST</span><span class="sxs-lookup"><span data-stu-id="5f3d8-309">POST</span></span>                      | <span data-ttu-id="5f3d8-310">150 solicitações a cada 15 minutos e 10000 solicitações a cada 24 horas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-310">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="5f3d8-311">1 solicitação a cada 15 minutos e 3 solicitações a cada 24 horas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-311">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="5f3d8-312">Os limites anteriores se aplicam aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-312">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="5f3d8-313">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-313">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="5f3d8-314">Proteção da identidade e limites do serviço de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="5f3d8-314">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="5f3d8-315">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-315">Request type</span></span> | <span data-ttu-id="5f3d8-316">Limitar por locatário para todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-316">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="5f3d8-317">Qualquer</span><span class="sxs-lookup"><span data-stu-id="5f3d8-317">Any</span></span> | <span data-ttu-id="5f3d8-318">1 solicitação por segundo</span><span class="sxs-lookup"><span data-stu-id="5f3d8-318">1 request per second</span></span> |

<span data-ttu-id="5f3d8-319">Os limites anteriores aplicam-se aos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="5f3d8-319">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="5f3d8-320">Detecçãoderisco, Usuárioderisco, HistóricodeItemdeUsuárioderisco, NomedoLocal, paísNomedoLocal, ipNomedoLocal, PolíticadeAcessoCondicional.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-320">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="5f3d8-321">**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-321">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="5f3d8-322">Percepção dos limites de serviço</span><span class="sxs-lookup"><span data-stu-id="5f3d8-322">Insights service limits</span></span>

<span data-ttu-id="5f3d8-323">Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-323">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="5f3d8-324">Limite</span><span class="sxs-lookup"><span data-stu-id="5f3d8-324">Limit</span></span>                                                      | <span data-ttu-id="5f3d8-325">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="5f3d8-325">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="5f3d8-326">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-326">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="5f3d8-327">pontos de extremidade v1.0 e beta</span><span class="sxs-lookup"><span data-stu-id="5f3d8-327">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="5f3d8-328">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-328">4 concurrent requests</span></span>                                      | <span data-ttu-id="5f3d8-329">v1.0 e pontos finais beta</span><span class="sxs-lookup"><span data-stu-id="5f3d8-329">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="5f3d8-330">Limites do serviço de relatórios do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5f3d8-330">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="5f3d8-331">Os seguintes limites se aplicam a qualquer solicitação no `/reports`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-331">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="5f3d8-332">Operation</span><span class="sxs-lookup"><span data-stu-id="5f3d8-332">Operation</span></span>                 | <span data-ttu-id="5f3d8-333">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-333">Limit per app per tenant</span></span>     | <span data-ttu-id="5f3d8-334">Limitar por locatário para todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-334">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="5f3d8-335">Qualquer pedido (CSV)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-335">Any request (CSV)</span></span>         | <span data-ttu-id="5f3d8-336">14 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-336">14 requests per 10 minutes</span></span>   | <span data-ttu-id="5f3d8-337">40 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-337">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="5f3d8-338">Qualquer solicitação (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="5f3d8-338">Any request (JSON, beta)</span></span>  | <span data-ttu-id="5f3d8-339">100 solicitações a cada 10 minutos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-339">100 requests per 10 minutes</span></span>  | <span data-ttu-id="5f3d8-340">n/d</span><span class="sxs-lookup"><span data-stu-id="5f3d8-340">n/a</span></span>                        |

<span data-ttu-id="5f3d8-341">Os limites anteriores aplicam-se individualmente a cada relatório de API.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-341">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="5f3d8-342">Por exemplo, uma solicitação de relatório da API do usuário da Microsoft Teams e uma solicitação de relatório da API do usuário do Outlook dentro de 10 minutos contará como 1 solicitação de 14 para cada API e não 2 solicitações de 14 para ambas.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-342">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="5f3d8-343">Limites de serviço do gerenciador de convite</span><span class="sxs-lookup"><span data-stu-id="5f3d8-343">Invitation manager service limits</span></span>

<span data-ttu-id="5f3d8-344">Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-344">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="5f3d8-345">Operation</span><span class="sxs-lookup"><span data-stu-id="5f3d8-345">Operation</span></span>                 | <span data-ttu-id="5f3d8-346">Limitar por locatário para todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-346">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="5f3d8-347">Qualquer operação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-347">Any operation</span></span>             | <span data-ttu-id="5f3d8-348">150 solicitações a cada 5 segundos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-348">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="5f3d8-349">Limites de serviços de detecção de segurança e incidentes</span><span class="sxs-lookup"><span data-stu-id="5f3d8-349">Security detections and incidents service limits</span></span>

<span data-ttu-id="5f3d8-350">Os seguintes limites se aplicam a qualquer solicitação no `/security`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-350">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="5f3d8-351">Operation</span><span class="sxs-lookup"><span data-stu-id="5f3d8-351">Operation</span></span>                  | <span data-ttu-id="5f3d8-352">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-352">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="5f3d8-353">Qualquer operação em `alert`, `securityActions`,  `secureScore`</span><span class="sxs-lookup"><span data-stu-id="5f3d8-353">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="5f3d8-354">150 solicitações por minuto</span><span class="sxs-lookup"><span data-stu-id="5f3d8-354">150 requests per minute</span></span>      |
| <span data-ttu-id="5f3d8-355">Qualquer operação em `tiIndicator`</span><span class="sxs-lookup"><span data-stu-id="5f3d8-355">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="5f3d8-356">1000 solicitações por minuto</span><span class="sxs-lookup"><span data-stu-id="5f3d8-356">1000 requests per minute</span></span> |
| <span data-ttu-id="5f3d8-357">Qualquer operação em `secureScore` ou `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="5f3d8-357">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="5f3d8-358">10.000 solicitações de API em um período de 10 minutos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-358">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="5f3d8-359">Qualquer operação em `secureScore` ou `secureScorecontrolProfile`</span><span class="sxs-lookup"><span data-stu-id="5f3d8-359">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="5f3d8-360">4 solicitações simultâneas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-360">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="5f3d8-361">Limitações de serviços à extensões de esquema e abertas</span><span class="sxs-lookup"><span data-stu-id="5f3d8-361">Open and schema extensions service limits</span></span>

| <span data-ttu-id="5f3d8-362">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-362">Request type</span></span> | <span data-ttu-id="5f3d8-363">Limitar por aplicativo por locatário</span><span class="sxs-lookup"><span data-stu-id="5f3d8-363">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="5f3d8-364">Qualquer</span><span class="sxs-lookup"><span data-stu-id="5f3d8-364">Any</span></span>          | <span data-ttu-id="5f3d8-365">455 solicitações a cada 10 segundos</span><span class="sxs-lookup"><span data-stu-id="5f3d8-365">455 requests per 10 seconds</span></span> |

<span data-ttu-id="5f3d8-366">Os limites acima se aplicam aos seguintes recursos: openTypeExtension, schemaExtension, administrativeUnit, contato, dispositivo, evento, grupo, mensagem, organização, postagem e usuário.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-366">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

### <a name="identity-and-access-data-policy-operation-service-limits"></a><span data-ttu-id="5f3d8-367">Limites de operação de serviços de política de dados de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="5f3d8-367">Identity and access data policy operation service limits</span></span>

| <span data-ttu-id="5f3d8-368">Tipo de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-368">Request type</span></span> | <span data-ttu-id="5f3d8-369">Limite por inquilino</span><span class="sxs-lookup"><span data-stu-id="5f3d8-369">Limit per tenant</span></span> |
| ------------ | ---------------- |
| <span data-ttu-id="5f3d8-370">Postar no `exportPersonalData`</span><span class="sxs-lookup"><span data-stu-id="5f3d8-370">POST on `exportPersonalData`</span></span> | <span data-ttu-id="5f3d8-371">1.000 solicitações por dia para todos os assuntos e 100 por assunto por dia</span><span class="sxs-lookup"><span data-stu-id="5f3d8-371">1000 requests per day for any subject and 100 per subject per day</span></span> |
| <span data-ttu-id="5f3d8-372">Qualquer outra solicitação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-372">Any other request</span></span> | <span data-ttu-id="5f3d8-373">10.000 solicitações por minuto</span><span class="sxs-lookup"><span data-stu-id="5f3d8-373">10000 requests per hour</span></span> |

<span data-ttu-id="5f3d8-374">Os limites anteriores se aplicam aos seguintes recursos: dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-374">The preceding limits apply to the following resources: dataPolicyOperation.</span></span>

> <span data-ttu-id="5f3d8-375">**Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` nas respostas `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="5f3d8-375">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="5f3d8-376">Limites do serviço de Educação</span><span class="sxs-lookup"><span data-stu-id="5f3d8-376">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="5f3d8-377">Limites de serviço do Excel</span><span class="sxs-lookup"><span data-stu-id="5f3d8-377">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="5f3d8-378">Limites do serviço de registros de auditoria de identidade e acesso</span><span class="sxs-lookup"><span data-stu-id="5f3d8-378">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="5f3d8-379">Limites de serviço dos fornecedores de identidade</span><span class="sxs-lookup"><span data-stu-id="5f3d8-379">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="5f3d8-380">Limites de serviço Intune</span><span class="sxs-lookup"><span data-stu-id="5f3d8-380">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="5f3d8-381">Limites do serviço Skype</span><span class="sxs-lookup"><span data-stu-id="5f3d8-381">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="5f3d8-382">Limites do serviço de assinatura</span><span class="sxs-lookup"><span data-stu-id="5f3d8-382">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
