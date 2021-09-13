---
title: Tipo de recurso managedDeviceMobileAppConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para a configuração de aplicativo móvel de dispositivo gerenciado PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fcf8ee11a0fe3c2a6f58ec0f3fb6ffc7aa565968
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080727"
---
# <a name="manageddevicemobileappconfigurationpolicysetitem-resource-type"></a>Tipo de recurso managedDeviceMobileAppConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a configuração de aplicativo móvel de dispositivo gerenciado PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationPolicySetItems](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-list.md)|[coleção managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Listar propriedades e relações dos [objetos managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|
|[Obter managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-get.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Leia propriedades e relações do [objeto managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|
|[Criar managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-create.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Crie um novo [objeto managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|
|[Excluir managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-delete.md)|Nenhum|Exclui [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md).|
|[Atualizar managedDeviceMobileAppConfigurationPolicySetItem](../api/intune-policyset-manageddevicemobileappconfigurationpolicysetitem-update.md)|[managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|Atualize as propriedades de [um objeto managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)|

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



