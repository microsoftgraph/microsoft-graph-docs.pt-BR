---
title: tipo de recurso configurationManageraction
description: Parâmetro para a ação triggerConfigurationManagerAction
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff71bc6b4094543e3da6d22639014f595a86ce7d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199677"
---
# <a name="configurationmanageraction-resource-type"></a>tipo de recurso configurationManageraction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parâmetro para a ação triggerConfigurationManagerAction

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[configurationManagerActionType](../resources/intune-devices-configurationmanageractiontype.md)|O tipo de ação a ser disparado no cliente do Configuration Manager. Os valores possíveis são: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerAction",
  "action": "String"
}
```



