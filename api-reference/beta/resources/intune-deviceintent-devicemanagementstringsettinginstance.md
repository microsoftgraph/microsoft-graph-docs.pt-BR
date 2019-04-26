---
title: tipo de recurso deviceManagementStringSettingInstance
description: Uma instância de configuração que representa um valor de cadeia de caracteres
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3297085a905934792de2d371f295b467ad9a8e44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562269"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a>tipo de recurso deviceManagementStringSettingInstance

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instância de configuração que representa um valor de cadeia de caracteres


Herda de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementStringSettingInstances](../api/intune-deviceintent-devicemanagementstringsettinginstance-list.md)|coleção [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Listar Propriedades e relações dos objetos [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|
|[Obter deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-get.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Leia as propriedades e as relações do objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|
|[Criar deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-create.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Criar um novo objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|
|[Excluir deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-delete.md)|Nenhum|Exclui [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).|
|[Atualizar deviceManagementStringSettingInstance](../api/intune-deviceintent-devicemanagementstringsettinginstance-update.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Atualiza as propriedades de um objeto [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da instância de configuração herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|DefinitionId|String|A ID da definição de configuração dessa instância herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|Representação JSON do valor herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Cadeia de caracteres|O valor da cadeia de caracteres|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementStringSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": "String"
}
```





