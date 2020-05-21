---
title: Listar grupos transitivos de dispositivo
description: Obter grupos dos quais o dispositivo é membro.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab4a13a3ae319847125a5ccbae22913c0be32a9a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333212"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="c7d61-103">Listar grupos transitivos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7d61-103">List device transitive groups</span></span>

<span data-ttu-id="c7d61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7d61-105">Obter grupos dos quais o dispositivo é membro.</span><span class="sxs-lookup"><span data-stu-id="c7d61-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="c7d61-106">Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o dispositivo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="c7d61-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7d61-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7d61-107">Permissions</span></span>

<span data-ttu-id="c7d61-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7d61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7d61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7d61-110">Permission type</span></span>      | <span data-ttu-id="c7d61-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7d61-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7d61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7d61-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7d61-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c7d61-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7d61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7d61-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7d61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7d61-115">Not supported.</span></span>    |
|<span data-ttu-id="c7d61-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7d61-116">Application</span></span> | <span data-ttu-id="c7d61-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7d61-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]


## <a name="http-request"></a><span data-ttu-id="c7d61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d61-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7d61-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7d61-119">Optional query parameters</span></span>

<span data-ttu-id="c7d61-120">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="c7d61-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="c7d61-121">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="c7d61-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="c7d61-122">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="c7d61-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="c7d61-123">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="c7d61-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c7d61-124">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="c7d61-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7d61-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d61-125">Request headers</span></span>

| <span data-ttu-id="c7d61-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7d61-126">Header</span></span>       | <span data-ttu-id="c7d61-127">Valor</span><span class="sxs-lookup"><span data-stu-id="c7d61-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7d61-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7d61-128">Authorization</span></span>  | <span data-ttu-id="c7d61-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7d61-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7d61-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c7d61-131">ConsistencyLevel</span></span> | <span data-ttu-id="c7d61-132">ocorra.</span><span class="sxs-lookup"><span data-stu-id="c7d61-132">eventual.</span></span> <span data-ttu-id="c7d61-133">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="c7d61-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c7d61-134">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="c7d61-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7d61-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d61-135">Request body</span></span>

<span data-ttu-id="c7d61-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7d61-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7d61-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d61-137">Response</span></span>

<span data-ttu-id="c7d61-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d61-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7d61-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7d61-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="c7d61-140">Exemplo 1: obter grupos dos quais o dispositivo é um membro transitiva</span><span class="sxs-lookup"><span data-stu-id="c7d61-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="c7d61-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d61-141">Request</span></span>

<span data-ttu-id="c7d61-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d61-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7d61-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d61-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="c7d61-144">C#</span><span class="sxs-lookup"><span data-stu-id="c7d61-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7d61-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7d61-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7d61-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7d61-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c7d61-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d61-147">Response</span></span>

<span data-ttu-id="c7d61-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d61-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="c7d61-151">Exemplo 2: obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="c7d61-151">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="c7d61-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d61-152">Request</span></span>

<span data-ttu-id="c7d61-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d61-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7d61-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d61-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c7d61-155">C#</span><span class="sxs-lookup"><span data-stu-id="c7d61-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7d61-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7d61-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7d61-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7d61-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c7d61-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d61-158">Response</span></span>

<span data-ttu-id="c7d61-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d61-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="c7d61-160">294</span><span class="sxs-lookup"><span data-stu-id="c7d61-160">294</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="c7d61-161">Exemplo 3: usar a conversão OData e $search para obter associação com nomes de exibição que contenham as letras "vídeo" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="c7d61-161">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c7d61-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d61-162">Request</span></span>

<span data-ttu-id="c7d61-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d61-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7d61-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7d61-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c7d61-165">C#</span><span class="sxs-lookup"><span data-stu-id="c7d61-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7d61-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7d61-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7d61-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7d61-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c7d61-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d61-168">Response</span></span>

<span data-ttu-id="c7d61-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d61-169">The following is an example of the response.</span></span>
><span data-ttu-id="c7d61-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d61-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c7d61-172">Exemplo 4: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com ' A ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="c7d61-172">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c7d61-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7d61-173">Request</span></span>

<span data-ttu-id="c7d61-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7d61-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c7d61-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7d61-175">Response</span></span>

<span data-ttu-id="c7d61-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7d61-176">The following is an example of the response.</span></span>
><span data-ttu-id="c7d61-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7d61-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
