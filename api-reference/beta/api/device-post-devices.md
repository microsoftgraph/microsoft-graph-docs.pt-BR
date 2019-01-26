---
title: Criar dispositivo
description: Crie um novo dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30c4852d3e44e9318fef38018f1a99823e362112
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577057"
---
# <a name="create-device"></a><span data-ttu-id="1e4c0-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e4c0-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e4c0-104">Crie um novo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e4c0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e4c0-105">Permissions</span></span>
<span data-ttu-id="1e4c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e4c0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e4c0-108">Permission type</span></span>      | <span data-ttu-id="1e4c0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e4c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e4c0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e4c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e4c0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e4c0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e4c0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e4c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e4c0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-113">Not supported.</span></span>    |
|<span data-ttu-id="1e4c0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e4c0-114">Application</span></span> | <span data-ttu-id="1e4c0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4c0-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e4c0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e4c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="1e4c0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4c0-117">Request headers</span></span>
| <span data-ttu-id="1e4c0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1e4c0-118">Name</span></span>       | <span data-ttu-id="1e4c0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e4c0-119">Type</span></span> | <span data-ttu-id="1e4c0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4c0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e4c0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e4c0-121">Authorization</span></span>  | <span data-ttu-id="1e4c0-122">string</span><span class="sxs-lookup"><span data-stu-id="1e4c0-122">string</span></span>  | <span data-ttu-id="1e4c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e4c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4c0-125">Request body</span></span>
<span data-ttu-id="1e4c0-126">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="1e4c0-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="1e4c0-127">Desde que o recurso de **dispositivo** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância de dispositivo ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="1e4c0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4c0-128">Response</span></span>

<span data-ttu-id="1e4c0-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4c0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e4c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e4c0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4c0-131">Request</span></span>
<span data-ttu-id="1e4c0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-132">Here is an example of the request.</span></span>
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
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
<span data-ttu-id="1e4c0-133">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="1e4c0-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1e4c0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4c0-134">Response</span></span>
<span data-ttu-id="1e4c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e4c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "key": "binary"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="1e4c0-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="1e4c0-138">See also</span></span>

- [<span data-ttu-id="1e4c0-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1e4c0-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1e4c0-140">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1e4c0-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1e4c0-141">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="1e4c0-141">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
