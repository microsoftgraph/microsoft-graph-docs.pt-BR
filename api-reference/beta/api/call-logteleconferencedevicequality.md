---
title: 'Call: logTeleconferenceDeviceQuality'
description: Registre dados de qualidade do dispositivo de videoconferência.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 141efaf0f08c91b12517c2e378df00ccd3803d12
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123269"
---
# <a name="call-logteleconferencedevicequality"></a><span data-ttu-id="bb523-103">Call: logTeleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="bb523-103">call: logTeleconferenceDeviceQuality</span></span>

<span data-ttu-id="bb523-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb523-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb523-105">Registre dados de qualidade do dispositivo de videoconferência.</span><span class="sxs-lookup"><span data-stu-id="bb523-105">Log video teleconferencing device quality data.</span></span>

<span data-ttu-id="bb523-106">O bot de interoperabilidade de vídeo de nuvem (CVI) representa dispositivos de teleconferência de vídeo (VTC) e atua como um agente back-to-back para um dispositivo VTC em uma chamada em conferência.</span><span class="sxs-lookup"><span data-stu-id="bb523-106">The Cloud Video Interop (CVI) bot represents video teleconferencing (VTC) devices and acts as a back-to-back agent for a VTC device in a conference call.</span></span> <span data-ttu-id="bb523-107">Como um bot do CVI está no meio do VTC e da infraestrutura do Microsoft Teams como um proxy do VTC, ele tem dois trechos de mídia.</span><span class="sxs-lookup"><span data-stu-id="bb523-107">Because a CVI bot is in the middle of the VTC and Microsoft Teams infrastructure as a VTC proxy, it has two media legs.</span></span> <span data-ttu-id="bb523-108">Um trecho de mídia está entre a infraestrutura de bot e de equipes do CVI, como o servidor de conferência do teams ou um cliente do teams.</span><span class="sxs-lookup"><span data-stu-id="bb523-108">One media leg is between the CVI bot and Teams infrastructure, such as Teams conference server or a Teams client.</span></span> <span data-ttu-id="bb523-109">O outro trecho de mídia está entre o bot CVI e o dispositivo VTC.</span><span class="sxs-lookup"><span data-stu-id="bb523-109">The other media leg is between the CVI bot and the VTC device.</span></span> 

<span data-ttu-id="bb523-110">Os parceiros de terceiros possuem o trecho de mídia do VTC e a infraestrutura de equipe não pode acessar os dados de qualidade do trecho de chamada de terceiros.</span><span class="sxs-lookup"><span data-stu-id="bb523-110">The third-party partners own the VTC media leg and the Teams infrastructure cannot access the quality data of the third-party call leg.</span></span>  <span data-ttu-id="bb523-111">Este método é somente para os parceiros do CVI fornecerem seus dados de qualidade de mídia.</span><span class="sxs-lookup"><span data-stu-id="bb523-111">This method is only for the CVI partners to provide their media quality data.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb523-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb523-112">Permissions</span></span>

<span data-ttu-id="bb523-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb523-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb523-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb523-115">Permission type</span></span>                        | <span data-ttu-id="bb523-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb523-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb523-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb523-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb523-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb523-118">Not supported.</span></span> |
| <span data-ttu-id="bb523-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb523-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb523-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb523-120">Not supported.</span></span> |
| <span data-ttu-id="bb523-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb523-121">Application</span></span>                            | <span data-ttu-id="bb523-122">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="bb523-122">Calls.AccessMedia.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb523-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb523-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/logTeleconferenceDeviceQuality
```

## <a name="request-headers"></a><span data-ttu-id="bb523-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb523-124">Request headers</span></span>

| <span data-ttu-id="bb523-125">Nome</span><span class="sxs-lookup"><span data-stu-id="bb523-125">Name</span></span>          | <span data-ttu-id="bb523-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb523-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb523-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb523-127">Authorization</span></span> | <span data-ttu-id="bb523-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb523-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb523-130">Agente de usuário</span><span class="sxs-lookup"><span data-stu-id="bb523-130">User-Agent</span></span>    | <span data-ttu-id="bb523-131">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="bb523-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="bb523-132">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="bb523-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="bb523-133">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="bb523-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="bb523-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb523-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb523-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb523-135">Request body</span></span>

<span data-ttu-id="bb523-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb523-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bb523-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bb523-137">Parameter</span></span>    | <span data-ttu-id="bb523-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb523-138">Type</span></span>        | <span data-ttu-id="bb523-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb523-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb523-140">qualidade</span><span class="sxs-lookup"><span data-stu-id="bb523-140">quality</span></span>|[<span data-ttu-id="bb523-141">teleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="bb523-141">teleconferenceDeviceQuality</span></span>](../resources/teleconferencedevicequality.md)|<span data-ttu-id="bb523-142">Dados de qualidade do trecho de mídia do VTC.</span><span class="sxs-lookup"><span data-stu-id="bb523-142">Quality data of VTC media leg.</span></span>|

## <a name="response"></a><span data-ttu-id="bb523-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb523-143">Response</span></span>

<span data-ttu-id="bb523-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb523-p106">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb523-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb523-146">Examples</span></span>

<span data-ttu-id="bb523-147">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bb523-147">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bb523-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb523-148">Request</span></span>

<span data-ttu-id="bb523-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb523-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb523-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb523-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call_logteleconferencedevicequality"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/logTeleconferenceDeviceQuality
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
# <a name="c"></a>[<span data-ttu-id="bb523-151">C#</span><span class="sxs-lookup"><span data-stu-id="bb523-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-logteleconferencedevicequality-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb523-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb523-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-logteleconferencedevicequality-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb523-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb523-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-logteleconferencedevicequality-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb523-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb523-154">Response</span></span>

<span data-ttu-id="bb523-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb523-155">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
