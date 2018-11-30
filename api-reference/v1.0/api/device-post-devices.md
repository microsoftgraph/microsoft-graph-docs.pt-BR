---
title: Criar dispositivo
description: Cria e registra um novo dispositivo na organização.
ms.openlocfilehash: 7dd4ab48c66383990eb3fca4630717ba8063c67a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005105"
---
# <a name="create-device"></a><span data-ttu-id="09cad-103">Criar dispositivo</span><span class="sxs-lookup"><span data-stu-id="09cad-103">Create device</span></span>

<span data-ttu-id="09cad-104">Cria e registra um novo dispositivo na organização.</span><span class="sxs-lookup"><span data-stu-id="09cad-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="09cad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09cad-105">Permissions</span></span>
<span data-ttu-id="09cad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09cad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="09cad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09cad-108">Permission type</span></span>      | <span data-ttu-id="09cad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09cad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09cad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09cad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09cad-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09cad-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09cad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09cad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09cad-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09cad-113">Not supported.</span></span>    |
|<span data-ttu-id="09cad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09cad-114">Application</span></span> | <span data-ttu-id="09cad-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09cad-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09cad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09cad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="09cad-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09cad-117">Request headers</span></span>
| <span data-ttu-id="09cad-118">Nome</span><span class="sxs-lookup"><span data-stu-id="09cad-118">Name</span></span>       | <span data-ttu-id="09cad-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="09cad-119">Type</span></span> | <span data-ttu-id="09cad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="09cad-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09cad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="09cad-121">Authorization</span></span>  | <span data-ttu-id="09cad-122">string</span><span class="sxs-lookup"><span data-stu-id="09cad-122">string</span></span>  | <span data-ttu-id="09cad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09cad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09cad-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="09cad-125">Content-type</span></span> | <span data-ttu-id="09cad-126">string</span><span class="sxs-lookup"><span data-stu-id="09cad-126">string</span></span> | <span data-ttu-id="09cad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="09cad-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09cad-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09cad-128">Request body</span></span>
<span data-ttu-id="09cad-129">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="09cad-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="09cad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="09cad-130">Response</span></span>

<span data-ttu-id="09cad-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09cad-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09cad-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09cad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09cad-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09cad-133">Request</span></span>
<span data-ttu-id="09cad-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09cad-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="09cad-135">No corpo da solicitação, forneça uma representação JSON do objeto [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="09cad-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="09cad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="09cad-136">Response</span></span>
<span data-ttu-id="09cad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09cad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
