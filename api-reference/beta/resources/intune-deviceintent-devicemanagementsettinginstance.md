---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9aef844dd4957b75b51f8d16014c2253b0253cc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523606"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>tipo de recurso deviceManagementSettingInstance

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo base para uma instância de configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementSettingInstances](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .|
|[Obter deviceManagementSettingInstance](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID de instância da configuração|
|DefinitionId|Cadeia de Caracteres|A ID da definição de configuração dessa instância|
|valueJson|Cadeia de Caracteres|Representação JSON do valor|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```







