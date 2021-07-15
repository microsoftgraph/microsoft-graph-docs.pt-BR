---
title: Excluir mobileDeviceManagementPolicy
description: Exclua uma política de gerenciamento de dispositivo móvel.
author: michaelrm97
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4ec86977e3abbb704098936051995e28ebace5c0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440700"
---
# <a name="delete-mobiledevicemanagementpolicy"></a><span data-ttu-id="f7618-103">Excluir mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f7618-103">Delete mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="f7618-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7618-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7618-105">[Exclua um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f7618-105">Delete a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="f7618-106">Essa operação só é suportada quando a política não é mais válida; ou seja, quando a **propriedade isValid** for false, o que indica que a entidade de serviço associada ao aplicativo para essa política foi excluída.</span><span class="sxs-lookup"><span data-stu-id="f7618-106">This operation is only supported when the policy is no longer valid; that is, when the **isValid** property is false, which indicates that the service principal associated with the application for this policy has been deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7618-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f7618-107">Permissions</span></span>

<span data-ttu-id="f7618-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7618-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7618-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7618-110">Permission type</span></span>|<span data-ttu-id="f7618-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7618-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7618-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7618-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7618-113">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="f7618-113">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="f7618-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7618-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7618-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7618-115">Not supported.</span></span>|
|<span data-ttu-id="f7618-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7618-116">Application</span></span> | <span data-ttu-id="f7618-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7618-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7618-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7618-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7618-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7618-119">Request headers</span></span>

|<span data-ttu-id="f7618-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7618-120">Name</span></span>|<span data-ttu-id="f7618-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7618-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7618-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7618-122">Authorization</span></span>|<span data-ttu-id="f7618-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7618-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7618-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7618-125">Request body</span></span>

<span data-ttu-id="f7618-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7618-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7618-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7618-127">Response</span></span>

<span data-ttu-id="f7618-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7618-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7618-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7618-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7618-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7618-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f7618-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7618-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mobilitymanagementpolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```
# <a name="c"></a>[<span data-ttu-id="f7618-133">C#</span><span class="sxs-lookup"><span data-stu-id="f7618-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7618-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7618-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7618-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7618-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7618-136">Java</span><span class="sxs-lookup"><span data-stu-id="f7618-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7618-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7618-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
