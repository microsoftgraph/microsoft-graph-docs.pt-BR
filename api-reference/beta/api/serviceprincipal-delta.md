---
title: 'servicePrincipal: delta'
description: Obter entidades de serviço recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Using Delta Query para obter detalhes.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a878e82a591f287712231c68022874b5967cbd1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051939"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="7dbc8-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="7dbc8-104">servicePrincipal: delta</span></span>

<span data-ttu-id="7dbc8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dbc8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dbc8-106">Obter entidades de serviço recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dbc8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dbc8-107">Permissions</span></span>

<span data-ttu-id="7dbc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dbc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7dbc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dbc8-110">Permission type</span></span>      | <span data-ttu-id="7dbc8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dbc8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dbc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dbc8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7dbc8-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dbc8-113">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7dbc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dbc8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dbc8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-115">Not supported.</span></span>    |
|<span data-ttu-id="7dbc8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dbc8-116">Application</span></span> | <span data-ttu-id="7dbc8-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dbc8-117">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dbc8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dbc8-118">HTTP request</span></span>

<span data-ttu-id="7dbc8-119">Para começar a controlar as alterações, você faz uma solicitação incluindo a função delta no recurso servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="7dbc8-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="7dbc8-120">Query parameters</span></span>

<span data-ttu-id="7dbc8-121">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="7dbc8-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="7dbc8-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="7dbc8-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="7dbc8-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="7dbc8-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="7dbc8-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="7dbc8-126">Query parameter</span></span>      | <span data-ttu-id="7dbc8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dbc8-127">Type</span></span>   |<span data-ttu-id="7dbc8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dbc8-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7dbc8-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="7dbc8-129">$deltatoken</span></span> | <span data-ttu-id="7dbc8-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7dbc8-130">string</span></span> | <span data-ttu-id="7dbc8-131">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="7dbc8-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="7dbc8-132">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="7dbc8-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7dbc8-133">$skiptoken</span></span> | <span data-ttu-id="7dbc8-134">string</span><span class="sxs-lookup"><span data-stu-id="7dbc8-134">string</span></span> | <span data-ttu-id="7dbc8-135">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção de `nextLink` recursos. </span><span class="sxs-lookup"><span data-stu-id="7dbc8-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="7dbc8-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7dbc8-136">Optional query parameters</span></span>

<span data-ttu-id="7dbc8-137">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="7dbc8-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="7dbc8-140">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="7dbc8-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="7dbc8-141">A única expressão `$filter` com suporte é para controlar alterações para recursos específicos, por sua id: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="7dbc8-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="7dbc8-142">O número de ids que você pode especificar é limitado pelo tamanho máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="7dbc8-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbc8-143">Request headers</span></span>
| <span data-ttu-id="7dbc8-144">Nome</span><span class="sxs-lookup"><span data-stu-id="7dbc8-144">Name</span></span>       | <span data-ttu-id="7dbc8-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dbc8-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7dbc8-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dbc8-146">Authorization</span></span>  | <span data-ttu-id="7dbc8-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="7dbc8-147">Bearer &lt;token&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dbc8-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbc8-148">Request body</span></span>
<span data-ttu-id="7dbc8-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-149">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="7dbc8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dbc8-150">Response</span></span>

<span data-ttu-id="7dbc8-151">Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-151">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="7dbc8-152">A resposta também inclui uma URL do nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-152">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="7dbc8-153">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-153">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="7dbc8-154">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-154">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="7dbc8-155">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-155">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="7dbc8-156">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="7dbc8-157">Confira:</span><span class="sxs-lookup"><span data-stu-id="7dbc8-157">See:</span></span></br>
- <span data-ttu-id="7dbc8-158">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="7dbc8-158">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="7dbc8-159">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-159">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="7dbc8-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dbc8-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="7dbc8-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbc8-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7dbc8-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dbc8-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="7dbc8-163">C#</span><span class="sxs-lookup"><span data-stu-id="7dbc8-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dbc8-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dbc8-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dbc8-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dbc8-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dbc8-166">Java</span><span class="sxs-lookup"><span data-stu-id="7dbc8-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7dbc8-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dbc8-167">Response</span></span>
><span data-ttu-id="7dbc8-168">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7dbc8-168">Note: The response object shown here might be shortened for readability.</span></span>
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



