---
title: 'servicePrincipal: delta'
description: Obter entidades de serviço recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Usando a Consulta Delta para obter detalhes.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 316ad5f18336cd269bcab8bbd773c9957654b240
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133326"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="b573f-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="b573f-104">servicePrincipal: delta</span></span>

<span data-ttu-id="b573f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b573f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b573f-106">Obter entidades de serviço recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="b573f-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="b573f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b573f-107">Permissions</span></span>

<span data-ttu-id="b573f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b573f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b573f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b573f-110">Permission type</span></span>      | <span data-ttu-id="b573f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b573f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b573f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b573f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b573f-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b573f-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b573f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b573f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b573f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b573f-115">Not supported.</span></span>    |
|<span data-ttu-id="b573f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b573f-116">Application</span></span> | <span data-ttu-id="b573f-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b573f-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b573f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b573f-118">HTTP request</span></span>

<span data-ttu-id="b573f-119">Para começar a controlar as alterações, faça uma solicitação incluindo a função delta no recurso servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="b573f-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="b573f-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b573f-120">Query parameters</span></span>

<span data-ttu-id="b573f-121">O rastreamento de alterações incorre em uma série de uma ou mais **chamadas de função delta.**</span><span class="sxs-lookup"><span data-stu-id="b573f-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b573f-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="b573f-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b573f-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="b573f-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="b573f-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="b573f-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="b573f-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="b573f-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="b573f-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="b573f-126">Query parameter</span></span>      | <span data-ttu-id="b573f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b573f-127">Type</span></span>   |<span data-ttu-id="b573f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b573f-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b573f-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b573f-129">$deltatoken</span></span> | <span data-ttu-id="b573f-130">string</span><span class="sxs-lookup"><span data-stu-id="b573f-130">string</span></span> | <span data-ttu-id="b573f-131">Um [token de](/graph/delta-query-overview) estado retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa série de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="b573f-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="b573f-132">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="b573f-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b573f-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b573f-133">$skiptoken</span></span> | <span data-ttu-id="b573f-134">string</span><span class="sxs-lookup"><span data-stu-id="b573f-134">string</span></span> | <span data-ttu-id="b573f-135">Um [token de](/graph/delta-query-overview) estado retornado na URL da chamada de função delta anterior indicando que não há mais alterações a serem controladas na mesma coleção de `nextLink` recursos. </span><span class="sxs-lookup"><span data-stu-id="b573f-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="b573f-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b573f-136">Optional query parameters</span></span>

<span data-ttu-id="b573f-137">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b573f-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="b573f-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="b573f-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="b573f-140">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="b573f-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="b573f-141">A única expressão com `$filter` suporte é para controlar alterações de recursos específicos, por sua id: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="b573f-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="b573f-142">O número de IDs que você pode especificar é limitado pelo comprimento máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="b573f-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="b573f-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b573f-143">Request headers</span></span>
| <span data-ttu-id="b573f-144">Nome</span><span class="sxs-lookup"><span data-stu-id="b573f-144">Name</span></span>       | <span data-ttu-id="b573f-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="b573f-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b573f-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="b573f-146">Authorization</span></span>  | <span data-ttu-id="b573f-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="b573f-147">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="b573f-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b573f-148">Request body</span></span>
<span data-ttu-id="b573f-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b573f-149">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="b573f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b573f-150">Response</span></span>

<span data-ttu-id="b573f-151">Se bem-sucedido, este método retorna um código de resposta e um objeto da coleção `200 OK` [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b573f-151">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="b573f-152">A resposta também inclui uma URL nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="b573f-152">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="b573f-153">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="b573f-153">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="b573f-154">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="b573f-154">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="b573f-155">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="b573f-155">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="b573f-156">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="b573f-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="b573f-157">Confira:</span><span class="sxs-lookup"><span data-stu-id="b573f-157">See:</span></span></br>
- <span data-ttu-id="b573f-158">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="b573f-158">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="b573f-159">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="b573f-159">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="b573f-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b573f-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="b573f-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b573f-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b573f-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b573f-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="b573f-163">C#</span><span class="sxs-lookup"><span data-stu-id="b573f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b573f-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b573f-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b573f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b573f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b573f-166">Java</span><span class="sxs-lookup"><span data-stu-id="b573f-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b573f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b573f-167">Response</span></span>
><span data-ttu-id="b573f-168">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b573f-168">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b573f-169">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b573f-169">All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



