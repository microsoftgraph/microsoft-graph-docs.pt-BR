---
title: Tipo de recurso deviceConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para a configuração do dispositivo PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c7abec05f6ef61218b7d86fb55e30859c2eb5d8f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068603"
---
# <a name="deviceconfigurationpolicysetitem-resource-type"></a>Tipo de recurso deviceConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a configuração do dispositivo PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurationPolicySetItems](../api/intune-policyset-deviceconfigurationpolicysetitem-list.md)|[Coleção deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Listar propriedades e relações dos [objetos deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|
|[Obter deviceConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-get.md)|[deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Ler propriedades e relações do [objeto deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|
|[Criar deviceConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-create.md)|[deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Crie um novo [objeto deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|
|[Excluir deviceConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-delete.md)|Nenhum|Exclui um [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md).|
|[Atualizar deviceConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-update.md)|[deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Atualize as propriedades de [um objeto deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Cadeia de Caracteres|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Conjunto de cadeias de caracteres|Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



