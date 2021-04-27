---
title: Criar dispositivo
description: Crie um novo dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2c316b2c6a4eac5e37d94b1182c3b3f5bfbce7c9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046941"
---
# <a name="create-device"></a><span data-ttu-id="1359b-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="1359b-103">Create device</span></span>

<span data-ttu-id="1359b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1359b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1359b-105">Crie um novo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1359b-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="1359b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1359b-106">Permissions</span></span>
<span data-ttu-id="1359b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1359b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1359b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1359b-109">Permission type</span></span>      | <span data-ttu-id="1359b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1359b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1359b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1359b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1359b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1359b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1359b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1359b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1359b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1359b-114">Not supported.</span></span>    |
|<span data-ttu-id="1359b-115">Application</span><span class="sxs-lookup"><span data-stu-id="1359b-115">Application</span></span> | <span data-ttu-id="1359b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1359b-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1359b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1359b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="1359b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1359b-118">Request headers</span></span>
| <span data-ttu-id="1359b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1359b-119">Name</span></span>       | <span data-ttu-id="1359b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1359b-120">Type</span></span> | <span data-ttu-id="1359b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1359b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1359b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1359b-122">Authorization</span></span>  | <span data-ttu-id="1359b-123">string</span><span class="sxs-lookup"><span data-stu-id="1359b-123">string</span></span>  | <span data-ttu-id="1359b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1359b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1359b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1359b-126">Request body</span></span>
<span data-ttu-id="1359b-127">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="1359b-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="1359b-128">Como o **recurso de dispositivo** dá suporte a extensões, você pode usar a operação e adicionar propriedades [personalizadas](/graph/extensibility-overview)com seus próprios dados à instância `POST` do dispositivo durante a criação.</span><span class="sxs-lookup"><span data-stu-id="1359b-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="1359b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1359b-129">Response</span></span>

<span data-ttu-id="1359b-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1359b-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1359b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1359b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1359b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1359b-132">Request</span></span>
<span data-ttu-id="1359b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1359b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1359b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1359b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/beta/devices
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
# <a name="c"></a>[<span data-ttu-id="1359b-135">C#</span><span class="sxs-lookup"><span data-stu-id="1359b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1359b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1359b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1359b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1359b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1359b-138">Java</span><span class="sxs-lookup"><span data-stu-id="1359b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1359b-139">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="1359b-139">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1359b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1359b-140">Response</span></span>
<span data-ttu-id="1359b-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1359b-141">Here is an example of the response.</span></span> <span data-ttu-id="1359b-142">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1359b-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="1359b-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="1359b-143">See also</span></span>

- [<span data-ttu-id="1359b-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1359b-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1359b-145">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1359b-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1359b-146">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="1359b-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


