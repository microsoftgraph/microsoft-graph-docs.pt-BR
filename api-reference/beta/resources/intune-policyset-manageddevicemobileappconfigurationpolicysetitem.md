---
title: tipo de recurso managedDeviceMobileAppConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para a configuração do aplicativo móvel do dispositivo PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3910cb9017e353de4cdbf3792779b0230c96d67d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288086"
---
# <a name="manageddevicemobileappconfigurationpolicysetitem-resource-type"></a>tipo de recurso managedDeviceMobileAppConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a configuração do aplicativo móvel do dispositivo PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationPolicySetItems](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-list.md)|coleção [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Listar Propriedades e relações dos objetos [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .|
|[Obter managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-get.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .|
|[Criar managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-create.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Criar um novo objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .|
|[Excluir managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-delete.md)|Nenhum|Exclui [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md).|
|[Atualizar managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-update.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Atualiza as propriedades de um objeto [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do MobileAppPolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|String|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro, caso algum tenha ocorrido. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Coleção de cadeias de caracteres|Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
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




