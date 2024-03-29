---
title: Tipo de recurso managedAppProtectionPolicySetItem
description: Uma classe que contém as propriedades usadas para proteção de aplicativo gerenciado PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0e4c143319f09f8a88744ee27909c6b837beec7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039613"
---
# <a name="managedappprotectionpolicysetitem-resource-type"></a>Tipo de recurso managedAppProtectionPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para proteção de aplicativo gerenciado PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppProtectionPolicySetItems](../api/intune-policyset-managedappprotectionpolicysetitem-list.md)|[Coleção managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Listar propriedades e relações dos [objetos managedAppProtectionPolicySetItem.](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|
|[Obter managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-get.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Leia propriedades e relações do [objeto managedAppProtectionPolicySetItem.](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|
|[Criar managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-create.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Crie um novo [objeto managedAppProtectionPolicySetItem.](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|
|[Excluir managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-delete.md)|Nenhum|Exclui [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).|
|[Atualizar managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-update.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Atualize as propriedades de [um objeto managedAppProtectionPolicySetItem.](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Cadeia de Caracteres|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|Cadeia de Caracteres|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)|
|targetedAppManagementLevels|Cadeia de Caracteres|TargetedAppManagementLevels do ManagedAppPolicySetItem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtectionPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
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
  "targetedAppManagementLevels": "String"
}
```



