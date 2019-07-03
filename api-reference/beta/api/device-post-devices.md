---
title: Criar dispositivo
description: Criar um novo dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 88c21a7bc977b499c020fc55e2d4d53b229a01f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437226"
---
# <a name="create-device"></a><span data-ttu-id="86c58-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="86c58-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c58-104">Criar um novo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86c58-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="86c58-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86c58-105">Permissions</span></span>
<span data-ttu-id="86c58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="86c58-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86c58-108">Permission type</span></span>      | <span data-ttu-id="86c58-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86c58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86c58-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86c58-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86c58-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86c58-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86c58-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86c58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c58-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86c58-113">Not supported.</span></span>    |
|<span data-ttu-id="86c58-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86c58-114">Application</span></span> | <span data-ttu-id="86c58-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86c58-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86c58-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86c58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="86c58-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86c58-117">Request headers</span></span>
| <span data-ttu-id="86c58-118">Nome</span><span class="sxs-lookup"><span data-stu-id="86c58-118">Name</span></span>       | <span data-ttu-id="86c58-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="86c58-119">Type</span></span> | <span data-ttu-id="86c58-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="86c58-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86c58-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="86c58-121">Authorization</span></span>  | <span data-ttu-id="86c58-122">string</span><span class="sxs-lookup"><span data-stu-id="86c58-122">string</span></span>  | <span data-ttu-id="86c58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86c58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86c58-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86c58-125">Request body</span></span>
<span data-ttu-id="86c58-126">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="86c58-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="86c58-127">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você pode usar `POST` a operação e adicionar propriedades personalizadas com seus próprios dados à instância do dispositivo ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="86c58-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="86c58-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c58-128">Response</span></span>

<span data-ttu-id="86c58-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86c58-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c58-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86c58-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86c58-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86c58-131">Request</span></span>
<span data-ttu-id="86c58-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86c58-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86c58-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="86c58-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="86c58-134">C#</span><span class="sxs-lookup"><span data-stu-id="86c58-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86c58-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="86c58-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86c58-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="86c58-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="86c58-137">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="86c58-137">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="86c58-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c58-138">Response</span></span>
<span data-ttu-id="86c58-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86c58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="86c58-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="86c58-142">See also</span></span>

- [<span data-ttu-id="86c58-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="86c58-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="86c58-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="86c58-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="86c58-145">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="86c58-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
