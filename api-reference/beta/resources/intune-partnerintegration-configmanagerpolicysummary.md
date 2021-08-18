---
title: Tipo de recurso configManagerPolicySummary
description: Um resumo de política ConfigManager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c14e64fb528d5b62ce172d6dc4e85704422ea1f5a74ef0f012b8e0d48b6f6cb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224478"
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




