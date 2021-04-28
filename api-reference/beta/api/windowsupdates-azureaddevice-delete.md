---
title: Excluir azureADDevice
description: Exclua um objeto azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6cb9d23b01241878eff96e7301f8322baa7f0fb0
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067779"
---
# <a name="delete-azureaddevice"></a><span data-ttu-id="da810-103">Excluir azureADDevice</span><span class="sxs-lookup"><span data-stu-id="da810-103">Delete azureADDevice</span></span>
<span data-ttu-id="da810-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="da810-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da810-105">[Exclua um objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="da810-105">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

<span data-ttu-id="da810-106">Quando um dispositivo do Azure AD é excluído, ele é desastrado do serviço de implantação e automaticamente desinteressado do gerenciamento pelo serviço para todas as categorias de atualização, bem como removido de todas as [implantaçõesAudiência](../resources/windowsupdates-deploymentaudience.md) e [updateableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="da810-106">When an Azure AD device is deleted, it is unregistered from the deployment service and automatically unenrolled from management by the service for all update categories, as well as removed from every [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="da810-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="da810-107">Permissions</span></span>
<span data-ttu-id="da810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da810-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da810-110">Permission type</span></span>|<span data-ttu-id="da810-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da810-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da810-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da810-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da810-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da810-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="da810-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da810-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da810-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da810-115">Not supported.</span></span>|
|<span data-ttu-id="da810-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da810-116">Application</span></span>|<span data-ttu-id="da810-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da810-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da810-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da810-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="da810-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da810-119">Request headers</span></span>
|<span data-ttu-id="da810-120">Nome</span><span class="sxs-lookup"><span data-stu-id="da810-120">Name</span></span>|<span data-ttu-id="da810-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="da810-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da810-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="da810-122">Authorization</span></span>|<span data-ttu-id="da810-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da810-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da810-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da810-125">Request body</span></span>
<span data-ttu-id="da810-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da810-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da810-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="da810-127">Response</span></span>

<span data-ttu-id="da810-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da810-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da810-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da810-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da810-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da810-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_azureaddevice"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a><span data-ttu-id="da810-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="da810-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

