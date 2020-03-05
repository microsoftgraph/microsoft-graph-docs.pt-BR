---
title: 'servicePrincipalName: Delta'
description: Obtenha entidades de serviço recém-criadas, atualizadas ou excluídas sem ter que realizar uma leitura completa de toda a coleção de recursos. Consulte usando a consulta Delta para obter detalhes.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 98d2398a56cd94b557c86f209361ee77fa100626
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453489"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="f6ee1-104">servicePrincipalName: Delta</span><span class="sxs-lookup"><span data-stu-id="f6ee1-104">servicePrincipal: delta</span></span>

<span data-ttu-id="f6ee1-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f6ee1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6ee1-106">Obtenha entidades de serviço recém-criadas, atualizadas ou excluídas sem ter que realizar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-106">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="f6ee1-107">Consulte [usando a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-107">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6ee1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6ee1-108">Permissions</span></span>

<span data-ttu-id="f6ee1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ee1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6ee1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6ee1-111">Permission type</span></span>      | <span data-ttu-id="f6ee1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6ee1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6ee1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6ee1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f6ee1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6ee1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6ee1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6ee1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6ee1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-116">Not supported.</span></span>    |
|<span data-ttu-id="f6ee1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6ee1-117">Application</span></span> | <span data-ttu-id="f6ee1-118">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6ee1-118">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6ee1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ee1-119">HTTP request</span></span>

<span data-ttu-id="f6ee1-120">Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso de servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-120">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="f6ee1-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="f6ee1-121">Query parameters</span></span>

<span data-ttu-id="f6ee1-122">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="f6ee1-122">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="f6ee1-123">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-123">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="f6ee1-124">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-124">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="f6ee1-125">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-125">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="f6ee1-126">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-126">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f6ee1-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="f6ee1-127">Query parameter</span></span>      | <span data-ttu-id="f6ee1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6ee1-128">Type</span></span>   |<span data-ttu-id="f6ee1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ee1-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6ee1-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f6ee1-130">$deltatoken</span></span> | <span data-ttu-id="f6ee1-131">string</span><span class="sxs-lookup"><span data-stu-id="f6ee1-131">string</span></span> | <span data-ttu-id="f6ee1-132">Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="f6ee1-133">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f6ee1-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f6ee1-134">$skiptoken</span></span> | <span data-ttu-id="f6ee1-135">string</span><span class="sxs-lookup"><span data-stu-id="f6ee1-135">string</span></span> | <span data-ttu-id="f6ee1-136">Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f6ee1-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6ee1-137">Optional query parameters</span></span>

<span data-ttu-id="f6ee1-138">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-138">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="f6ee1-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="f6ee1-141">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="f6ee1-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="f6ee1-142">A única expressão `$filter` suportada é para controlar alterações de recursos específicos, por sua `$filter=id+eq+{value}` ID `$filter=id+eq+{value1}+or+id+eq+{value2}`: ou.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-142">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="f6ee1-143">O número de IDs que você pode especificar é limitado pelo tamanho máximo de URL.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-143">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="f6ee1-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6ee1-144">Request headers</span></span>
| <span data-ttu-id="f6ee1-145">Nome</span><span class="sxs-lookup"><span data-stu-id="f6ee1-145">Name</span></span>       | <span data-ttu-id="f6ee1-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ee1-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f6ee1-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6ee1-147">Authorization</span></span>  | <span data-ttu-id="f6ee1-148">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="f6ee1-148">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f6ee1-149">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6ee1-149">Content-Type</span></span>  | <span data-ttu-id="f6ee1-150">application/json</span><span class="sxs-lookup"><span data-stu-id="f6ee1-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6ee1-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6ee1-151">Request body</span></span>
<span data-ttu-id="f6ee1-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-152">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="f6ee1-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6ee1-153">Response</span></span>

<span data-ttu-id="f6ee1-154">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-154">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="f6ee1-155">A resposta também inclui uma URL do nextLink ou uma URL do deltaLink.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-155">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="f6ee1-156">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-156">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="f6ee1-157">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-157">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="f6ee1-158">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-158">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="f6ee1-159">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-159">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="f6ee1-160">Confira:</span><span class="sxs-lookup"><span data-stu-id="f6ee1-160">See:</span></span></br>
- <span data-ttu-id="f6ee1-161">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f6ee1-161">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="f6ee1-162">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-162">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="f6ee1-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6ee1-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6ee1-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6ee1-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6ee1-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ee1-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```
# <a name="c"></a>[<span data-ttu-id="f6ee1-166">C#</span><span class="sxs-lookup"><span data-stu-id="f6ee1-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6ee1-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6ee1-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6ee1-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6ee1-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6ee1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6ee1-169">Response</span></span>
<span data-ttu-id="f6ee1-p111">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f6ee1-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
