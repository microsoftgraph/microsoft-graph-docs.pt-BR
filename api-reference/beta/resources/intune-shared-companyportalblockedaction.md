---
title: Tipo de recurso companyPortalBlockedAction
description: Ações bloqueadas no portal da empresa de acordo com tipos de propriedade de plataforma e dispositivo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8b04ce4697d2ff24f28644908cf12764f8bd3d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039193"
---
# <a name="companyportalblockedaction-resource-type"></a>Tipo de recurso companyPortalBlockedAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ações bloqueadas no portal da empresa de acordo com tipos de propriedade de plataforma e dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|plataforma|[devicePlatformType](../resources/intune-wip-deviceplatformtype.md)|Sistema operacional/plataforma do dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Tipo de propriedade do dispositivo. Os valores possíveis são: `unknown`, `company`, `personal`.|
|ação|[companyPortalAction](../resources/intune-shared-companyportalaction.md)|Ação do dispositivo. Os valores possíveis são: `unknown`, `remove`, `reset`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```



