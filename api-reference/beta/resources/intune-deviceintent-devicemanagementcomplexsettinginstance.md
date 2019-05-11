---
title: tipo de recurso deviceManagementComplexSettingInstance
description: Uma instância de configuração representando um valor complexo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b91753befa679fe003d9d271e07cd210ee3757f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943519"
---
# <a name="devicemanagementcomplexsettinginstance-resource-type"></a>tipo de recurso deviceManagementComplexSettingInstance

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instância de configuração representando um valor complexo


Herda de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementComplexSettingInstances](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-list.md)|coleção [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Listar Propriedades e relações dos objetos [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .|
|[Obter deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-get.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Leia as propriedades e as relações do objeto [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .|
|[Criar deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-create.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Criar um novo objeto [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .|
|[Excluir deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-delete.md)|Nenhum|Exclui [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).|
|[Atualizar deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-update.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Atualiza as propriedades de um objeto [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|DefinitionId|Cadeia de caracteres|A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|Cadeia de caracteres|Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|valor|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Os valores que compõem a configuração complexa|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplexSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```




