---
title: Criar dispositivo
description: Cria e registra um novo dispositivo na organização.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3b3496fd232af5c7f6397aa7a9c538a8b0532737
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051505"
---
# <a name="create-device"></a><span data-ttu-id="e317f-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="e317f-103">Create device</span></span>

<span data-ttu-id="e317f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e317f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e317f-105">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="e317f-105">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e317f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e317f-106">Permissions</span></span>
<span data-ttu-id="e317f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e317f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e317f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e317f-109">Permission type</span></span>      | <span data-ttu-id="e317f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e317f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e317f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e317f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e317f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e317f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e317f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e317f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e317f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e317f-114">Not supported.</span></span>    |
|<span data-ttu-id="e317f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e317f-115">Application</span></span> | <span data-ttu-id="e317f-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e317f-116">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e317f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e317f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="e317f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e317f-118">Request headers</span></span>
| <span data-ttu-id="e317f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e317f-119">Name</span></span>       | <span data-ttu-id="e317f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e317f-120">Type</span></span> | <span data-ttu-id="e317f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e317f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e317f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e317f-122">Authorization</span></span>  | <span data-ttu-id="e317f-123">string</span><span class="sxs-lookup"><span data-stu-id="e317f-123">string</span></span>  | <span data-ttu-id="e317f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e317f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e317f-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="e317f-126">Content-type</span></span> | <span data-ttu-id="e317f-127">string</span><span class="sxs-lookup"><span data-stu-id="e317f-127">string</span></span> | <span data-ttu-id="e317f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e317f-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e317f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e317f-129">Request body</span></span>
<span data-ttu-id="e317f-130">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="e317f-130">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e317f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e317f-131">Response</span></span>

<span data-ttu-id="e317f-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e317f-132">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e317f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e317f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e317f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e317f-134">Request</span></span>
<span data-ttu-id="e317f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e317f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e317f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e317f-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e317f-137">C#</span><span class="sxs-lookup"><span data-stu-id="e317f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e317f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e317f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e317f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e317f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e317f-140">Java</span><span class="sxs-lookup"><span data-stu-id="e317f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e317f-141">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="e317f-141">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e317f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e317f-142">Response</span></span>
<span data-ttu-id="e317f-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e317f-143">Here is an example of the response.</span></span> <span data-ttu-id="e317f-144">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e317f-144">Note: The response object shown here might be shortened for readability.</span></span>
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

