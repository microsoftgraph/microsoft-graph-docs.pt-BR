---
title: Excluir cloudPcUserSetting
description: Exclua um objeto cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6f434d4536eff7361311ad20d2bc17498b700af3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207830"
---
# <a name="delete-cloudpcusersetting"></a><span data-ttu-id="c5dc3-103">Excluir cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="c5dc3-103">Delete cloudPcUserSetting</span></span>

<span data-ttu-id="c5dc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5dc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5dc3-105">[Exclua um objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="c5dc3-105">Delete a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="c5dc3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5dc3-106">Permissions</span></span>

<span data-ttu-id="c5dc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5dc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5dc3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5dc3-109">Permission type</span></span>|<span data-ttu-id="c5dc3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5dc3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5dc3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5dc3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c5dc3-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5dc3-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c5dc3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5dc3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5dc3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5dc3-114">Not supported.</span></span>|
|<span data-ttu-id="c5dc3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5dc3-115">Application</span></span>|<span data-ttu-id="c5dc3-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5dc3-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5dc3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5dc3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c5dc3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5dc3-118">Request headers</span></span>
|<span data-ttu-id="c5dc3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c5dc3-119">Name</span></span>|<span data-ttu-id="c5dc3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5dc3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5dc3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5dc3-121">Authorization</span></span>|<span data-ttu-id="c5dc3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5dc3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5dc3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5dc3-124">Request body</span></span>
<span data-ttu-id="c5dc3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5dc3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5dc3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5dc3-126">Response</span></span>

<span data-ttu-id="c5dc3-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c5dc3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c5dc3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5dc3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5dc3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5dc3-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c5dc3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5dc3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_cloudpcusersetting"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
```
# <a name="c"></a>[<span data-ttu-id="c5dc3-131">C#</span><span class="sxs-lookup"><span data-stu-id="c5dc3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5dc3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5dc3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5dc3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5dc3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5dc3-134">Java</span><span class="sxs-lookup"><span data-stu-id="c5dc3-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c5dc3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5dc3-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
