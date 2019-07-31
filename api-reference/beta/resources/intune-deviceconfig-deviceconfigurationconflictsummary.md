---
title: tipo de recurso Propriedadesdeviceconfigurationconflictsummary
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f4beeafbf6dd52cc29791bfde917e363c7077e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001653"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>tipo de recurso Propriedadesdeviceconfigurationconflictsummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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





