---
title: Criar dispositivo
description: Crie um novo dispositivo.
ms.openlocfilehash: 33dc1f8da40e29e8c135cf24f35ec3ce52af9b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037788"
---
# <a name="create-device"></a><span data-ttu-id="88047-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="88047-103">Create device</span></span>

> <span data-ttu-id="88047-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="88047-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88047-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="88047-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88047-106">Crie um novo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88047-106">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="88047-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="88047-107">Permissions</span></span>
<span data-ttu-id="88047-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88047-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88047-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88047-110">Permission type</span></span>      | <span data-ttu-id="88047-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88047-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88047-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88047-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88047-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88047-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88047-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88047-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88047-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88047-115">Not supported.</span></span>    |
|<span data-ttu-id="88047-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88047-116">Application</span></span> | <span data-ttu-id="88047-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88047-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88047-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88047-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="88047-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88047-119">Request headers</span></span>
| <span data-ttu-id="88047-120">Nome</span><span class="sxs-lookup"><span data-stu-id="88047-120">Name</span></span>       | <span data-ttu-id="88047-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="88047-121">Type</span></span> | <span data-ttu-id="88047-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="88047-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88047-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88047-123">Authorization</span></span>  | <span data-ttu-id="88047-124">string</span><span class="sxs-lookup"><span data-stu-id="88047-124">string</span></span>  | <span data-ttu-id="88047-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88047-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88047-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88047-127">Request body</span></span>
<span data-ttu-id="88047-128">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="88047-128">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="88047-129">Desde que o recurso de **dispositivo** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `POST` operação e adicionar propriedades personalizadas com seus próprios dados à instância de dispositivo ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="88047-129">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="88047-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="88047-130">Response</span></span>

<span data-ttu-id="88047-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88047-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88047-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88047-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88047-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88047-133">Request</span></span>
<span data-ttu-id="88047-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88047-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="88047-135">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="88047-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="88047-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="88047-136">Response</span></span>
<span data-ttu-id="88047-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88047-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="88047-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="88047-140">See also</span></span>

- [<span data-ttu-id="88047-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="88047-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="88047-142">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="88047-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="88047-143">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="88047-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->