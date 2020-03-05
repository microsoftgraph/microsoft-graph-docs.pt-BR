---
title: Criar accessPackageResourceRequest
description: Criar um novo accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f5087b313f21fdce39d67d93d814ac1e0a1ee61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441939"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="b2d19-103">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="b2d19-103">Create accessPackageResourceRequest</span></span>

<span data-ttu-id="b2d19-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2d19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d19-105">Criar um novo objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) para solicitar a adição de um recurso a um catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="b2d19-105">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2d19-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2d19-106">Permissions</span></span>

<span data-ttu-id="b2d19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2d19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2d19-109">Permission type</span></span>                        | <span data-ttu-id="b2d19-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2d19-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2d19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2d19-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="b2d19-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d19-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="b2d19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2d19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2d19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d19-114">Not supported.</span></span> |
| <span data-ttu-id="b2d19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2d19-115">Application</span></span>                            | <span data-ttu-id="b2d19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d19-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2d19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d19-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="b2d19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d19-118">Request headers</span></span>

| <span data-ttu-id="b2d19-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b2d19-119">Name</span></span>          | <span data-ttu-id="b2d19-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d19-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b2d19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2d19-121">Authorization</span></span> | <span data-ttu-id="b2d19-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2d19-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2d19-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2d19-124">Content-Type</span></span>  | <span data-ttu-id="b2d19-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2d19-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2d19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d19-127">Request body</span></span>

<span data-ttu-id="b2d19-128">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b2d19-128">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="b2d19-129">Inclua a `accessPackageResource` relação com um objeto [accessPackageResource](../resources/accesspackageresource.md) como parte da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d19-129">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="b2d19-130">Para adicionar um grupo do Azure AD como um recurso a um catálogo, o valor da propriedade **originSystem** dentro do `accessPackageResource` deve ser **AadGroup** e o valor de **originid** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="b2d19-130">To add an Azure AD group as a resource to a catalog, the value of the **originSystem** property within the `accessPackageResource` should be **AadGroup** and the value of the **originId** is the identifier of the group.</span></span>


## <a name="response"></a><span data-ttu-id="b2d19-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d19-131">Response</span></span>

<span data-ttu-id="b2d19-132">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d19-132">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2d19-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b2d19-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2d19-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d19-134">Request</span></span>

<span data-ttu-id="b2d19-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d19-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2d19-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d19-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b2d19-137">C#</span><span class="sxs-lookup"><span data-stu-id="b2d19-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerequest-from-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2d19-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2d19-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerequest-from-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2d19-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2d19-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerequest-from-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2d19-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d19-140">Response</span></span>

<span data-ttu-id="b2d19-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d19-141">The following is an example of the response.</span></span>

> <span data-ttu-id="b2d19-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2d19-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
