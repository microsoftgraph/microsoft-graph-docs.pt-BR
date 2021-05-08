---
title: Excluir azureADDevice
description: Exclua um objeto azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 82e457f433ab3e307eaf727dc09d18144f3dd844
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241440"
---
# <a name="delete-azureaddevice"></a><span data-ttu-id="93dd4-103">Excluir azureADDevice</span><span class="sxs-lookup"><span data-stu-id="93dd4-103">Delete azureADDevice</span></span>
<span data-ttu-id="93dd4-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="93dd4-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93dd4-105">[Exclua um objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="93dd4-105">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

<span data-ttu-id="93dd4-106">Quando um dispositivo do Azure AD é excluído, ele é desastrado do serviço de implantação e automaticamente desinteressado do gerenciamento pelo serviço para todas as categorias de atualização, bem como removido de todas as [implantaçõesAudiência](../resources/windowsupdates-deploymentaudience.md) e [updateableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="93dd4-106">When an Azure AD device is deleted, it is unregistered from the deployment service and automatically unenrolled from management by the service for all update categories, as well as removed from every [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93dd4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="93dd4-107">Permissions</span></span>
<span data-ttu-id="93dd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93dd4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93dd4-110">Permission type</span></span>|<span data-ttu-id="93dd4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93dd4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93dd4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93dd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93dd4-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93dd4-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="93dd4-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93dd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93dd4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93dd4-115">Not supported.</span></span>|
|<span data-ttu-id="93dd4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93dd4-116">Application</span></span>|<span data-ttu-id="93dd4-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93dd4-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93dd4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93dd4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="93dd4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93dd4-119">Request headers</span></span>
|<span data-ttu-id="93dd4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="93dd4-120">Name</span></span>|<span data-ttu-id="93dd4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="93dd4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="93dd4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="93dd4-122">Authorization</span></span>|<span data-ttu-id="93dd4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93dd4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93dd4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93dd4-125">Request body</span></span>
<span data-ttu-id="93dd4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93dd4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93dd4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="93dd4-127">Response</span></span>

<span data-ttu-id="93dd4-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93dd4-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93dd4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93dd4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93dd4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93dd4-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="93dd4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="93dd4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_azureaddevice"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```
# <a name="c"></a>[<span data-ttu-id="93dd4-133">C#</span><span class="sxs-lookup"><span data-stu-id="93dd4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-azureaddevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93dd4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93dd4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-azureaddevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93dd4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93dd4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-azureaddevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93dd4-136">Java</span><span class="sxs-lookup"><span data-stu-id="93dd4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-azureaddevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93dd4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="93dd4-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

