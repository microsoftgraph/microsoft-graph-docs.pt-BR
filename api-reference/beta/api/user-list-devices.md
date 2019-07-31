---
title: Listar os dispositivos do usuário
description: Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto. Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para enviar um comando ao dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 292124babfb71ad1c86ae373f123c2f5d57df3b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996249"
---
# <a name="list-user-devices"></a><span data-ttu-id="10882-105">Listar os dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="10882-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10882-106">Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto.</span><span class="sxs-lookup"><span data-stu-id="10882-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="10882-107">Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10882-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="10882-108">Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para [enviar um comando](send-device-command.md) ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10882-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="10882-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="10882-109">Permissions</span></span>

<span data-ttu-id="10882-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10882-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="10882-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10882-112">Permission type</span></span>      | <span data-ttu-id="10882-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10882-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10882-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10882-114">Delegated (work or school account)</span></span> | <span data-ttu-id="10882-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10882-115">Not supported.</span></span>    |
|<span data-ttu-id="10882-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10882-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10882-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="10882-117">Device.Read</span></span>    |
|<span data-ttu-id="10882-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10882-118">Application</span></span> | <span data-ttu-id="10882-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10882-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10882-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10882-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="10882-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10882-121">Request headers</span></span>

| <span data-ttu-id="10882-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10882-122">Header</span></span> |<span data-ttu-id="10882-123">Valor</span><span class="sxs-lookup"><span data-stu-id="10882-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="10882-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="10882-124">Authorization</span></span>| <span data-ttu-id="10882-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10882-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="10882-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10882-127">Accept</span></span> | <span data-ttu-id="10882-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10882-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="10882-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10882-129">Request body</span></span>
<span data-ttu-id="10882-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10882-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10882-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="10882-131">Response</span></span>

<span data-ttu-id="10882-132">Se tiver êxito, este método retornará um código de resposta 200 e as propriedades do dispositivo do usuário no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10882-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="10882-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10882-133">Example</span></span>
<span data-ttu-id="10882-134">Este exemplo retornará a lista de dispositivos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="10882-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="10882-135">Para executar um comando em `me/devices/{id}/command`um dispositivo usando o, você precisará obter a ID do dispositivo que é retornado.</span><span class="sxs-lookup"><span data-stu-id="10882-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="10882-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10882-136">Request</span></span>

<span data-ttu-id="10882-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10882-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="10882-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="10882-138">Response</span></span>

<span data-ttu-id="10882-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10882-139">The following is an example of the response.</span></span> <span data-ttu-id="10882-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="10882-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="10882-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10882-141">All of the properties will be returned from an actual call.</span></span>

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
