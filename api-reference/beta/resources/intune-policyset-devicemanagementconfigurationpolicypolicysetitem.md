---
title: Tipo de recurso deviceManagementConfigurationPolicyPolicySetItem
description: Uma classe que contém as propriedades usadas para DeviceManagementConfiguration PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06a49c845003ef52b240e4ef95dc46a245359ebf
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259186"
---
# <a name="devicemanagementconfigurationpolicypolicysetitem-resource-type"></a>Tipo de recurso deviceManagementConfigurationPolicyPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para DeviceManagementConfiguration PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementConfigurationPolicyPolicySetItems](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-list.md)|[Coleção deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|Listar propriedades e relações dos [objetos deviceManagementConfigurationPolicyPolicySetItem.](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|
|[Obter deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-get.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|Leia propriedades e relações do [objeto deviceManagementConfigurationPolicyPolicySetItem.](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|
|[Criar deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-create.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|Crie um novo [objeto deviceManagementConfigurationPolicyPolicySetItem.](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|
|[Excluir deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-delete.md)|Nenhum|Exclui um [deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md).|
|[Atualizar deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-update.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|Atualize as propriedades de [um objeto deviceManagementConfigurationPolicyPolicySetItem.](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Cadeia de caracteres|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|Cadeia de caracteres|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyPolicySetItem",
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




