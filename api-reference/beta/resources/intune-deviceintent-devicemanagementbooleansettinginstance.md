---
title: Tipo de recurso deviceManagementBooleanSettingInstance
description: Uma instância de configuração que representa um valor booleano
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eed3006e8138070227abd7fd64faa6be46532a8f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784482"
---
# <a name="devicemanagementbooleansettinginstance-resource-type"></a>Tipo de recurso deviceManagementBooleanSettingInstance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instância de configuração que representa um valor booleano


Herda [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementBooleanSettingInstances](../api/intune-deviceintent-devicemanagementbooleansettinginstance-list.md)|[Coleção deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Listar propriedades e relações dos [objetos deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|
|[Obter deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-get.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Leia propriedades e relações do [objeto deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|
|[Criar deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-create.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Crie um novo [objeto deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|
|[Excluir deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-delete.md)|Nenhum(a)|Exclui um [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).|
|[Atualizar deviceManagementBooleanSettingInstance](../api/intune-deviceintent-devicemanagementbooleansettinginstance-update.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|Atualize as propriedades de [um objeto deviceManagementBooleanSettingInstance.](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|Cadeia de caracteres|A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|Cadeia de caracteres|Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Boolean|O valor booleano|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```



