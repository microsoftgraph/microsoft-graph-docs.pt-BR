---
title: tipo de recurso teleconferenceDeviceQuality
description: Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4d76114a35a9ac7d0c9901437b672697c295ebbf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763267"
---
# <a name="teleconferencedevicequality-resource-type"></a>tipo de recurso teleconferenceDeviceQuality

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados de qualidade do nível da sessão do dispositivo de teleconferência de vídeo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|callChainId|Guid|Um identificador exclusivo para todas as chamadas de participantes em uma conferência ou um identificador exclusivo para duas chamadas de participantes na chamada P2P. Isso precisa ser copiado do `Microsoft.Graph.Call.CallChainId`.|
|cloudServiceDeploymentEnvironment|String|Uma região geográfica onde o serviço é implantado, como `ProdNoam`.|
|cloudServiceDeploymentId|String|Um identificador de implantação exclusivo atribuído pelo Azure.|
|cloudServiceInstanceName|String|O nome da instância do serviço de nuvem implantada do Azure, como `FrontEnd_IN_3`.|
|cloudServiceName|String|O nome do serviço de nuvem implantada `contoso.cloudapp.net`do Azure, como.|
|deviceDescription|String|Qualquer descrição adicional, como `VTC Bldg 30/21`.|
|deviceName|String|O nome do agente de mídia do usuário `Cisco SX80`, como.|
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
