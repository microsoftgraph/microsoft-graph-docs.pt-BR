---
title: tipo de recurso targetedManagedAppConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para a configuração de aplicativo gerenciado direcionada PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5bb8de4505a9f6b7396814a0c51946f60bfe3f38
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051136"
---
# <a name="targetedmanagedappconfigurationpolicysetitem-resource-type"></a>tipo de recurso targetedManagedAppConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a configuração de aplicativo gerenciado direcionada PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar targetedManagedAppConfigurationPolicySetItems](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-list.md)|[coleção targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Listar propriedades e relações dos objetos [targetedManagedAppConfigurationPolicySetItem.](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|
|[Obter targetedManagedAppConfigurationPolicySetItem](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-get.md)|[targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Leia propriedades e relações do [objeto targetedManagedAppConfigurationPolicySetItem.](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|
|[Criar targetedManagedAppConfigurationPolicySetItem](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-create.md)|[targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Crie um novo [objeto targetedManagedAppConfigurationPolicySetItem.](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|
|[Excluir targetedManagedAppConfigurationPolicySetItem](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-delete.md)|Nenhum|Exclui um [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md).|
|[Atualizar targetedManagedAppConfigurationPolicySetItem](../api/intune-policyset-targetedmanagedappconfigurationpolicysetitem-update.md)|[targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|Atualize as propriedades de [um objeto targetedManagedAppConfigurationPolicySetItem.](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)|

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

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
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



