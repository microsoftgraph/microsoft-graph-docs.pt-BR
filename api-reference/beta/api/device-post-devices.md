---
title: Criar dispositivo
description: Criar um novo dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 60a3e3bf2e44d975e1c3dc8383e0320a9906eda7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326063"
---
# <a name="create-device"></a><span data-ttu-id="e172a-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="e172a-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e172a-104">Criar um novo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e172a-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="e172a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e172a-105">Permissions</span></span>
<span data-ttu-id="e172a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e172a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e172a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e172a-108">Permission type</span></span>      | <span data-ttu-id="e172a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e172a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e172a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e172a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e172a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e172a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e172a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e172a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e172a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e172a-113">Not supported.</span></span>    |
|<span data-ttu-id="e172a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e172a-114">Application</span></span> | <span data-ttu-id="e172a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e172a-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e172a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e172a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="e172a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e172a-117">Request headers</span></span>
| <span data-ttu-id="e172a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e172a-118">Name</span></span>       | <span data-ttu-id="e172a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e172a-119">Type</span></span> | <span data-ttu-id="e172a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e172a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e172a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e172a-121">Authorization</span></span>  | <span data-ttu-id="e172a-122">string</span><span class="sxs-lookup"><span data-stu-id="e172a-122">string</span></span>  | <span data-ttu-id="e172a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e172a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e172a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e172a-125">Request body</span></span>
<span data-ttu-id="e172a-126">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="e172a-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="e172a-127">Como o recurso de **dispositivo** suporta [extensões](/graph/extensibility-overview), você pode usar `POST` a operação e adicionar propriedades personalizadas com seus próprios dados à instância do dispositivo ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="e172a-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e172a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e172a-128">Response</span></span>

<span data-ttu-id="e172a-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e172a-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e172a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e172a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e172a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e172a-131">Request</span></span>
<span data-ttu-id="e172a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e172a-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="e172a-133">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="e172a-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e172a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e172a-134">Response</span></span>
<span data-ttu-id="e172a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e172a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e172a-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="e172a-138">See also</span></span>

- [<span data-ttu-id="e172a-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="e172a-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e172a-140">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="e172a-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e172a-141">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="e172a-141">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
