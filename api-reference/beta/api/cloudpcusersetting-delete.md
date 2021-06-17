---
title: Excluir cloudPcUserSetting
description: Exclua um objeto cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a3a6c5b7c7c75b89d1c27adcf7b123788f5cfe51
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993633"
---
# <a name="delete-cloudpcusersetting"></a><span data-ttu-id="a4585-103">Excluir cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="a4585-103">Delete cloudPcUserSetting</span></span>

<span data-ttu-id="a4585-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4585-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4585-105">[Exclua um objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="a4585-105">Delete a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="a4585-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a4585-106">Permissions</span></span>

<span data-ttu-id="a4585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4585-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4585-109">Permission type</span></span>|<span data-ttu-id="a4585-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4585-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4585-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4585-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4585-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4585-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a4585-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4585-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4585-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4585-114">Not supported.</span></span>|
|<span data-ttu-id="a4585-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4585-115">Application</span></span>|<span data-ttu-id="a4585-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4585-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4585-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4585-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a4585-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4585-118">Request headers</span></span>
|<span data-ttu-id="a4585-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a4585-119">Name</span></span>|<span data-ttu-id="a4585-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4585-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4585-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4585-121">Authorization</span></span>|<span data-ttu-id="a4585-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4585-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4585-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4585-124">Request body</span></span>
<span data-ttu-id="a4585-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4585-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4585-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4585-126">Response</span></span>

<span data-ttu-id="a4585-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4585-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a4585-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4585-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4585-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4585-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_cloudpcusersetting"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
```


### <a name="response"></a><span data-ttu-id="a4585-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4585-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
