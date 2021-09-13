---
title: Tipo de recurso iosLobAppProvisioningConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para a configuração de provisionamento de aplicativos lob do iOS PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32f806bf0150bd4a83dc594256d869fa64998b63
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033424"
---
# <a name="ioslobappprovisioningconfigurationpolicysetitem-resource-type"></a>Tipo de recurso iosLobAppProvisioningConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a configuração de provisionamento de aplicativos lob do iOS PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosLobAppProvisioningConfigurationPolicySetItems](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-list.md)|[Coleção iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Listar propriedades e relações dos [objetos iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|
|[Obter iosLobAppProvisioningConfigurationPolicySetItem](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-get.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Leia propriedades e relações do [objeto iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|
|[Criar iosLobAppProvisioningConfigurationPolicySetItem](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-create.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Crie um novo [objeto iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|
|[Excluir iosLobAppProvisioningConfigurationPolicySetItem](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-delete.md)|Nenhum|Exclui um [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).|
|[Atualizar iosLobAppProvisioningConfigurationPolicySetItem](../api/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem-update.md)|[iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|Atualize as propriedades de [um objeto iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)|

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
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
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



