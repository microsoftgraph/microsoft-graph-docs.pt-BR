---
title: Criar dispositivo
description: Cria e registra um novo dispositivo na organização.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3fcaaa3e2da274848495eb0dfbb259ed4200db87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002962"
---
# <a name="create-device"></a><span data-ttu-id="4d952-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="4d952-103">Create device</span></span>

<span data-ttu-id="4d952-104">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="4d952-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d952-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d952-105">Permissions</span></span>
<span data-ttu-id="4d952-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d952-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d952-108">Permission type</span></span>      | <span data-ttu-id="4d952-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d952-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d952-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d952-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d952-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d952-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d952-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d952-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d952-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d952-113">Not supported.</span></span>    |
|<span data-ttu-id="4d952-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d952-114">Application</span></span> | <span data-ttu-id="4d952-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d952-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d952-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d952-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="4d952-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d952-117">Request headers</span></span>
| <span data-ttu-id="4d952-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4d952-118">Name</span></span>       | <span data-ttu-id="4d952-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d952-119">Type</span></span> | <span data-ttu-id="4d952-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d952-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d952-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d952-121">Authorization</span></span>  | <span data-ttu-id="4d952-122">string</span><span class="sxs-lookup"><span data-stu-id="4d952-122">string</span></span>  | <span data-ttu-id="4d952-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d952-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d952-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4d952-125">Content-type</span></span> | <span data-ttu-id="4d952-126">string</span><span class="sxs-lookup"><span data-stu-id="4d952-126">string</span></span> | <span data-ttu-id="4d952-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4d952-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d952-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d952-128">Request body</span></span>
<span data-ttu-id="4d952-129">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="4d952-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d952-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d952-130">Response</span></span>

<span data-ttu-id="4d952-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d952-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d952-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d952-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d952-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d952-133">Request</span></span>
<span data-ttu-id="4d952-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d952-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d952-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d952-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d952-136">C#</span><span class="sxs-lookup"><span data-stu-id="4d952-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d952-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d952-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d952-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d952-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4d952-139">Java</span><span class="sxs-lookup"><span data-stu-id="4d952-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4d952-140">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="4d952-140">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4d952-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d952-141">Response</span></span>
<span data-ttu-id="4d952-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d952-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
