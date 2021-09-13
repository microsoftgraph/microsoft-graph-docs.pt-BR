---
title: Tipo de recurso configManagerPolicySummary
description: Um resumo de política ConfigManager.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88c31f9314f7cc4c55c68b328768e3119d913298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033452"
---
# <a name="configmanagerpolicysummary-resource-type"></a>Tipo de recurso configManagerPolicySummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um resumo de política ConfigManager.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|targetedDeviceCount|Int32|O número de dispositivos direcionados pela política.|
|compliantDeviceCount|Int32|O número de dispositivos avaliados para serem compatíveis com a política.|
|nonCompliantDeviceCount|Int32|O número de dispositivos avaliados como não compatíveis com a política.|
|failedDeviceCount|Int32|O número de dispositivos que não foram avaliados pela política.|
|pendingDeviceCount|Int32|O número de dispositivos que reconheceram a política, mas estão pendentes de avaliação.|
|enforcedDeviceCount|Int32|O número de dispositivos que foram remediados pela política.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configManagerPolicySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerPolicySummary",
  "targetedDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "enforcedDeviceCount": 1024
}
```



