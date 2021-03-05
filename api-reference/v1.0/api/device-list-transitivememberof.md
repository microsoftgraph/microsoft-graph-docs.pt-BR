---
title: Listar grupos transitivos de dispositivos
description: Obter grupos dos que o dispositivo é membro.
author: spunukol
ms.prod: directory-management
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: e6fa162d5c72c33fe0322d11e7549a1f809b3498
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434542"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="225b7-103">Listar grupos transitivos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="225b7-103">List device transitive groups</span></span>

<span data-ttu-id="225b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="225b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="225b7-105">Obter grupos dos que o dispositivo é membro.</span><span class="sxs-lookup"><span data-stu-id="225b7-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="225b7-106">Essa solicitação de API é transitiva e também retornará todos os grupos de que o dispositivo é membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="225b7-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="225b7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="225b7-107">Permissions</span></span>

<span data-ttu-id="225b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="225b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="225b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="225b7-110">Permission type</span></span>      | <span data-ttu-id="225b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="225b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="225b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="225b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="225b7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="225b7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="225b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="225b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="225b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="225b7-115">Not supported.</span></span>    |
|<span data-ttu-id="225b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="225b7-116">Application</span></span> | <span data-ttu-id="225b7-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225b7-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="225b7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="225b7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="225b7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="225b7-119">Optional query parameters</span></span>

<span data-ttu-id="225b7-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="225b7-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="225b7-121">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="225b7-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="225b7-122">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="225b7-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="225b7-123">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="225b7-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="225b7-124">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="225b7-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="225b7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="225b7-125">Request headers</span></span>

| <span data-ttu-id="225b7-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="225b7-126">Header</span></span>       | <span data-ttu-id="225b7-127">Valor</span><span class="sxs-lookup"><span data-stu-id="225b7-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="225b7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="225b7-128">Authorization</span></span>  | <span data-ttu-id="225b7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="225b7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="225b7-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="225b7-131">ConsistencyLevel</span></span> | <span data-ttu-id="225b7-132">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="225b7-132">eventual.</span></span> <span data-ttu-id="225b7-133">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="225b7-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="225b7-134">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="225b7-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="225b7-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="225b7-135">Request body</span></span>

<span data-ttu-id="225b7-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="225b7-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="225b7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="225b7-137">Response</span></span>

<span data-ttu-id="225b7-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="225b7-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="225b7-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="225b7-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="225b7-140">Exemplo 1: Obter grupos de que o dispositivo é um membro transitivo</span><span class="sxs-lookup"><span data-stu-id="225b7-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="225b7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="225b7-141">Request</span></span>

<span data-ttu-id="225b7-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="225b7-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="225b7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="225b7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="225b7-144">C#</span><span class="sxs-lookup"><span data-stu-id="225b7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="225b7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="225b7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="225b7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="225b7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="225b7-147">Java</span><span class="sxs-lookup"><span data-stu-id="225b7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="225b7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="225b7-148">Response</span></span>

<span data-ttu-id="225b7-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="225b7-149">The following is an example of the response.</span></span>

><span data-ttu-id="225b7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="225b7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="225b7-152">Exemplo 2: Obter apenas uma contagem de todas as associações transitivas</span><span class="sxs-lookup"><span data-stu-id="225b7-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="225b7-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="225b7-153">Request</span></span>

<span data-ttu-id="225b7-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="225b7-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="225b7-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="225b7-155">Response</span></span>

<span data-ttu-id="225b7-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="225b7-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-and-search-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="225b7-157">Exemplo 3: use o OData cast e $search para obter a associação de grupo com nomes de exibição que contêm as letras "Vídeo", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="225b7-157">Example 3: Use OData cast and $search to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="225b7-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="225b7-158">Request</span></span>

<span data-ttu-id="225b7-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="225b7-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="225b7-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="225b7-160">Response</span></span>

<span data-ttu-id="225b7-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="225b7-161">The following is an example of the response.</span></span>

><span data-ttu-id="225b7-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="225b7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="225b7-164">Exemplo 4: use o OData cast e $filter para obter associação com um nome de exibição que começa com "A", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="225b7-164">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="225b7-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="225b7-165">Request</span></span>

<span data-ttu-id="225b7-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="225b7-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="225b7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="225b7-167">Response</span></span>

<span data-ttu-id="225b7-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="225b7-168">The following is an example of the response.</span></span>

><span data-ttu-id="225b7-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="225b7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
}-->
