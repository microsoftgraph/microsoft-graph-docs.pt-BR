---
title: Tipo de recurso teamworkCameraConfiguration
description: Representa os detalhes sobre a configuração da câmera para um Salas do Microsoft Teams dispositivo.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f10a0db06b158dda00f4db9e7df0e34e1ab6ac1c
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262263"
---
# <a name="teamworkcameraconfiguration-resource-type"></a>Tipo de recurso teamworkCameraConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração da câmera para um Salas do Microsoft Teams [dispositivo](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentCameraConfiguration|[teamworkContentCameraConfiguration](../resources/teamworkcontentcameraconfiguration.md)|A configuração da câmera de conteúdo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|cameras|[coleção teamworkPeripheral](../resources/teamworkperipheral.md)|A lista de câmeras conectadas.|
|defaultContentCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|A câmera de conteúdo configurada usada para compartilhar conteúdo de quadro de trabalho analógico em uma reunião.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkCameraConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkCameraConfiguration",
  "contentCameraConfiguration": {
    "@odata.type": "microsoft.graph.teamworkContentCameraConfiguration"
  }
}
```

