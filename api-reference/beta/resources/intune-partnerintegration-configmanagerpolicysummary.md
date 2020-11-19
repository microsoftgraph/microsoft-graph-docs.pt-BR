---
title: tipo de recurso configManagerPolicySummary
description: Um resumo da política de Configmanager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c63e85448b70abc76f4df0021c4f5516e778ebe0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301410"
---
# <a name="configmanagerpolicysummary-resource-type"></a>tipo de recurso configManagerPolicySummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um resumo da política de Configmanager.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|targetedDeviceCount|Int32|O número de dispositivos direcionados pela política.|
|compliantDeviceCount|Int32|O número de dispositivos avaliados para serem compatíveis com a política.|
|nonCompliantDeviceCount|Int32|O número de dispositivos avaliados não são compatíveis com a política.|
|failedDeviceCount|Int32|O número de dispositivos que não puderam ser avaliados pela política.|
|pendingDeviceCount|Int32|O número de dispositivos que confirmaram a política, mas têm avaliação pendente.|
|enforcedDeviceCount|Int32|O número de dispositivos que foram corrigidos pela política.|

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




