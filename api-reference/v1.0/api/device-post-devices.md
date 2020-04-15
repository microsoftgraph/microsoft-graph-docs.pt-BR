---
title: Criar dispositivo
description: Cria e registra um novo dispositivo na organização.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 396d74e2ef423b8efd61877b1a2b1fd8fdeee371
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466708"
---
# <a name="create-device"></a><span data-ttu-id="7da37-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="7da37-103">Create device</span></span>

<span data-ttu-id="7da37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7da37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7da37-105">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="7da37-105">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="7da37-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7da37-106">Permissions</span></span>
<span data-ttu-id="7da37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7da37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7da37-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7da37-109">Permission type</span></span>      | <span data-ttu-id="7da37-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7da37-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7da37-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7da37-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7da37-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7da37-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7da37-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7da37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7da37-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7da37-114">Not supported.</span></span>    |
|<span data-ttu-id="7da37-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7da37-115">Application</span></span> | <span data-ttu-id="7da37-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da37-116">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7da37-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7da37-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="7da37-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7da37-118">Request headers</span></span>
| <span data-ttu-id="7da37-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7da37-119">Name</span></span>       | <span data-ttu-id="7da37-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7da37-120">Type</span></span> | <span data-ttu-id="7da37-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da37-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7da37-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7da37-122">Authorization</span></span>  | <span data-ttu-id="7da37-123">string</span><span class="sxs-lookup"><span data-stu-id="7da37-123">string</span></span>  | <span data-ttu-id="7da37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7da37-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7da37-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7da37-126">Content-type</span></span> | <span data-ttu-id="7da37-127">string</span><span class="sxs-lookup"><span data-stu-id="7da37-127">string</span></span> | <span data-ttu-id="7da37-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7da37-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7da37-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7da37-129">Request body</span></span>
<span data-ttu-id="7da37-130">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="7da37-130">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7da37-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da37-131">Response</span></span>

<span data-ttu-id="7da37-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7da37-132">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7da37-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7da37-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7da37-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7da37-134">Request</span></span>
<span data-ttu-id="7da37-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7da37-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7da37-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7da37-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7da37-137">C#</span><span class="sxs-lookup"><span data-stu-id="7da37-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7da37-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7da37-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7da37-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7da37-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7da37-140">Java</span><span class="sxs-lookup"><span data-stu-id="7da37-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7da37-141">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="7da37-141">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7da37-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7da37-142">Response</span></span>
<span data-ttu-id="7da37-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7da37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
