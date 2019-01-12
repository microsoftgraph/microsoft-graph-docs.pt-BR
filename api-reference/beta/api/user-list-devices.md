---
title: Lista de dispositivos de usuário
description: Obtenha uma lista de dispositivos do usuário que oferecem suporte a recursos de projeto Roma. Isso inclui a capacidade de iniciar um aplicativo, ou de mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada GET em mim / dispositivos, passe a ID do dispositivo para enviar um comando para seu dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 04b67b770eec38d9e70a2263cd54212077335c85
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983538"
---
# <a name="list-user-devices"></a><span data-ttu-id="1e3ab-105">Lista de dispositivos de usuário</span><span class="sxs-lookup"><span data-stu-id="1e3ab-105">List user devices</span></span>

> <span data-ttu-id="1e3ab-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e3ab-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e3ab-108">Obtenha uma lista de dispositivos do usuário que oferecem suporte a recursos de projeto Roma.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-108">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="1e3ab-109">Isso inclui a capacidade de iniciar um aplicativo, ou de mensagem ou enviar dados para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-109">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="1e3ab-110">Depois de fazer uma chamada GET em mim / dispositivos, passe a ID do dispositivo para [Enviar um comando](send-device-command.md) para seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-110">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e3ab-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e3ab-111">Permissions</span></span>

<span data-ttu-id="1e3ab-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e3ab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e3ab-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e3ab-114">Permission type</span></span>      | <span data-ttu-id="1e3ab-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e3ab-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e3ab-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e3ab-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1e3ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-117">Not supported.</span></span>    |
|<span data-ttu-id="1e3ab-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e3ab-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e3ab-119">Device.Read</span><span class="sxs-lookup"><span data-stu-id="1e3ab-119">Device.Read</span></span>    |
|<span data-ttu-id="1e3ab-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e3ab-120">Application</span></span> | <span data-ttu-id="1e3ab-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e3ab-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e3ab-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="1e3ab-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3ab-123">Request headers</span></span>

| <span data-ttu-id="1e3ab-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e3ab-124">Header</span></span> |<span data-ttu-id="1e3ab-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1e3ab-125">Value</span></span>
|:----|:------|
|<span data-ttu-id="1e3ab-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e3ab-126">Authorization</span></span>| <span data-ttu-id="1e3ab-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1e3ab-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e3ab-129">Accept</span></span> | <span data-ttu-id="1e3ab-130">application/json</span><span class="sxs-lookup"><span data-stu-id="1e3ab-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e3ab-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3ab-131">Request body</span></span>
<span data-ttu-id="1e3ab-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e3ab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e3ab-133">Response</span></span>

<span data-ttu-id="1e3ab-134">Se tiver êxito, esse método retorna um código de 200 resposta e as propriedades de usuário do dispositivo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-134">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="1e3ab-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e3ab-135">Example</span></span>
<span data-ttu-id="1e3ab-136">Este exemplo retornará a lista de dispositivos para um usuário.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-136">This example will return the list of devices for a user.</span></span> <span data-ttu-id="1e3ab-137">Para um dispositivo usando de comando `me/devices/{id}/command`, você precisará obter a ID do dispositivo que é retornado.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-137">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="1e3ab-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3ab-138">Request</span></span>

<span data-ttu-id="1e3ab-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="1e3ab-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e3ab-140">Response</span></span>

<span data-ttu-id="1e3ab-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-141">The following is an example of the response.</span></span> <span data-ttu-id="1e3ab-142">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1e3ab-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e3ab-143">All of the properties will be returned from an actual call.</span></span>

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
