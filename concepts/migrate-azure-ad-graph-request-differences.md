---
title: Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph
description: Descreve como as solicitações do Microsoft Graph são diferentes das solicitações do Azure AD, o que ajuda a migrar aplicativos para o serviço mais recente..
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8130daf4037e6ef1a433ca537a8fecec996a34ce
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845905"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="342c7-103">Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="342c7-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="342c7-104">Este artigo faz parte da *etapa 1: revisar as diferenças de API* do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="342c7-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="342c7-105">O Microsoft Graph e a API do Azure AD Graph são APIs REST e cada uma suportam convenções ODATA para parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="342c7-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="342c7-106">No entanto, a sintaxe varia entre essas duas APIs.</span><span class="sxs-lookup"><span data-stu-id="342c7-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="342c7-107">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar esses padrões de solicitação em seus próprios dados, pois é uma ótima maneira de aprender sobre as diferenças de solicitação e resposta.</span><span class="sxs-lookup"><span data-stu-id="342c7-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="342c7-108">Solicitações básicas</span><span class="sxs-lookup"><span data-stu-id="342c7-108">Basic requests</span></span>

<span data-ttu-id="342c7-109">A tabela a seguir realça as principais diferenças de solicitação entre as duas APIs:</span><span class="sxs-lookup"><span data-stu-id="342c7-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="342c7-110">Detalhes da solicitação</span><span class="sxs-lookup"><span data-stu-id="342c7-110">Request details</span></span>| <span data-ttu-id="342c7-111">Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-111">Azure AD Graph</span></span> | <span data-ttu-id="342c7-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="342c7-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="342c7-113">Sintaxe de solicitação</span><span class="sxs-lookup"><span data-stu-id="342c7-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="342c7-114">Pontos de extremidade de serviço &nbsp; :</span><span class="sxs-lookup"><span data-stu-id="342c7-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="342c7-115">-&nbsp;Global</span><span class="sxs-lookup"><span data-stu-id="342c7-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="342c7-116">-&nbsp;&nbsp;L4 gov (EUA) &nbsp;</span><span class="sxs-lookup"><span data-stu-id="342c7-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="342c7-117">-&nbsp;&nbsp; &nbsp; &nbsp; (DoD) de US gov</span><span class="sxs-lookup"><span data-stu-id="342c7-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="342c7-118">-&nbsp;Alemanha</span><span class="sxs-lookup"><span data-stu-id="342c7-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="342c7-119">-&nbsp;China &nbsp; (21vianet)</span><span class="sxs-lookup"><span data-stu-id="342c7-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="342c7-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="342c7-120">{tenant_id}</span></span>|<span data-ttu-id="342c7-121">Especifique a ID do locatário na solicitação.</span><span class="sxs-lookup"><span data-stu-id="342c7-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="342c7-122">É opcional especificar uma ID de locatário na solicitação, pois ela é inferida do token de acesso.</span><span class="sxs-lookup"><span data-stu-id="342c7-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="342c7-123">Se você especificar a ID do locatário, ela vai entre o `{version}` e o `{resource}` na URL da solicitação.</span><span class="sxs-lookup"><span data-stu-id="342c7-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="342c7-124">Version</span><span class="sxs-lookup"><span data-stu-id="342c7-124">{version}</span></span>|<span data-ttu-id="342c7-125">Especifique a versão de lançamento do Graph do Azure AD na solicitação usando um parâmetro de consulta necessário.</span><span class="sxs-lookup"><span data-stu-id="342c7-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="342c7-126">Especifique a versão de lançamento do Microsoft Graph na solicitação como parte do caminho da URL imediatamente após o ponto de extremidade do serviço.</span><span class="sxs-lookup"><span data-stu-id="342c7-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="342c7-127">Você pode continuar a usar os mesmos parâmetros de consulta no Microsoft Graph como o Graph do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="342c7-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="342c7-128">Exemplo de comparação de solicitação</span><span class="sxs-lookup"><span data-stu-id="342c7-128">Example request comparison</span></span>

<span data-ttu-id="342c7-129">Suponha que você queira uma lista de todos os usuários com nomes que começam com "Dan".</span><span class="sxs-lookup"><span data-stu-id="342c7-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="342c7-130">No Azure AD Graph, você pode usar essa solicitação:</span><span class="sxs-lookup"><span data-stu-id="342c7-130">In Azure AD Graph, you might use this request:</span></span>

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

<span data-ttu-id="342c7-131">Esta solicitação:</span><span class="sxs-lookup"><span data-stu-id="342c7-131">This request:</span></span>

- <span data-ttu-id="342c7-132">Targets versão 1,6 do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-132">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="342c7-133">Especifica `contoso.com` como a ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="342c7-133">Specifies `contoso.com` as the tenant ID.</span></span>
- <span data-ttu-id="342c7-134">Chama o recurso users.</span><span class="sxs-lookup"><span data-stu-id="342c7-134">Calls the users resource.</span></span>
- <span data-ttu-id="342c7-135">Usa o `$filter` parâmetro de consulta para limitar a resposta a determinados nomes que começam com `Dan` .</span><span class="sxs-lookup"><span data-stu-id="342c7-135">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="342c7-136">Os resultados incluem usuários com nomes como Daniel, Danforth, Danielle, DANERYS e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="342c7-136">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="342c7-137">Uma solicitação semelhante para o Microsoft Graph seria:</span><span class="sxs-lookup"><span data-stu-id="342c7-137">A similar request for Microsoft Graph would be:</span></span>

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="342c7-138">Nela</span><span class="sxs-lookup"><span data-stu-id="342c7-138">Here:</span></span>

- <span data-ttu-id="342c7-139">A versão é `v1.0` .</span><span class="sxs-lookup"><span data-stu-id="342c7-139">The version is `v1.0`.</span></span>
- <span data-ttu-id="342c7-140">A ID do locatário é inferida do token de acesso (não mostrado).</span><span class="sxs-lookup"><span data-stu-id="342c7-140">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="342c7-141">O parâmetro de recurso e de `$filter` consulta é o mesmo que a consulta do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="342c7-141">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="342c7-142">**Observação**: se você estiver usando a biblioteca de cliente .net do Azure ad Graph, confira [bibliotecas de clientes .net](migrate-azure-ad-graph-client-libraries.md) para obter estratégias e assistência mais específicas para mover para a biblioteca de cliente .net do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-142">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="342c7-143">Identificadores de chave: objectId vs ID</span><span class="sxs-lookup"><span data-stu-id="342c7-143">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="342c7-144">No gráfico do Azure AD, todos os tipos de recursos de entidade têm um identificador (ou chave) exclusivo chamado **ObjectID**.</span><span class="sxs-lookup"><span data-stu-id="342c7-144">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="342c7-145">Para a maior parte (salvo indicação em contrário) esse mesmo identificador é chamado de **ID** no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-145">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="342c7-146">Propriedades e $select padrão</span><span class="sxs-lookup"><span data-stu-id="342c7-146">Default properties and $select</span></span>

<span data-ttu-id="342c7-147">Use o `$select` parâmetro de consulta, em solicitações GET, para personalizar a resposta para incluir todas as propriedades exigidas pelo seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="342c7-147">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="342c7-148">As operações de **obtenção** ou **lista** do Microsoft Graph para recursos de usuário ou grupo retornam apenas um subconjunto de todas as propriedades, conhecidas como _propriedades padrão_.</span><span class="sxs-lookup"><span data-stu-id="342c7-148">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="342c7-149">As propriedades padrão representam as propriedades mais comumente usadas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="342c7-149">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="342c7-150">Por outro lado, o Azure AD Graph retorna o conjunto completo de todas as propriedades do respectivo recurso.</span><span class="sxs-lookup"><span data-stu-id="342c7-150">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="342c7-151">Para obter outras propriedades na v 1.0, seu aplicativo precisa solicitá-las explicitamente, usando o `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="342c7-151">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="342c7-152">Isso inclui todas as extensões de esquema de diretório que o aplicativo pode estar usando.</span><span class="sxs-lookup"><span data-stu-id="342c7-152">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="342c7-153">É uma prática recomendada solicitar apenas as propriedades que seu aplicativo realmente precisa.</span><span class="sxs-lookup"><span data-stu-id="342c7-153">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="342c7-154">Para ilustrar a diferença, use o explorador do Graph para executar as seguintes solicitações e comparar as diferentes respostas.</span><span class="sxs-lookup"><span data-stu-id="342c7-154">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="342c7-155">Revise as respostas de cada consulta.</span><span class="sxs-lookup"><span data-stu-id="342c7-155">Review the responses from each query.</span></span> <span data-ttu-id="342c7-156">Você notará que as informações de endereço são retornadas pela versão/beta, mas não pela versão/v1.0.</span><span class="sxs-lookup"><span data-stu-id="342c7-156">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="342c7-157">Isso ocorre porque as propriedades address não estão no conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="342c7-157">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="342c7-158">Se seu aplicativo depende das propriedades de endereço, você precisa atualizar suas solicitações v 1.0 para incluir o parâmetro de `$select` consulta:</span><span class="sxs-lookup"><span data-stu-id="342c7-158">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="342c7-159">A resposta para esta solicitação incluiria as propriedades de endereço.</span><span class="sxs-lookup"><span data-stu-id="342c7-159">The response for this request would include the address properties.</span></span>  <span data-ttu-id="342c7-160">Ele também inclui a propriedade **DisplayName** , mas somente porque foi especificado pelo parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="342c7-160">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="342c7-161">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="342c7-161">To learn more about:</span></span>

- <span data-ttu-id="342c7-162">Propriedades padrão no usuário, consulte [usuários](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="342c7-162">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="342c7-163">O `$select` parâmetro e outros parâmetros de consulta ODATA suportados, confira [usar parâmetros de consulta para personalizar respostas](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="342c7-163">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](/graph/query-parameters).</span></span>
- <span data-ttu-id="342c7-164">Esta e outras otimizações recomendadas, consulte [práticas recomendadas](/graph/best-practices-concept).</span><span class="sxs-lookup"><span data-stu-id="342c7-164">This and other recommended optimizations, see [Best practices](/graph/best-practices-concept).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="342c7-165">Propriedades de relações e navegação</span><span class="sxs-lookup"><span data-stu-id="342c7-165">Relationships and navigation properties</span></span>

<span data-ttu-id="342c7-166">Relações (ou propriedades de navegação) são um conceito importante no gráfico do Azure AD e no Microsoft Graph, criando uma rede de recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="342c7-166">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="342c7-167">Por exemplo, as propriedades **Manager** e **DirectReports** estendem o recurso User para fornecer a hierarquia organizacional.</span><span class="sxs-lookup"><span data-stu-id="342c7-167">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="342c7-168">As relações também definem associações, como os grupos aos quais um usuário pertence, os membros que pertencem a um grupo ou uma função de diretório e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="342c7-168">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="342c7-169">As solicitações do Azure AD Graph usam `$link` para indicar relações entre recursos.</span><span class="sxs-lookup"><span data-stu-id="342c7-169">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="342c7-170">No Microsoft Graph, isso usa a `$ref` notação ODATA 4, 1 em vez disso.</span><span class="sxs-lookup"><span data-stu-id="342c7-170">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="342c7-171">A tabela a seguir mostra vários exemplos:</span><span class="sxs-lookup"><span data-stu-id="342c7-171">The following table shows several examples:</span></span>

| <span data-ttu-id="342c7-172">Task</span><span class="sxs-lookup"><span data-stu-id="342c7-172">Task</span></span> | <span data-ttu-id="342c7-173">Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-173">Azure AD Graph</span></span> | <span data-ttu-id="342c7-174">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="342c7-174">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="342c7-175">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="342c7-175">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="342c7-176">Listar links de membros</span><span class="sxs-lookup"><span data-stu-id="342c7-176">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="342c7-177">Listar membros</span><span class="sxs-lookup"><span data-stu-id="342c7-177">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="342c7-178">Remover membro</span><span class="sxs-lookup"><span data-stu-id="342c7-178">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="342c7-179">Ao migrar seus aplicativos para o Microsoft Graph, procure solicitações que usam `$link` para associar recursos; altere-os para usar `$ref` em vez disso.</span><span class="sxs-lookup"><span data-stu-id="342c7-179">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="342c7-180">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="342c7-180">Next Steps</span></span>

- <span data-ttu-id="342c7-181">Saiba mais sobre as [diferenças de recursos de serviço](migrate-azure-ad-graph-feature-differences.md) entre o Azure ad Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-181">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="342c7-182">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="342c7-182">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="342c7-183">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="342c7-183">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
