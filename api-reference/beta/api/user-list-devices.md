---
title: Listar os dispositivos do usuário
description: Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto. Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para enviar um comando ao dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc8fedf14d2b61bb407bd5a4eec99ad83c4f1f71
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334841"
---
# <a name="list-user-devices"></a><span data-ttu-id="b536e-105">Listar os dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="b536e-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b536e-106">Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto.</span><span class="sxs-lookup"><span data-stu-id="b536e-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="b536e-107">Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b536e-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="b536e-108">Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para [enviar um comando](send-device-command.md) ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b536e-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="b536e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b536e-109">Permissions</span></span>

<span data-ttu-id="b536e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b536e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b536e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b536e-112">Permission type</span></span>      | <span data-ttu-id="b536e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b536e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b536e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b536e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b536e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b536e-115">Not supported.</span></span>    |
|<span data-ttu-id="b536e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b536e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b536e-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="b536e-117">Device.Read</span></span>    |
|<span data-ttu-id="b536e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b536e-118">Application</span></span> | <span data-ttu-id="b536e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b536e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b536e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b536e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="b536e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b536e-121">Request headers</span></span>

| <span data-ttu-id="b536e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b536e-122">Header</span></span> |<span data-ttu-id="b536e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b536e-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="b536e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b536e-124">Authorization</span></span>| <span data-ttu-id="b536e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b536e-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b536e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b536e-127">Accept</span></span> | <span data-ttu-id="b536e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b536e-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b536e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b536e-129">Request body</span></span>
<span data-ttu-id="b536e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b536e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b536e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b536e-131">Response</span></span>

<span data-ttu-id="b536e-132">Se tiver êxito, este método retornará um código de resposta 200 e as propriedades do dispositivo do usuário no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b536e-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="b536e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b536e-133">Example</span></span>
<span data-ttu-id="b536e-134">Este exemplo retornará a lista de dispositivos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b536e-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="b536e-135">Para executar um comando em `me/devices/{id}/command`um dispositivo usando o, você precisará obter a ID do dispositivo que é retornado.</span><span class="sxs-lookup"><span data-stu-id="b536e-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="b536e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b536e-136">Request</span></span>

<span data-ttu-id="b536e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b536e-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="b536e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b536e-138">Response</span></span>

<span data-ttu-id="b536e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b536e-139">The following is an example of the response.</span></span> <span data-ttu-id="b536e-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b536e-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b536e-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b536e-141">All of the properties will be returned from an actual call.</span></span>

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
