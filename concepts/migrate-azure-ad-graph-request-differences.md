---
title: Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph
description: Descreve como as solicitações do Microsoft Graph diferem das solicitações do Azure AD, o que ajuda a migrar aplicativos para o serviço mais novo..
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e30a0c98aaf7ec0d042787f511872d02529aaa5c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760662"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="96224-103">Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="96224-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="96224-104">Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="96224-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="96224-105">O Microsoft Graph e a API do Azure AD Graph são APIs REST e cada uma delas oferece suporte a convenções ODATA para parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="96224-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="96224-106">No entanto, a sintaxe varia entre essas duas APIs.</span><span class="sxs-lookup"><span data-stu-id="96224-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="96224-107">Use o [Graph Explorer](https://aka.ms/ge) para experimentar esses padrões de solicitação em relação aos seus próprios dados, pois é uma ótima maneira de aprender sobre as diferenças de solicitação e resposta.</span><span class="sxs-lookup"><span data-stu-id="96224-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="96224-108">Solicitações básicas</span><span class="sxs-lookup"><span data-stu-id="96224-108">Basic requests</span></span>

<span data-ttu-id="96224-109">A tabela a seguir destaca as principais diferenças de solicitação entre as duas APIs:</span><span class="sxs-lookup"><span data-stu-id="96224-109">The following table highlights the main request differences between the two APIs:</span></span>

|<span data-ttu-id="96224-110">Detalhes da solicitação</span><span class="sxs-lookup"><span data-stu-id="96224-110">Request details</span></span>| <span data-ttu-id="96224-111">Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="96224-111">Azure AD Graph</span></span> | <span data-ttu-id="96224-112">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="96224-112">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="96224-113">Sintaxe de solicitação</span><span class="sxs-lookup"><span data-stu-id="96224-113">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="96224-114">Pontos &nbsp; de extremidade do serviço:</span><span class="sxs-lookup"><span data-stu-id="96224-114">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="96224-115">-&nbsp;Global</span><span class="sxs-lookup"><span data-stu-id="96224-115">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="96224-116">-&nbsp;US &nbsp; Gov &nbsp; L4</span><span class="sxs-lookup"><span data-stu-id="96224-116">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="96224-117">-&nbsp;US &nbsp; Gov &nbsp; L5 &nbsp; (DOD)</span><span class="sxs-lookup"><span data-stu-id="96224-117">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="96224-118">-&nbsp;Alemanha</span><span class="sxs-lookup"><span data-stu-id="96224-118">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="96224-119">-&nbsp;China &nbsp; (21Vianet)</span><span class="sxs-lookup"><span data-stu-id="96224-119">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="96224-120">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="96224-120">{tenant_id}</span></span>|<span data-ttu-id="96224-121">Especifique a ID do locatário na solicitação.</span><span class="sxs-lookup"><span data-stu-id="96224-121">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="96224-122">É opcional especificar uma ID de locatário na solicitação, pois ela é inferida do token de acesso.</span><span class="sxs-lookup"><span data-stu-id="96224-122">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="96224-123">Se você especificar a ID do locatário, ela fica entre a URL e `{version}` `{resource}` a da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96224-123">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="96224-124">{version}</span><span class="sxs-lookup"><span data-stu-id="96224-124">{version}</span></span>|<span data-ttu-id="96224-125">Especifique a versão de versão do Azure AD Graph na solicitação usando um parâmetro de consulta necessário.</span><span class="sxs-lookup"><span data-stu-id="96224-125">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="96224-126">Especifique a versão de versão do Microsoft Graph na solicitação como parte do caminho da URL logo após o ponto de extremidade do serviço.</span><span class="sxs-lookup"><span data-stu-id="96224-126">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="96224-127">Você pode continuar a usar os mesmos parâmetros de consulta no Microsoft Graph que o Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="96224-127">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="96224-128">Comparação de solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="96224-128">Example request comparison</span></span>

<span data-ttu-id="96224-129">Suponha que você queira uma lista de todos os usuários com nomes começando com "Dan".</span><span class="sxs-lookup"><span data-stu-id="96224-129">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="96224-130">No Azure AD Graph, você pode usar esta solicitação:</span><span class="sxs-lookup"><span data-stu-id="96224-130">In Azure AD Graph, you might use this request:</span></span>

<span data-ttu-id="96224-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` ou </span><span class="sxs-lookup"><span data-stu-id="96224-131">`GET https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6` or</span></span>

`GET https://graph.windows.net/myOrganization/users?$filter=startswith(givenName,'Dan')&api-version=1.6`


<span data-ttu-id="96224-132">Esta solicitação:</span><span class="sxs-lookup"><span data-stu-id="96224-132">This request:</span></span>

- <span data-ttu-id="96224-133">Direciona a versão 1.6 do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="96224-133">Targets version 1.6 of Azure AD Graph.</span></span>
- <span data-ttu-id="96224-134">Especifica como `contoso.com` a ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="96224-134">Specifies `contoso.com` as the tenant ID.</span></span> <span data-ttu-id="96224-135">A alternativa mostra o uso de um alias com base na ID do `myOrganization` locatário no token de acesso.</span><span class="sxs-lookup"><span data-stu-id="96224-135">The alternative shows the use of an alias `myOrganization` based on the tenant ID in the access token.</span></span>
- <span data-ttu-id="96224-136">Chama o recurso users.</span><span class="sxs-lookup"><span data-stu-id="96224-136">Calls the users resource.</span></span>
- <span data-ttu-id="96224-137">Usa o `$filter` parâmetro de consulta para limitar a resposta a determinados nomes que começam com `Dan` .</span><span class="sxs-lookup"><span data-stu-id="96224-137">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>

<span data-ttu-id="96224-138">Os resultados incluem usuários com nomes como Daniel, Danforth, Danielle, Danerys e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="96224-138">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="96224-139">Uma solicitação semelhante para o Microsoft Graph seria:</span><span class="sxs-lookup"><span data-stu-id="96224-139">A similar request for Microsoft Graph would be:</span></span>

`GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="96224-140">Aqui:</span><span class="sxs-lookup"><span data-stu-id="96224-140">Here:</span></span>

- <span data-ttu-id="96224-141">A versão é `v1.0` .</span><span class="sxs-lookup"><span data-stu-id="96224-141">The version is `v1.0`.</span></span>
- <span data-ttu-id="96224-142">A ID do locatário é inferida do token de acesso (não mostrado).</span><span class="sxs-lookup"><span data-stu-id="96224-142">The tenant ID is inferred from the access token (not shown).</span></span>
- <span data-ttu-id="96224-143">O parâmetro resource and query é o mesmo que a consulta `$filter` do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96224-143">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>

> <span data-ttu-id="96224-144">**OBSERVAÇÃO**: se você estiver usando a biblioteca de clientes do Azure AD Graph .NET, consulte Bibliotecas de clientes [.NET](migrate-azure-ad-graph-client-libraries.md) para obter estratégias e assistência mais específicas para mover para a biblioteca de clientes do Microsoft Graph .NET.</span><span class="sxs-lookup"><span data-stu-id="96224-144">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="96224-145">Identificadores de chave: objectId vs id</span><span class="sxs-lookup"><span data-stu-id="96224-145">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="96224-146">No Azure AD Graph, todos os tipos de recursos de entidade têm um identificador exclusivo (ou chave) chamado **objectId**.</span><span class="sxs-lookup"><span data-stu-id="96224-146">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="96224-147">Na maioria das partes (a menos que seja declarado de outra forma), esse mesmo identificador é chamado **de id** no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96224-147">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="96224-148">Propriedades padrão e $select</span><span class="sxs-lookup"><span data-stu-id="96224-148">Default properties and $select</span></span>

<span data-ttu-id="96224-149">Use o parâmetro de consulta, em solicitações GET, para personalizar a resposta para incluir todas as `$select` propriedades que seu aplicativo exige.</span><span class="sxs-lookup"><span data-stu-id="96224-149">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="96224-150">O Microsoft Graph **obter** ou **listar** operações para recursos de usuário ou grupo retorna apenas um subconjunto de todas as propriedades, conhecidas como _as propriedades padrão_.</span><span class="sxs-lookup"><span data-stu-id="96224-150">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="96224-151">As propriedades padrão representam as propriedades mais comumente usadas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="96224-151">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="96224-152">Por outro lado, o Azure AD Graph retorna o conjunto completo de todas as propriedades do respectivo recurso.</span><span class="sxs-lookup"><span data-stu-id="96224-152">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="96224-153">Para obter outras propriedades em v1.0, seu aplicativo precisa solicitá-las explicitamente, usando o `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="96224-153">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="96224-154">Isso inclui qualquer extensão de esquema de diretório que seu aplicativo possa estar usando.</span><span class="sxs-lookup"><span data-stu-id="96224-154">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="96224-155">É uma prática prática só solicitar as propriedades que seu aplicativo realmente precisa.</span><span class="sxs-lookup"><span data-stu-id="96224-155">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="96224-156">Para ilustrar a diferença, use o Graph Explorer para executar as seguintes solicitações e comparar as diferentes respostas.</span><span class="sxs-lookup"><span data-stu-id="96224-156">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="96224-157">Revise as respostas de cada consulta.</span><span class="sxs-lookup"><span data-stu-id="96224-157">Review the responses from each query.</span></span> <span data-ttu-id="96224-158">Você notará que as informações de endereço são retornadas pela versão /beta, mas não pela versão /v1.0.</span><span class="sxs-lookup"><span data-stu-id="96224-158">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="96224-159">Isso porque as propriedades de endereço não estão no conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="96224-159">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="96224-160">Se o aplicativo se basear nas propriedades de endereço, você precisará atualizar suas solicitações v1.0 para incluir o `$select` parâmetro de consulta:</span><span class="sxs-lookup"><span data-stu-id="96224-160">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="96224-161">A resposta para essa solicitação incluiria as propriedades de endereço.</span><span class="sxs-lookup"><span data-stu-id="96224-161">The response for this request would include the address properties.</span></span>  <span data-ttu-id="96224-162">Ele também inclui a **propriedade displayName,** mas somente porque foi especificada pelo parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="96224-162">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="96224-163">Para saber mais sobre:</span><span class="sxs-lookup"><span data-stu-id="96224-163">To learn more about:</span></span>

- <span data-ttu-id="96224-164">Propriedades padrão no usuário, consulte [users](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="96224-164">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96224-165">O parâmetro e outros parâmetros de consulta ODATA com `$select` suporte, consulte [Use query parameters to customize responses](./query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="96224-165">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](./query-parameters.md).</span></span>
- <span data-ttu-id="96224-166">Esta e outras otimizações recomendadas, consulte [Práticas recomendadas.](./best-practices-concept.md)</span><span class="sxs-lookup"><span data-stu-id="96224-166">This and other recommended optimizations, see [Best practices](./best-practices-concept.md).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="96224-167">Relações e propriedades de navegação</span><span class="sxs-lookup"><span data-stu-id="96224-167">Relationships and navigation properties</span></span>

<span data-ttu-id="96224-168">As relações (ou propriedades de navegação) são um conceito-chave no Azure AD Graph e no Microsoft Graph, criando uma rede de recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="96224-168">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="96224-169">Por exemplo, as **propriedades manager** e **directReports** estendem o recurso do usuário para fornecer hierarquia organizacional.</span><span class="sxs-lookup"><span data-stu-id="96224-169">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>

<span data-ttu-id="96224-170">As relações também definem associações, como os grupos aos quais um usuário pertence, os membros pertencentes a um grupo ou a uma função de diretório e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="96224-170">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="96224-171">As solicitações do Azure AD Graph `$link` são usadas para indicar relações entre recursos.</span><span class="sxs-lookup"><span data-stu-id="96224-171">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="96224-172">No Microsoft Graph, isso usa a notação ODATA 4.01. `$ref`</span><span class="sxs-lookup"><span data-stu-id="96224-172">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="96224-173">A tabela a seguir mostra vários exemplos:</span><span class="sxs-lookup"><span data-stu-id="96224-173">The following table shows several examples:</span></span>

| <span data-ttu-id="96224-174">Tarefa</span><span class="sxs-lookup"><span data-stu-id="96224-174">Task</span></span> | <span data-ttu-id="96224-175">Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="96224-175">Azure AD Graph</span></span> | <span data-ttu-id="96224-176">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="96224-176">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="96224-177">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="96224-177">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="96224-178">Listar links de membros</span><span class="sxs-lookup"><span data-stu-id="96224-178">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="96224-179">Listar membros</span><span class="sxs-lookup"><span data-stu-id="96224-179">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="96224-180">Remover membro</span><span class="sxs-lookup"><span data-stu-id="96224-180">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="96224-181">Ao migrar seus aplicativos para o Microsoft Graph, procure solicitações que usam para associar `$link` recursos; altere-os para `$ref` usar.</span><span class="sxs-lookup"><span data-stu-id="96224-181">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="96224-182">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="96224-182">Next Steps</span></span>

- <span data-ttu-id="96224-183">Saiba mais [sobre as diferenças de](migrate-azure-ad-graph-feature-differences.md) recursos de serviço entre o Azure AD Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96224-183">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="96224-184">Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.</span><span class="sxs-lookup"><span data-stu-id="96224-184">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>