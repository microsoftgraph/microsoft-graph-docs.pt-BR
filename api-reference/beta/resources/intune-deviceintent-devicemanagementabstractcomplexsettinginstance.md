---
title: Tipo de recurso deviceManagementAbstractComplexSettingInstance
description: Uma instância de configuração que representa um valor complexo para uma configuração abstrata
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64e869f4cbb369a5446d255f4659fb4a3a620130
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797518"
---
# <a name="devicemanagementabstractcomplexsettinginstance-resource-type"></a>Tipo de recurso deviceManagementAbstractComplexSettingInstance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instância de configuração que representa um valor complexo para uma configuração abstrata


Herda [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementAbstractComplexSettingInstances](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-list.md)|[Coleção deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Listar propriedades e relações dos [objetos deviceManagementAbstractComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|
|[Obter deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-get.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Leia propriedades e relações do [objeto deviceManagementAbstractComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|
|[Criar deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-create.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Crie um novo [objeto deviceManagementAbstractComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|
|[Excluir deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-delete.md)|Nenhum(a)|Exclui um [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).|
|[Atualizar deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-update.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Atualize as propriedades de [um objeto deviceManagementAbstractComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|Cadeia de caracteres|A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|Cadeia de caracteres|Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|implementationId|Cadeia de caracteres|A ID de definição para a implementação escolhida dessa configuração complexa|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|valor|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Os valores que comem a configuração complexa|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "implementationId": "String"
}
```



