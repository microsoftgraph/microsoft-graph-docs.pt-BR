---
title: tipo de recurso de deviceConfigurationConflictSummary
description: Resumo de um conjunto de políticas de configuração de dispositivo de conflito.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6f366a36b2b24eafee8e3685821688f2ac85a2bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948653"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>tipo de recurso de deviceConfigurationConflictSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Resumo de um conjunto de políticas de configuração de dispositivo de conflito.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista deviceConfigurationConflictSummaries](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|coleção [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Lista as propriedades e os relacionamentos dos objetos [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Obter deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Leia as propriedades e os relacionamentos do objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Criar deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Crie um novo objeto de [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Excluir deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Nenhum|Exclui um [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[Atualizar deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Atualize as propriedades de um objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conflictingDeviceConfigurations|Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)|O conjunto de diretivas em conflito com a configuração de determinado|
|id|String|A identificação para este conjunto de diretivas conflitantes. Este id é as identificações de todas as políticas do ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.|
|contributingSettings|String collection|O conjunto de configurações em conflito com as políticas de determinado|
|deviceCheckinsImpacted|Int32|A contagem de check-ins afetados pelas configurações e diretivas conflitantes|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```





