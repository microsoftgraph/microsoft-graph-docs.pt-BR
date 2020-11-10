---
title: Criar dispositivo
description: Criar um novo dispositivo.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: df785c6555c7b7cbcec3fe59421ebcc326e72fb4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963419"
---
# <a name="create-device"></a><span data-ttu-id="a9de4-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="a9de4-103">Create device</span></span>

<span data-ttu-id="a9de4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9de4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9de4-105">Criar um novo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9de4-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9de4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9de4-106">Permissions</span></span>
<span data-ttu-id="a9de4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9de4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9de4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9de4-109">Permission type</span></span>      | <span data-ttu-id="a9de4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9de4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9de4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9de4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9de4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9de4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9de4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9de4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9de4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9de4-114">Not supported.</span></span>    |
|<span data-ttu-id="a9de4-115">Application</span><span class="sxs-lookup"><span data-stu-id="a9de4-115">Application</span></span> | <span data-ttu-id="a9de4-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9de4-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9de4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9de4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="a9de4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9de4-118">Request headers</span></span>
| <span data-ttu-id="a9de4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a9de4-119">Name</span></span>       | <span data-ttu-id="a9de4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9de4-120">Type</span></span> | <span data-ttu-id="a9de4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9de4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9de4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9de4-122">Authorization</span></span>  | <span data-ttu-id="a9de4-123">string</span><span class="sxs-lookup"><span data-stu-id="a9de4-123">string</span></span>  | <span data-ttu-id="a9de4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9de4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9de4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9de4-126">Request body</span></span>
<span data-ttu-id="a9de4-127">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="a9de4-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="a9de4-128">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância do dispositivo ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="a9de4-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="a9de4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9de4-129">Response</span></span>

<span data-ttu-id="a9de4-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9de4-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9de4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9de4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9de4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9de4-132">Request</span></span>
<span data-ttu-id="a9de4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9de4-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9de4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9de4-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a9de4-135">C#</span><span class="sxs-lookup"><span data-stu-id="a9de4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9de4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9de4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9de4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9de4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9de4-138">Java</span><span class="sxs-lookup"><span data-stu-id="a9de4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a9de4-139">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="a9de4-139">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a9de4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9de4-140">Response</span></span>
<span data-ttu-id="a9de4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9de4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a9de4-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="a9de4-144">See also</span></span>

- [<span data-ttu-id="a9de4-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a9de4-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a9de4-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="a9de4-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a9de4-147">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="a9de4-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


