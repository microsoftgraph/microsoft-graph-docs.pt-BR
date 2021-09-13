---
title: Tipo de recurso teleconferenceDeviceQuality
description: Representa dados de qualidade de nível de sessão de dispositivo de teleconferência de vídeo.
ms.localizationpriority: medium
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6e7b29330634b099974300c660b45923b31b9b66
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128085"
---
# <a name="teleconferencedevicequality-resource-type"></a>Tipo de recurso teleconferenceDeviceQuality

Namespace: microsoft.graph

Representa dados de qualidade de nível de sessão de dispositivo de teleconferência de vídeo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|callChainId|Guid|Um identificador exclusivo para todas as chamadas do participante em uma conferência ou um identificador exclusivo para duas chamadas de participantes em chamada P2P. Isso precisa ser copiado de `Microsoft.Graph.Call.CallChainId`.|
|cloudServiceDeploymentEnvironment|Cadeia de caracteres|Uma região geográfica onde o serviço é implantado, como `ProdNoam` .|
|cloudServiceDeploymentId|Cadeia de caracteres|Um identificador de implantação exclusivo atribuído pelo Azure.|
|cloudServiceInstanceName|Cadeia de caracteres|O nome da instância do serviço de nuvem implantado pelo Azure, como `FrontEnd_IN_3` .|
|cloudServiceName|Cadeia de caracteres|O nome do serviço de nuvem implantado pelo Azure, como `contoso.cloudapp.net` .|
|deviceDescription|String|Qualquer descrição adicional, como `VTC Bldg 30/21` .|
|deviceName|String|O nome do agente de mídia do usuário, como `Cisco SX80` .|
|mediaLegId|Guid|Um identificador exclusivo para uma etapa de mídia específica de um participante em uma conferência.  Um participante pode ter vários identificadores de leg de mídia se a retargeting acontecer. O parceiro CVI atribui esse valor.|
|mediaQualityList|[Coleção teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)|A lista de qualidades de mídia em uma sessão de mídia (chamada), como qualidade de áudio, qualidade de vídeo e/ou qualidade de compartilhamento de tela.|
|participantId|Guid|Um identificador exclusivo para um participante específico em uma conferência. O parceiro CVI precisa copiar `Call.MyParticipantId` para essa propriedade.|

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

