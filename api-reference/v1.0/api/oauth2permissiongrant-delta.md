---
title: 'oauth2permissiongrant: delta'
description: Obter recém-criados, atualizados ou excluídos oauth2permissiongrants sem executar uma leitura completa de toda a coleção de recursos.
localization_priority: Normal
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 63d936ab649a4e8842d633033a74d8958cd22bed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441778"
---
# <a name="oauth2permissiongrant-delta"></a><span data-ttu-id="b80ab-103">oauth2permissiongrant: delta</span><span class="sxs-lookup"><span data-stu-id="b80ab-103">oauth2permissiongrant: delta</span></span>

<span data-ttu-id="b80ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b80ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b80ab-105">Obter objetos [oauth2permissiongrant](../resources/oauth2permissiongrant.md) recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="b80ab-105">Get newly created, updated, or deleted [oauth2permissiongrant](../resources/oauth2permissiongrant.md) objects without performing a full read of the entire resource collection.</span></span> <span data-ttu-id="b80ab-106">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="b80ab-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="b80ab-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b80ab-107">Permissions</span></span>

<span data-ttu-id="b80ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b80ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b80ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b80ab-110">Permission type</span></span>      | <span data-ttu-id="b80ab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b80ab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b80ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b80ab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b80ab-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b80ab-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b80ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b80ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b80ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b80ab-115">Not supported.</span></span>    |
|<span data-ttu-id="b80ab-116">oauth2permissiongrant</span><span class="sxs-lookup"><span data-stu-id="b80ab-116">oauth2permissiongrant</span></span> | <span data-ttu-id="b80ab-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80ab-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b80ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b80ab-118">HTTP request</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b80ab-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b80ab-119">Query parameters</span></span>

<span data-ttu-id="b80ab-120">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="b80ab-120">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b80ab-121">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="b80ab-121">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b80ab-122">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="b80ab-122">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="b80ab-123">Você só precisa especificar parâmetros de consulta uma vez.</span><span class="sxs-lookup"><span data-stu-id="b80ab-123">You only need to specify query parameters once.</span></span> <span data-ttu-id="b80ab-124">Em solicitações subsequentes, copie e aplique `nextLink` a URL ou da resposta `deltaLink` anterior.</span><span class="sxs-lookup"><span data-stu-id="b80ab-124">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="b80ab-125">A URL inclui os parâmetros codificados.</span><span class="sxs-lookup"><span data-stu-id="b80ab-125">The URL includes the encoded parameters.</span></span>

| <span data-ttu-id="b80ab-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="b80ab-126">Query parameter</span></span>      | <span data-ttu-id="b80ab-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b80ab-127">Type</span></span>   |<span data-ttu-id="b80ab-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b80ab-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b80ab-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="b80ab-129">$deltatoken</span></span> | <span data-ttu-id="b80ab-130">string</span><span class="sxs-lookup"><span data-stu-id="b80ab-130">string</span></span> | <span data-ttu-id="b80ab-131">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="b80ab-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="b80ab-132">Salve e aplique a URL inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle `deltaLink` de alterações para essa coleção.</span><span class="sxs-lookup"><span data-stu-id="b80ab-132">Save and apply the entire `deltaLink` URL, including this token, in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="b80ab-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b80ab-133">$skiptoken</span></span> | <span data-ttu-id="b80ab-134">string</span><span class="sxs-lookup"><span data-stu-id="b80ab-134">string</span></span> | <span data-ttu-id="b80ab-135">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na `nextLink` mesma coleção de recursos. </span><span class="sxs-lookup"><span data-stu-id="b80ab-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="b80ab-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b80ab-136">Optional query parameters</span></span>

<span data-ttu-id="b80ab-137">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b80ab-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="b80ab-138">Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades de que precisa para o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="b80ab-138">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="b80ab-139">A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="b80ab-139">The **id** property is always returned.</span></span>
- <span data-ttu-id="b80ab-140">O parâmetro de consulta só pode ser usado para rastrear alterações em recursos `$filter` específicos usando a ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="b80ab-140">The `$filter` query parameter can only be used to track changes on specific resources by using the resource ID.</span></span> <span data-ttu-id="b80ab-141">Por exemplo, `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="b80ab-141">For example, `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="b80ab-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b80ab-142">Request headers</span></span>
| <span data-ttu-id="b80ab-143">Nome</span><span class="sxs-lookup"><span data-stu-id="b80ab-143">Name</span></span>       | <span data-ttu-id="b80ab-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b80ab-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b80ab-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="b80ab-145">Authorization</span></span>  | <span data-ttu-id="b80ab-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b80ab-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b80ab-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b80ab-148">Request body</span></span>
<span data-ttu-id="b80ab-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b80ab-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b80ab-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b80ab-150">Response</span></span>

<span data-ttu-id="b80ab-151">Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [oauth2permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b80ab-151">If successful, this method returns a `200 OK` response code and an [oauth2permissiongrant](../resources/oauth2permissiongrant.md) collection object in the response body.</span></span> <span data-ttu-id="b80ab-152">A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="b80ab-152">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="b80ab-153">Se uma `nextLink` URL for retornada, páginas adicionais de dados poderão ser recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="b80ab-153">If a `nextLink` URL is returned, additional pages of data can be retrieved in the session.</span></span> <span data-ttu-id="b80ab-154">O **oauth2permissiongrant** continua fazendo solicitações usando `nextLink` a URL até que uma URL seja incluída na `deltaLink` resposta.</span><span class="sxs-lookup"><span data-stu-id="b80ab-154">The **oauth2permissiongrant** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="b80ab-155">Se uma `deltaLink` URL for retornada, nenhum dado sobre o recurso será retornado.</span><span class="sxs-lookup"><span data-stu-id="b80ab-155">If a `deltaLink` URL is returned, no more data about the resource is returned.</span></span> <span data-ttu-id="b80ab-156">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="b80ab-156">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="b80ab-157">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="b80ab-157">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="b80ab-158">Por exemplo, solicitações, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="b80ab-158">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="b80ab-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b80ab-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="b80ab-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b80ab-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b80ab-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b80ab-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/delta
```
# <a name="c"></a>[<span data-ttu-id="b80ab-162">C#</span><span class="sxs-lookup"><span data-stu-id="b80ab-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b80ab-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b80ab-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b80ab-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b80ab-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b80ab-165">Java</span><span class="sxs-lookup"><span data-stu-id="b80ab-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b80ab-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b80ab-166">Response</span></span>
><span data-ttu-id="b80ab-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b80ab-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
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

