---
title: 'call: logTeleconferenceDeviceQuality'
description: Registre dados de qualidade do dispositivo de videoconferência.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a6cbacb3ce97ca1b9b09b12e0185757d5c8392ac
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786044"
---
# <a name="call-logteleconferencedevicequality"></a><span data-ttu-id="1d691-103">call: logTeleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="1d691-103">call: logTeleconferenceDeviceQuality</span></span>

<span data-ttu-id="1d691-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d691-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d691-105">Registre dados de qualidade do dispositivo de videoconferência.</span><span class="sxs-lookup"><span data-stu-id="1d691-105">Log video teleconferencing device quality data.</span></span>

<span data-ttu-id="1d691-106">O bot do Cloud Video Interop (CVI) representa dispositivos VTC (video teleconferência) e age como um agente back-to-back para um dispositivo VTC em uma chamada de conferência.</span><span class="sxs-lookup"><span data-stu-id="1d691-106">The Cloud Video Interop (CVI) bot represents video teleconferencing (VTC) devices and acts as a back-to-back agent for a VTC device in a conference call.</span></span> <span data-ttu-id="1d691-107">Como um bot CVI está no meio da infraestrutura do VTC e Microsoft Teams como um proxy VTC, ele tem duas patas de mídia.</span><span class="sxs-lookup"><span data-stu-id="1d691-107">Because a CVI bot is in the middle of the VTC and Microsoft Teams infrastructure as a VTC proxy, it has two media legs.</span></span> <span data-ttu-id="1d691-108">Uma etapa de mídia está entre o bot CVI e Teams infraestrutura, como um servidor de conferência Teams ou um cliente Teams.</span><span class="sxs-lookup"><span data-stu-id="1d691-108">One media leg is between the CVI bot and Teams infrastructure, such as Teams conference server or a Teams client.</span></span> <span data-ttu-id="1d691-109">A outra etapa de mídia está entre o bot CVI e o dispositivo VTC.</span><span class="sxs-lookup"><span data-stu-id="1d691-109">The other media leg is between the CVI bot and the VTC device.</span></span> 

<span data-ttu-id="1d691-110">Os parceiros de terceiros são os donos do trecho de mídia VTC e a infraestrutura Teams não podem acessar os dados de qualidade do trecho de chamada de terceiros.</span><span class="sxs-lookup"><span data-stu-id="1d691-110">The third-party partners own the VTC media leg and the Teams infrastructure cannot access the quality data of the third-party call leg.</span></span>  <span data-ttu-id="1d691-111">Esse método é destinado apenas aos parceiros CVI para fornecer seus dados de qualidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="1d691-111">This method is only for the CVI partners to provide their media quality data.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d691-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d691-112">Permissions</span></span>

<span data-ttu-id="1d691-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d691-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d691-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d691-115">Permission type</span></span>                        | <span data-ttu-id="1d691-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d691-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1d691-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d691-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d691-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d691-118">Not supported.</span></span> |
| <span data-ttu-id="1d691-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d691-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d691-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d691-120">Not supported.</span></span> |
| <span data-ttu-id="1d691-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d691-121">Application</span></span>                            | <span data-ttu-id="1d691-122">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="1d691-122">Calls.AccessMedia.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d691-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d691-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/logTeleconferenceDeviceQuality
```

## <a name="request-headers"></a><span data-ttu-id="1d691-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d691-124">Request headers</span></span>

| <span data-ttu-id="1d691-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1d691-125">Name</span></span>          | <span data-ttu-id="1d691-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d691-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1d691-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d691-127">Authorization</span></span> | <span data-ttu-id="1d691-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d691-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d691-130">User-Agent</span><span class="sxs-lookup"><span data-stu-id="1d691-130">User-Agent</span></span>    | <span data-ttu-id="1d691-131">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="1d691-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="1d691-132">Os detalhes aparecerão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="1d691-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="1d691-133">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="1d691-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="1d691-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d691-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d691-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d691-135">Request body</span></span>

<span data-ttu-id="1d691-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d691-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d691-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1d691-137">Parameter</span></span>    | <span data-ttu-id="1d691-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d691-138">Type</span></span>        | <span data-ttu-id="1d691-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d691-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d691-140">quality</span><span class="sxs-lookup"><span data-stu-id="1d691-140">quality</span></span>|[<span data-ttu-id="1d691-141">teleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="1d691-141">teleconferenceDeviceQuality</span></span>](../resources/teleconferencedevicequality.md)|<span data-ttu-id="1d691-142">Dados de qualidade da etapa de mídia VTC.</span><span class="sxs-lookup"><span data-stu-id="1d691-142">Quality data of VTC media leg.</span></span>|

## <a name="response"></a><span data-ttu-id="1d691-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d691-143">Response</span></span>

<span data-ttu-id="1d691-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d691-p106">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d691-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d691-146">Examples</span></span>

<span data-ttu-id="1d691-147">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1d691-147">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1d691-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d691-148">Request</span></span>

<span data-ttu-id="1d691-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d691-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d691-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d691-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call_logteleconferencedevicequality"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/logTeleconferenceDeviceQuality
Content-type: application/json

{
  "quality": {
    "@odata.type": "#microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "0622673d-9f69-49b3-9d4f-5ec64f42ecce",
    "participantId": "ea078406-b5d4-4d3c-b85e-90103dcec7f6",
    "mediaLegId": "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f",
    "deviceName": "TestAgent",
    "deviceDescription": "TestDescription",
    "mediaQualityList": [
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceAudioQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      },
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceVideoQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      },
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1d691-151">C#</span><span class="sxs-lookup"><span data-stu-id="1d691-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-logteleconferencedevicequality-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d691-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d691-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-logteleconferencedevicequality-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d691-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d691-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-logteleconferencedevicequality-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d691-154">Java</span><span class="sxs-lookup"><span data-stu-id="1d691-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-logteleconferencedevicequality-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d691-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d691-155">Response</span></span>

<span data-ttu-id="1d691-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d691-156">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: logTeleconferenceDeviceQuality",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

