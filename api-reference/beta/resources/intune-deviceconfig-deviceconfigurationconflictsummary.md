---
title: tipo de recurso Propriedadesdeviceconfigurationconflictsummary
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3add7a02064035e363f5d2d4886edc93cbd0d37a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705988"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>tipo de recurso Propriedadesdeviceconfigurationconflictsummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo de conflito para um conjunto de políticas de configuração de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurationConflictSummaries](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|coleção [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Listar Propriedades e relações dos objetos [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Obter Propriedadesdeviceconfigurationconflictsummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Leia as propriedades e as relações do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Criar Propriedadesdeviceconfigurationconflictsummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Criar um novo objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Excluir Propriedadesdeviceconfigurationconflictsummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Nenhum|Exclui [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[Atualizar Propriedadesdeviceconfigurationconflictsummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Atualiza as propriedades de um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conflictingDeviceConfigurations|Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)|O conjunto de políticas em conflito com a configuração determinada|
|id|String|A ID desse conjunto de diretivas conflitantes. Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.|
|contributingSettings|Coleção de cadeias de caracteres|O conjunto de configurações em conflito com as políticas determinadas|
|deviceCheckinsImpacted|Int32|A contagem de check-ins impactados pelas políticas e configurações conflitantes|

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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```





