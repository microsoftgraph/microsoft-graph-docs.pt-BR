---
title: 'oauth2permissiongrant: Delta'
description: Obter oauth2permissiongrants recentemente criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.
localization_priority: Normal
author: psignoret
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f7775425ad31bba33cb31df296cc5985ea73ab70
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064763"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="a534e-103">oauth2permissiongrant: Delta</span><span class="sxs-lookup"><span data-stu-id="a534e-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="a534e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a534e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a534e-105">Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="a534e-105">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="a534e-106">Para obter detalhes, consulte [usando a consulta Delta](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="a534e-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="a534e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a534e-107">Permissions</span></span>

<span data-ttu-id="a534e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a534e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a534e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a534e-110">Permission type</span></span>      | <span data-ttu-id="a534e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a534e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a534e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a534e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a534e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a534e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a534e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a534e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a534e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a534e-115">Not supported.</span></span>    |
|<span data-ttu-id="a534e-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="a534e-116">oauth2permissiongrant</span></span> | <span data-ttu-id="a534e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a534e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a534e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a534e-118">HTTP request</span></span>

<span data-ttu-id="a534e-119">Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso **oauth2permissiongrant** .</span><span class="sxs-lookup"><span data-stu-id="a534e-119">To begin tracking changes, you make a request including the delta function on the **oauth2permissiongrant** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /oauth2permissiongrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a534e-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="a534e-120">Query parameters</span></span>

<span data-ttu-id="a534e-121">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="a534e-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="a534e-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="a534e-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="a534e-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="a534e-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="a534e-124">Você só precisa especificar qualquer parâmetro de consulta uma vez na frente.</span><span class="sxs-lookup"><span data-stu-id="a534e-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="a534e-125">Em solicitações subsequentes, copie e aplique `nextLink` a `deltaLink` URL ou à resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="a534e-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="a534e-126">Essa URL já inclui os parâmetros codificados.</span><span class="sxs-lookup"><span data-stu-id="a534e-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="a534e-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="a534e-127">Query parameter</span></span>      | <span data-ttu-id="a534e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a534e-128">Type</span></span>   |<span data-ttu-id="a534e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a534e-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a534e-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a534e-130">$deltatoken</span></span> | <span data-ttu-id="a534e-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a534e-131">string</span></span> | <span data-ttu-id="a534e-132">Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="a534e-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="a534e-133">Salve e aplique a `deltaLink` URL inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle de alterações para essa coleção.</span><span class="sxs-lookup"><span data-stu-id="a534e-133">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a534e-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a534e-134">$skiptoken</span></span> | <span data-ttu-id="a534e-135">string</span><span class="sxs-lookup"><span data-stu-id="a534e-135">string</span></span> | <span data-ttu-id="a534e-136">Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="a534e-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="a534e-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a534e-137">Optional query parameters</span></span>

<span data-ttu-id="a534e-138">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a534e-138">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="a534e-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="a534e-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span>
- <span data-ttu-id="a534e-141">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="a534e-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="a534e-142">A única expressão suportada `$filter` é para controlar alterações de recursos específicos, por sua ID:  `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="a534e-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="a534e-143">O número de IDs que você pode especificar é limitado pelo tamanho máximo de URL.</span><span class="sxs-lookup"><span data-stu-id="a534e-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="a534e-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a534e-144">Request headers</span></span>
| <span data-ttu-id="a534e-145">Nome</span><span class="sxs-lookup"><span data-stu-id="a534e-145">Name</span></span>       | <span data-ttu-id="a534e-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="a534e-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a534e-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="a534e-147">Authorization</span></span>  | <span data-ttu-id="a534e-148">&lt;token&gt; de portador.</span><span class="sxs-lookup"><span data-stu-id="a534e-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="a534e-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a534e-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a534e-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a534e-150">Request body</span></span>
<span data-ttu-id="a534e-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a534e-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a534e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a534e-152">Response</span></span>

<span data-ttu-id="a534e-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [oauth2permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a534e-153">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="a534e-154">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="a534e-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="a534e-155">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="a534e-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a534e-156">O **oauth2permissiongrant** continua fazendo solicitações usando a `nextLink` URL até que uma `deltaLink` URL seja incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="a534e-156">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="a534e-157">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a534e-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a534e-158">Persista e use a `deltaLink` URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="a534e-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="a534e-159">Para obter detalhes, consulte [usando a consulta Delta](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="a534e-159">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="a534e-160">Por exemplo, consulte [obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="a534e-160">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="a534e-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a534e-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="a534e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a534e-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a534e-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="a534e-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2permissiongrants/delta
```
# <a name="c"></a>[<span data-ttu-id="a534e-164">C#</span><span class="sxs-lookup"><span data-stu-id="a534e-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a534e-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a534e-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a534e-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a534e-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a534e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="a534e-167">Response</span></span>
><span data-ttu-id="a534e-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a534e-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/beta/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "expiryTime": "2017-08-13T21:41:23.3929007Z",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "startTime": "0001-01-01T00:00:00Z",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


