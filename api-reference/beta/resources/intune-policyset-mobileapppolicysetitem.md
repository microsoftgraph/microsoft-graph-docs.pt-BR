---
title: Tipo de recurso mobileAppPolicySetItem
description: Uma classe que contém as propriedades usadas para o aplicativo móvel PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 985170b659cb8c54f4723d68cd531fa06699e76a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080685"
---
# <a name="mobileapppolicysetitem-resource-type"></a>Tipo de recurso mobileAppPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para o aplicativo móvel PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppPolicySetItems](../api/intune-policyset-mobileapppolicysetitem-list.md)|[Coleção mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Listar propriedades e relações dos [objetos mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Obter mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-get.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Leia propriedades e relações do [objeto mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Criar mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-create.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Crie um novo [objeto mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|
|[Excluir mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-delete.md)|Nenhum|Exclui um [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).|
|[Atualizar mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-update.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Atualize as propriedades de [um objeto mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)|

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
|finalidade|[installIntent](../resources/intune-shared-installintent.md)|Intenção de instalação do MobileAppPolicySetItem. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|configurações|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|Configurações do MobileAppPolicySetItem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
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
  ],
  "intent": "String",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "String",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```



