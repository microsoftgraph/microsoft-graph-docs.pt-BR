---
title: Listar os dispositivos do usuário
description: Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto. Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para enviar um comando ao dispositivo.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bf6dff6b3eea14455bb9dc1e8eed2f515847efc5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016937"
---
# <a name="list-user-devices"></a><span data-ttu-id="f575a-105">Listar os dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="f575a-105">List user devices</span></span>

<span data-ttu-id="f575a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f575a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f575a-107">Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto.</span><span class="sxs-lookup"><span data-stu-id="f575a-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="f575a-108">Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f575a-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="f575a-109">Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para [enviar um comando](send-device-command.md) ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f575a-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="f575a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f575a-110">Permissions</span></span>

<span data-ttu-id="f575a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f575a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f575a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f575a-113">Permission type</span></span>      | <span data-ttu-id="f575a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f575a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f575a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f575a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f575a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f575a-116">Not supported.</span></span>    |
|<span data-ttu-id="f575a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f575a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f575a-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="f575a-118">Device.Read</span></span>    |
|<span data-ttu-id="f575a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f575a-119">Application</span></span> | <span data-ttu-id="f575a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f575a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f575a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f575a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="f575a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f575a-122">Request headers</span></span>

| <span data-ttu-id="f575a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f575a-123">Header</span></span> |<span data-ttu-id="f575a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f575a-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="f575a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f575a-125">Authorization</span></span>| <span data-ttu-id="f575a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f575a-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f575a-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f575a-128">Accept</span></span> | <span data-ttu-id="f575a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f575a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f575a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f575a-130">Request body</span></span>
<span data-ttu-id="f575a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f575a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f575a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f575a-132">Response</span></span>

<span data-ttu-id="f575a-133">Se tiver êxito, este método retornará um código de resposta 200 e as propriedades do dispositivo do usuário no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f575a-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a><span data-ttu-id="f575a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f575a-134">Example</span></span>
<span data-ttu-id="f575a-135">Este exemplo retornará a lista de dispositivos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f575a-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="f575a-136">Para executar um comando em um dispositivo usando `me/devices/{id}/command` o, você precisará obter a ID do dispositivo que é retornado.</span><span class="sxs-lookup"><span data-stu-id="f575a-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="f575a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f575a-137">Request</span></span>

<span data-ttu-id="f575a-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f575a-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f575a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f575a-139">Response</span></span>

<span data-ttu-id="f575a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f575a-140">The following is an example of the response.</span></span> <span data-ttu-id="f575a-141">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f575a-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f575a-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f575a-142">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```


