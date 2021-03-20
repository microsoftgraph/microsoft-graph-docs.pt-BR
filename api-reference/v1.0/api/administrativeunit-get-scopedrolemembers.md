---
title: Obter um scopedRoleMember
description: Recupere um recurso scopedRoleMembership específico.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8bd98416a3c1c62303c806021876038dd46e246a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945570"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="b0344-103">Obter um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="b0344-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="b0344-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0344-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0344-105">Recupere um recurso [scopedRoleMembership](../resources/scopedrolemembership.md) específico.</span><span class="sxs-lookup"><span data-stu-id="b0344-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0344-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0344-106">Permissions</span></span>
<span data-ttu-id="b0344-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0344-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0344-109">Permission type</span></span>      | <span data-ttu-id="b0344-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0344-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0344-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0344-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0344-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0344-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0344-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0344-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0344-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0344-114">Not supported.</span></span>    |
|<span data-ttu-id="b0344-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0344-115">Application</span></span> | <span data-ttu-id="b0344-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0344-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0344-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0344-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0344-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0344-118">Optional query parameters</span></span>
<span data-ttu-id="b0344-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0344-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0344-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0344-120">Request headers</span></span>
| <span data-ttu-id="b0344-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b0344-121">Name</span></span>      |<span data-ttu-id="b0344-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0344-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0344-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0344-123">Authorization</span></span>  | <span data-ttu-id="b0344-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0344-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0344-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0344-126">Request body</span></span>
<span data-ttu-id="b0344-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0344-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0344-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0344-128">Response</span></span>

<span data-ttu-id="b0344-129">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0344-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0344-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0344-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0344-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0344-131">Request</span></span>
<span data-ttu-id="b0344-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0344-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b0344-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0344-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="b0344-134">C#</span><span class="sxs-lookup"><span data-stu-id="b0344-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0344-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0344-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0344-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0344-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0344-137">Java</span><span class="sxs-lookup"><span data-stu-id="b0344-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="b0344-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0344-138">Response</span></span>
<span data-ttu-id="b0344-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0344-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
