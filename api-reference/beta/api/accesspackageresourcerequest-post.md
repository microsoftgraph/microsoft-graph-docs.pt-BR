---
title: Criar accessPackageResourceRequest
description: Criar um novo accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46b40c4650890db6a506fce0c8422cea07a4f5c1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871706"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="8145f-103">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="8145f-103">Create accessPackageResourceRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8145f-104">Criar um novo objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) para solicitar a adição de um recurso a um catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="8145f-104">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="8145f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8145f-105">Permissions</span></span>

<span data-ttu-id="8145f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8145f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8145f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8145f-108">Permission type</span></span>                        | <span data-ttu-id="8145f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8145f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8145f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8145f-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="8145f-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8145f-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="8145f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8145f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8145f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8145f-113">Not supported.</span></span> |
| <span data-ttu-id="8145f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8145f-114">Application</span></span>                            | <span data-ttu-id="8145f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8145f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8145f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8145f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="8145f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8145f-117">Request headers</span></span>

| <span data-ttu-id="8145f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8145f-118">Name</span></span>          | <span data-ttu-id="8145f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8145f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8145f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8145f-120">Authorization</span></span> | <span data-ttu-id="8145f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8145f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8145f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8145f-123">Content-Type</span></span>  | <span data-ttu-id="8145f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8145f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8145f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8145f-126">Request body</span></span>

<span data-ttu-id="8145f-127">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8145f-127">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="8145f-128">Inclua a `accessPackageResource` relação com um objeto [accessPackageResource](../resources/accesspackageresource.md) como parte da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8145f-128">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="8145f-129">Para adicionar um grupo do Azure AD como um recurso a um catálogo, o valor da propriedade **originSystem** dentro do `accessPackageResource` deve ser **AadGroup** e o valor de **originid** é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="8145f-129">To add an Azure AD group as a resource to a catalog, the value of the **originSystem** property within the `accessPackageResource` should be **AadGroup** and the value of the **originId** is the identifier of the group.</span></span>


## <a name="response"></a><span data-ttu-id="8145f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8145f-130">Response</span></span>

<span data-ttu-id="8145f-131">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8145f-131">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8145f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8145f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8145f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8145f-133">Request</span></span>

<span data-ttu-id="8145f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8145f-134">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8145f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8145f-135">Response</span></span>

<span data-ttu-id="8145f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8145f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="8145f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8145f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
