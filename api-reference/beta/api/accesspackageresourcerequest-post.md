---
title: Criar accessPackageResourceRequest
description: Crie um novo accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e7ea15dbe0ec63e539246851ce853b83c40229aa
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934533"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="bdcf4-103">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="bdcf4-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="bdcf4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdcf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdcf4-105">Crie um novo [objeto accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) para solicitar a adição de um recurso a um catálogo de pacotes de acesso ou a remoção de um recurso de um catálogo.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog, or the removal of a resource from a catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdcf4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdcf4-106">Permissions</span></span>

<span data-ttu-id="bdcf4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdcf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdcf4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdcf4-109">Permission type</span></span>                        | <span data-ttu-id="bdcf4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdcf4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdcf4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdcf4-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="bdcf4-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcf4-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="bdcf4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdcf4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdcf4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-114">Not supported.</span></span> |
| <span data-ttu-id="bdcf4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdcf4-115">Application</span></span>                            | <span data-ttu-id="bdcf4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdcf4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdcf4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="bdcf4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcf4-118">Request headers</span></span>

| <span data-ttu-id="bdcf4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bdcf4-119">Name</span></span>          | <span data-ttu-id="bdcf4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdcf4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bdcf4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdcf4-121">Authorization</span></span> | <span data-ttu-id="bdcf4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdcf4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdcf4-124">Content-Type</span></span>  | <span data-ttu-id="bdcf4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bdcf4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcf4-127">Request body</span></span>

<span data-ttu-id="bdcf4-128">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageResourceRequest.](../resources/accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="bdcf4-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="bdcf4-129">Inclua a `accessPackageResource` relação com um objeto [accessPackageResource](../resources/accesspackageresource.md) como parte da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="bdcf4-130">Para adicionar um grupo do Azure AD como um recurso a um catálogo, de definida **a catalogId** como sendo da ID do catálogo, **requestType** como e uma representa o `AdminAdd` `accessPackageResource` recurso.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-130">To add an Azure AD group as a resource to a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminAdd`, and an `accessPackageResource` representing the resource.</span></span> <span data-ttu-id="bdcf4-131">O valor da **propriedade originSystem** dentro do deve ser e o valor de `accessPackageResource` `AadGroup` **originId** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-131">The value of the **originSystem** property within the `accessPackageResource` should be `AadGroup` and the value of the **originId** is the identifier of the group.</span></span>

<span data-ttu-id="bdcf4-132">Para remover um aplicativo do Azure AD de um catálogo, de definida **a catalogId** como sendo da ID do catálogo, **requestType** como e o objeto de recurso a ser `AdminRemove` `accessPackageResource` removido.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-132">To remove an Azure AD app from a catalog, set the **catalogId** to be of the ID of the catalog, **requestType** to be `AdminRemove`, and the `accessPackageResource` the resource object to be removed.</span></span>  <span data-ttu-id="bdcf4-133">O objeto de recurso pode ser recuperado usando [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span><span class="sxs-lookup"><span data-stu-id="bdcf4-133">The resource object can be retrieved using [list accessPackageResources](accesspackagecatalog-list-accesspackageresources.md).</span></span>


## <a name="response"></a><span data-ttu-id="bdcf4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdcf4-134">Response</span></span>

<span data-ttu-id="bdcf4-135">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-135">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdcf4-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bdcf4-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdcf4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdcf4-137">Request</span></span>

<span data-ttu-id="bdcf4-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdcf4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdcf4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
     "displayName": "Sales",
     "description": "https://contoso.sharepoint.com/sites/Sales",
     "url": "https://contoso.sharepoint.com/sites/Sales",
     "resourceType": "SharePoint Online Site",
     "originId": "https://contoso.sharepoint.com/sites/Sales",
     "originSystem": "SharePointOnline"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="bdcf4-140">C#</span><span class="sxs-lookup"><span data-stu-id="bdcf4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdcf4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdcf4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdcf4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdcf4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bdcf4-143">Java</span><span class="sxs-lookup"><span data-stu-id="bdcf4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerequest-from-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bdcf4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdcf4-144">Response</span></span>

<span data-ttu-id="bdcf4-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-145">The following is an example of the response.</span></span>

> <span data-ttu-id="bdcf4-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdcf4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


