---
title: 'servicePrincipal: delta'
description: Obter entidades de serviço recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Usando a Consulta Delta para obter detalhes.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c07df18bc685e6a9ee351ad76bdcf42ea65548b2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134614"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="781a1-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="781a1-104">servicePrincipal: delta</span></span>

<span data-ttu-id="781a1-105">Obter entidades de serviço recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="781a1-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="781a1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="781a1-106">Permissions</span></span>

<span data-ttu-id="781a1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="781a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="781a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="781a1-109">Permission type</span></span>      | <span data-ttu-id="781a1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="781a1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="781a1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="781a1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="781a1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="781a1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="781a1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="781a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="781a1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="781a1-114">Not supported.</span></span>    |
|<span data-ttu-id="781a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="781a1-115">Application</span></span> | <span data-ttu-id="781a1-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="781a1-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="781a1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="781a1-117">HTTP request</span></span>

<span data-ttu-id="781a1-118">Para começar a controlar as alterações, faça uma solicitação incluindo a função delta no recurso servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="781a1-118">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

## <a name="query-parameters"></a><span data-ttu-id="781a1-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="781a1-119">Query parameters</span></span>

<span data-ttu-id="781a1-120">O rastreamento de alterações incorre em uma série de uma ou mais **chamadas de função delta.**</span><span class="sxs-lookup"><span data-stu-id="781a1-120">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="781a1-121">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="781a1-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="781a1-122">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="781a1-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="781a1-123">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="781a1-123">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="781a1-124">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="781a1-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="781a1-125">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="781a1-125">Query parameter</span></span>      | <span data-ttu-id="781a1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="781a1-126">Type</span></span>   |<span data-ttu-id="781a1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="781a1-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="781a1-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="781a1-128">$deltatoken</span></span> | <span data-ttu-id="781a1-129">string</span><span class="sxs-lookup"><span data-stu-id="781a1-129">string</span></span> | <span data-ttu-id="781a1-130">Um [token de](/graph/delta-query-overview) estado retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa série de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="781a1-130">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="781a1-131">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="781a1-131">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="781a1-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="781a1-132">$skiptoken</span></span> | <span data-ttu-id="781a1-133">string</span><span class="sxs-lookup"><span data-stu-id="781a1-133">string</span></span> | <span data-ttu-id="781a1-134">Um [token de](/graph/delta-query-overview) estado retornado na URL da chamada de função delta anterior indicando que não há mais alterações a serem controladas na mesma coleção de `nextLink` recursos. </span><span class="sxs-lookup"><span data-stu-id="781a1-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="781a1-135">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="781a1-135">Optional query parameters</span></span>

<span data-ttu-id="781a1-136">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="781a1-136">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="781a1-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="781a1-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="781a1-139">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="781a1-139">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="781a1-140">A única expressão com `$filter` suporte é para controlar alterações de recursos específicos, por sua id: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="781a1-140">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="781a1-141">O número de IDs que você pode especificar é limitado pelo comprimento máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="781a1-141">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="781a1-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="781a1-142">Request headers</span></span>
| <span data-ttu-id="781a1-143">Nome</span><span class="sxs-lookup"><span data-stu-id="781a1-143">Name</span></span>       | <span data-ttu-id="781a1-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="781a1-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="781a1-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="781a1-145">Authorization</span></span>  | <span data-ttu-id="781a1-146">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="781a1-146">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="781a1-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="781a1-147">Request body</span></span>
<span data-ttu-id="781a1-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="781a1-148">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="781a1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="781a1-149">Response</span></span>

<span data-ttu-id="781a1-150">Se bem-sucedido, este método retorna um código de resposta e um objeto da coleção `200 OK` [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="781a1-150">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="781a1-151">A resposta também inclui uma URL nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="781a1-151">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="781a1-152">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="781a1-152">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="781a1-153">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="781a1-153">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="781a1-154">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="781a1-154">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="781a1-155">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="781a1-155">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="781a1-156">Confira:</span><span class="sxs-lookup"><span data-stu-id="781a1-156">See:</span></span></br>
- <span data-ttu-id="781a1-157">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="781a1-157">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="781a1-158">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="781a1-158">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="781a1-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="781a1-159">Example</span></span>
#### <a name="request"></a><span data-ttu-id="781a1-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="781a1-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="781a1-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="781a1-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="781a1-162">C#</span><span class="sxs-lookup"><span data-stu-id="781a1-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="781a1-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="781a1-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="781a1-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="781a1-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="781a1-165">Java</span><span class="sxs-lookup"><span data-stu-id="781a1-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="781a1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="781a1-166">Response</span></span>
><span data-ttu-id="781a1-167">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="781a1-167">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="781a1-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="781a1-168">All the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

