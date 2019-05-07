---
title: Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph
description: Descreve como as solicitações do Microsoft Graph são diferentes das solicitações do Azure AD, o que ajuda a migrar aplicativos para o serviço mais recente..
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f046043b6a30d66cef96bb6eb6192bddd90d2f5f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630206"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="30b1f-103">Solicitar diferenças entre o Azure AD Graph e o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="30b1f-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="30b1f-104">Este artigo faz parte da *etapa 1:* revisar as diferenças de API do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="30b1f-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="30b1f-105">O Microsoft Graph e a API do Azure AD Graph são APIs REST e cada uma suportam convenções ODATA para parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="30b1f-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="30b1f-106">No entanto, a sintaxe varia entre essas duas APIs.</span><span class="sxs-lookup"><span data-stu-id="30b1f-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="30b1f-107">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar esses padrões de solicitação em seus próprios dados, pois é uma ótima maneira de aprender sobre as diferenças de solicitação e resposta.</span><span class="sxs-lookup"><span data-stu-id="30b1f-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="30b1f-108">Solicitações básicas</span><span class="sxs-lookup"><span data-stu-id="30b1f-108">Basic requests</span></span>

<span data-ttu-id="30b1f-109">A tabela a seguir realça as principais diferenças de solicitação entre as duas APIs:</span><span class="sxs-lookup"><span data-stu-id="30b1f-109">The following table highlights the main request differences between the two APIs:</span></span>

|| <span data-ttu-id="30b1f-110">Gráfico do Azure AD</span><span class="sxs-lookup"><span data-stu-id="30b1f-110">Azure AD Graph</span></span> | <span data-ttu-id="30b1f-111">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="30b1f-111">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="30b1f-112">Sintaxe de solicitação</span><span class="sxs-lookup"><span data-stu-id="30b1f-112">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="30b1f-113">Pontos&nbsp;de extremidade de serviço:</span><span class="sxs-lookup"><span data-stu-id="30b1f-113">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="30b1f-114">-&nbsp;Global</span><span class="sxs-lookup"><span data-stu-id="30b1f-114">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="30b1f-115">-&nbsp;L4&nbsp;gov&nbsp;(EUA)</span><span class="sxs-lookup"><span data-stu-id="30b1f-115">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="30b1f-116">-&nbsp;(DoD) de US gov&nbsp;&nbsp;&nbsp;</span><span class="sxs-lookup"><span data-stu-id="30b1f-116">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="30b1f-117">-&nbsp;Alemanha</span><span class="sxs-lookup"><span data-stu-id="30b1f-117">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="30b1f-118">-&nbsp;China&nbsp;(21vianet)</span><span class="sxs-lookup"><span data-stu-id="30b1f-118">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="30b1f-119">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="30b1f-119">{tenant_id}</span></span>|<span data-ttu-id="30b1f-120">Especifique a ID do locatário na solicitação.</span><span class="sxs-lookup"><span data-stu-id="30b1f-120">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="30b1f-121">É opcional especificar uma ID de locatário na solicitação, pois ela é inferida do token de acesso.</span><span class="sxs-lookup"><span data-stu-id="30b1f-121">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="30b1f-122">Se você especificar a ID do locatário, ela vai entre `{version}` o e `{resource}` o na URL da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30b1f-122">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="30b1f-123">Version</span><span class="sxs-lookup"><span data-stu-id="30b1f-123">{version}</span></span>|<span data-ttu-id="30b1f-124">Especifique a versão de lançamento do Graph do Azure AD na solicitação usando um parâmetro de consulta necessário.</span><span class="sxs-lookup"><span data-stu-id="30b1f-124">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="30b1f-125">Especifique a versão de lançamento do Microsoft Graph na solicitação como parte do caminho da URL imediatamente após o ponto de extremidade do serviço.</span><span class="sxs-lookup"><span data-stu-id="30b1f-125">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="30b1f-126">Você pode continuar a usar os mesmos parâmetros de consulta no Microsoft Graph como o Graph do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30b1f-126">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="30b1f-127">Exemplo de comparação de solicitação</span><span class="sxs-lookup"><span data-stu-id="30b1f-127">Example request comparison</span></span>

<span data-ttu-id="30b1f-128">Suponha que você queira uma lista de todos os usuários com nomes que começam com "Dan".</span><span class="sxs-lookup"><span data-stu-id="30b1f-128">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="30b1f-129">No Azure AD Graph, você pode usar essa solicitação:</span><span class="sxs-lookup"><span data-stu-id="30b1f-129">In Azure AD Graph, you might use this request:</span></span>

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

<span data-ttu-id="30b1f-130">Esta solicitação:</span><span class="sxs-lookup"><span data-stu-id="30b1f-130">This request:</span></span>

- <span data-ttu-id="30b1f-131">Targets versão 1,6 do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="30b1f-131">Targets version 1.6 of Azure AD Graph.</span></span>  
- <span data-ttu-id="30b1f-132">Especifica `contoso.com` como a ID do locatário.</span><span class="sxs-lookup"><span data-stu-id="30b1f-132">Specifies `contoso.com` as the tenant ID.</span></span>  
- <span data-ttu-id="30b1f-133">Chama o recurso users.</span><span class="sxs-lookup"><span data-stu-id="30b1f-133">Calls the users resource.</span></span>  
- <span data-ttu-id="30b1f-134">Usa o `$filter` parâmetro de consulta para limitar a resposta a determinados nomes que começam `Dan`com.</span><span class="sxs-lookup"><span data-stu-id="30b1f-134">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>  

<span data-ttu-id="30b1f-135">Os resultados incluem usuários com nomes como Daniel, Danforth, Danielle, DANERYS e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="30b1f-135">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="30b1f-136">Uma solicitação semelhante para o Microsoft Graph seria:</span><span class="sxs-lookup"><span data-stu-id="30b1f-136">A similar request for Microsoft Graph would be:</span></span>

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="30b1f-137">Nela</span><span class="sxs-lookup"><span data-stu-id="30b1f-137">Here:</span></span>

- <span data-ttu-id="30b1f-138">A versão é `v1.0`.</span><span class="sxs-lookup"><span data-stu-id="30b1f-138">The version is `v1.0`.</span></span>  
- <span data-ttu-id="30b1f-139">A ID do locatário é inferida do token de acesso (não mostrado).</span><span class="sxs-lookup"><span data-stu-id="30b1f-139">The tenant ID is inferred from the access token (not shown).</span></span>  
- <span data-ttu-id="30b1f-140">O parâmetro de `$filter` recurso e de consulta é o mesmo que a consulta do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30b1f-140">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>  

> <span data-ttu-id="30b1f-141">**Observação**: se você estiver usando a biblioteca de cliente .net do Azure ad Graph, confira [bibliotecas de clientes .net](migrate-azure-ad-graph-client-libraries.md) para obter estratégias e assistência mais específicas para mover para a biblioteca de cliente .net do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30b1f-141">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="30b1f-142">Identificadores de chave: objectId vs ID</span><span class="sxs-lookup"><span data-stu-id="30b1f-142">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="30b1f-143">No gráfico do Azure AD, todos os tipos de recursos de entidade têm um identificador (ou chave) exclusivo chamado **ObjectID**.</span><span class="sxs-lookup"><span data-stu-id="30b1f-143">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="30b1f-144">Para a maior parte (salvo indicação em contrário) esse mesmo identificador é chamado de **ID** no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30b1f-144">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="30b1f-145">Propriedades e $select padrão</span><span class="sxs-lookup"><span data-stu-id="30b1f-145">Default properties and $select</span></span>

<span data-ttu-id="30b1f-146">Use o `$select` parâmetro de consulta, em solicitações GET, para personalizar a resposta para incluir todas as propriedades exigidas pelo seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30b1f-146">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="30b1f-147">As operações de **obtenção** ou **lista** do Microsoft Graph para recursos de usuário ou grupo retornam apenas um subconjunto de todas as propriedades, conhecidas como _propriedades padrão_.</span><span class="sxs-lookup"><span data-stu-id="30b1f-147">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="30b1f-148">As propriedades padrão representam as propriedades mais comumente usadas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="30b1f-148">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="30b1f-149">Por outro lado, o Azure AD Graph retorna o conjunto completo de todas as propriedades do respectivo recurso.</span><span class="sxs-lookup"><span data-stu-id="30b1f-149">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="30b1f-150">Para obter outras propriedades na v 1.0, seu aplicativo precisa solicitá-las explicitamente, usando `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="30b1f-150">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="30b1f-151">Isso inclui todas as extensões de esquema de diretório que o aplicativo pode estar usando.</span><span class="sxs-lookup"><span data-stu-id="30b1f-151">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="30b1f-152">É uma prática recomendada solicitar apenas as propriedades que seu aplicativo realmente precisa.</span><span class="sxs-lookup"><span data-stu-id="30b1f-152">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="30b1f-153">Para ilustrar a diferença, use o explorador do Graph para executar as seguintes solicitações e comparar as diferentes respostas.</span><span class="sxs-lookup"><span data-stu-id="30b1f-153">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="30b1f-154">Revise as respostas de cada consulta.</span><span class="sxs-lookup"><span data-stu-id="30b1f-154">Review the responses from each query.</span></span> <span data-ttu-id="30b1f-155">Você notará que as informações de endereço são retornadas pela versão/beta, mas não pela versão/v1.0.</span><span class="sxs-lookup"><span data-stu-id="30b1f-155">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="30b1f-156">Isso ocorre porque as propriedades address não estão no conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="30b1f-156">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="30b1f-157">Se seu aplicativo depende das propriedades de endereço, você precisa atualizar suas solicitações v 1.0 para incluir o parâmetro de `$select` consulta:</span><span class="sxs-lookup"><span data-stu-id="30b1f-157">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="30b1f-158">A resposta para esta solicitação incluiria as propriedades de endereço.</span><span class="sxs-lookup"><span data-stu-id="30b1f-158">The response for this request would include the address properties.</span></span>  <span data-ttu-id="30b1f-159">Ele também inclui a propriedade **DisplayName** , mas somente porque foi especificado pelo parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="30b1f-159">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="30b1f-160">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="30b1f-160">To learn more about:</span></span>

- <span data-ttu-id="30b1f-161">Propriedades padrão no usuário, consulte [usuários](/graph/api/resources/users?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="30b1f-161">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="30b1f-162">O `$select` parâmetro e outros parâmetros de consulta ODATA suportados, confira [usar parâmetros de consulta para personalizar respostas](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="30b1f-162">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](/graph/query-parameters).</span></span>
- <span data-ttu-id="30b1f-163">Esta e outras otimizações recomendadas, consulte [práticas recomendadas](/graph/best-practices-concept).</span><span class="sxs-lookup"><span data-stu-id="30b1f-163">This and other recommended optimizations, see [Best practices](/graph/best-practices-concept).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="30b1f-164">Propriedades de relações e navegação</span><span class="sxs-lookup"><span data-stu-id="30b1f-164">Relationships and navigation properties</span></span>

<span data-ttu-id="30b1f-165">Relações (ou propriedades de navegação) são um conceito importante no gráfico do Azure AD e no Microsoft Graph, criando uma rede de recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="30b1f-165">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="30b1f-166">Por exemplo, as propriedades **Manager** e **DirectReports** estendem o recurso User para fornecer a hierarquia organizacional.</span><span class="sxs-lookup"><span data-stu-id="30b1f-166">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>  

<span data-ttu-id="30b1f-167">As relações também definem associações, como os grupos aos quais um usuário pertence, os membros que pertencem a um grupo ou uma função de diretório e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="30b1f-167">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="30b1f-168">As solicitações do Azure AD `$link` Graph usam para indicar relações entre recursos.</span><span class="sxs-lookup"><span data-stu-id="30b1f-168">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="30b1f-169">No Microsoft Graph, isso usa a notação ODATA 4, 1 `$ref` em vez disso.</span><span class="sxs-lookup"><span data-stu-id="30b1f-169">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="30b1f-170">A tabela a seguir mostra vários exemplos:</span><span class="sxs-lookup"><span data-stu-id="30b1f-170">The following table shows several examples:</span></span>

| <span data-ttu-id="30b1f-171">Tarefa</span><span class="sxs-lookup"><span data-stu-id="30b1f-171">Task</span></span> | <span data-ttu-id="30b1f-172">Gráfico do Azure AD</span><span class="sxs-lookup"><span data-stu-id="30b1f-172">Azure AD Graph</span></span> | <span data-ttu-id="30b1f-173">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="30b1f-173">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="30b1f-174">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="30b1f-174">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="30b1f-175">Listar links de membros</span><span class="sxs-lookup"><span data-stu-id="30b1f-175">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="30b1f-176">Listar membros</span><span class="sxs-lookup"><span data-stu-id="30b1f-176">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="30b1f-177">Remover membro</span><span class="sxs-lookup"><span data-stu-id="30b1f-177">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="30b1f-178">Ao migrar seus aplicativos para o Microsoft Graph, procure solicitações que `$link` usam para associar recursos; Altere-os para `$ref` usar em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="30b1f-178">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="30b1f-179">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="30b1f-179">Next Steps</span></span>

- <span data-ttu-id="30b1f-180">Saiba mais sobre as [diferenças de recursos de serviço](migrate-azure-ad-graph-feature-differences.md) entre o Azure ad Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30b1f-180">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="30b1f-181">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="30b1f-181">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="30b1f-182">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30b1f-182">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
