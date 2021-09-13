---
title: Tipo de recurso deviceManagementComplexSettingInstance
description: Uma instância de configuração que representa um valor complexo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0789c0720ff773666c992c86fb389c4ea010e5b4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137998"
---
# <a name="devicemanagementcomplexsettinginstance-resource-type"></a>Tipo de recurso deviceManagementComplexSettingInstance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instância de configuração que representa um valor complexo


Herda [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementComplexSettingInstances](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-list.md)|[Coleção deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Listar propriedades e relações dos [objetos deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|
|[Obter deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-get.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Leia propriedades e relações do [objeto deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|
|[Criar deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-create.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Crie um novo [objeto deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|
|[Excluir deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-delete.md)|Nenhum|Exclui um [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).|
|[Atualizar deviceManagementComplexSettingInstance](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-update.md)|[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|Atualize as propriedades de [um objeto deviceManagementComplexSettingInstance.](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da instância de configuração Herdada [de deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|Cadeia de Caracteres|A ID da definição de configuração para esta instância Herdada de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|Cadeia de Caracteres|Representação JSON do valor Herdado de [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|valor|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Os valores que comem a configuração complexa|

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



