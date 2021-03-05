---
title: Criar dispositivo
description: Cria e registra um novo dispositivo na organização.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 89e4b54e91cb027d88b36c426da8146f98fce781
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434528"
---
# <a name="create-device"></a><span data-ttu-id="9d74e-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="9d74e-103">Create device</span></span>

<span data-ttu-id="9d74e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d74e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d74e-105">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="9d74e-105">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d74e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d74e-106">Permissions</span></span>
<span data-ttu-id="9d74e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d74e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d74e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d74e-109">Permission type</span></span>      | <span data-ttu-id="9d74e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d74e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d74e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d74e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d74e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d74e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d74e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d74e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d74e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d74e-114">Not supported.</span></span>    |
|<span data-ttu-id="9d74e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d74e-115">Application</span></span> | <span data-ttu-id="9d74e-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d74e-116">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d74e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d74e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="9d74e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d74e-118">Request headers</span></span>
| <span data-ttu-id="9d74e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9d74e-119">Name</span></span>       | <span data-ttu-id="9d74e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d74e-120">Type</span></span> | <span data-ttu-id="9d74e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d74e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d74e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d74e-122">Authorization</span></span>  | <span data-ttu-id="9d74e-123">string</span><span class="sxs-lookup"><span data-stu-id="9d74e-123">string</span></span>  | <span data-ttu-id="9d74e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d74e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d74e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="9d74e-126">Content-type</span></span> | <span data-ttu-id="9d74e-127">string</span><span class="sxs-lookup"><span data-stu-id="9d74e-127">string</span></span> | <span data-ttu-id="9d74e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9d74e-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d74e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d74e-129">Request body</span></span>
<span data-ttu-id="9d74e-130">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="9d74e-130">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9d74e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d74e-131">Response</span></span>

<span data-ttu-id="9d74e-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d74e-132">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d74e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d74e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d74e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d74e-134">Request</span></span>
<span data-ttu-id="9d74e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d74e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d74e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d74e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
# <a name="c"></a>[<span data-ttu-id="9d74e-137">C#</span><span class="sxs-lookup"><span data-stu-id="9d74e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d74e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d74e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d74e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d74e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d74e-140">Java</span><span class="sxs-lookup"><span data-stu-id="9d74e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9d74e-141">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="9d74e-141">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9d74e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d74e-142">Response</span></span>
<span data-ttu-id="9d74e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d74e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

