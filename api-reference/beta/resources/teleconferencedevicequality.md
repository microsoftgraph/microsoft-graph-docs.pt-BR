---
title: tipo de recurso teleconferenceDeviceQuality
description: Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 577a68cfe2d765b8d6731748687d11f9e26ee3d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046304"
---
# <a name="teleconferencedevicequality-resource-type"></a>tipo de recurso teleconferenceDeviceQuality

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|callChainId|Guid|Um identificador exclusivo para todas as chamadas de participantes em uma conferência ou um identificador exclusivo para duas chamadas de participantes na chamada P2P. Isso precisa ser copiado de `Microsoft.Graph.Call.CallChainId`.|
|cloudServiceDeploymentEnvironment|Cadeia de caracteres|Uma região geográfica onde o serviço é implantado, como `ProdNoam` .|
|cloudServiceDeploymentId|Cadeia de caracteres|Um identificador de implantação exclusivo atribuído pelo Azure.|
|cloudServiceInstanceName|Cadeia de caracteres|O nome da instância do serviço de nuvem implantada do Azure, como `FrontEnd_IN_3` .|
|cloudServiceName|Cadeia de caracteres|O nome do serviço de nuvem implantada do Azure, como `contoso.cloudapp.net` .|
|deviceDescription|Cadeia de caracteres|Qualquer descrição adicional, como `VTC Bldg 30/21` .|
|deviceName|String|O nome do agente de mídia do usuário, como `Cisco SX80` .|
|mediaLegId|Guid|Um identificador exclusivo para um trecho de mídia específico de um participante de uma conferência.  Um participante pode ter vários identificadores de trechos de mídia se o redirecionamento ocorrer. O parceiro CVI atribui esse valor.|
|mediaQualityList|coleção [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)|A lista de qualidades de mídia em uma sessão de mídia (chamada), como qualidade de áudio, qualidade de vídeo e/ou qualidade de compartilhamento de tela.|
|participante de participantes|Guid|Um identificador exclusivo para um participante específico em uma conferência. O parceiro CVI precisa copiar `Call.MyParticipantId` para esta propriedade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
  "baseType": null
}-->

```json
{
  "callChainId": "Guid",
  "cloudServiceDeploymentEnvironment": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceName": "String",
  "deviceDescription": "String",
  "deviceName": "String",
  "mediaLegId": "Guid",
  "mediaQualityList": [{"@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"}],
  "participantId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


