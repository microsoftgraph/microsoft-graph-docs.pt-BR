---
title: tipo de recurso enrollmentRestrictionsConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para a restrição de registro PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68741546d8b4e83e1076dd82bf45eab03610b221
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272112"
---
# <a name="enrollmentrestrictionsconfigurationpolicysetitem-resource-type"></a>tipo de recurso enrollmentRestrictionsConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a restrição de registro PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enrollmentRestrictionsConfigurationPolicySetItems](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-list.md)|coleção [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Listar Propriedades e relações dos objetos [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Obter enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-get.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Leia as propriedades e as relações do objeto [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Criar enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-create.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Criar um novo objeto [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|
|[Excluir enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-delete.md)|Nenhum|Exclui [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).|
|[Atualizar enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-update.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|Atualiza as propriedades de um objeto [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .|

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
|prioridade|Int32|Prioridade do EnrollmentRestrictionsConfigurationPolicySetItem.|
|limite|Int32|Limite do EnrollmentRestrictionsConfigurationPolicySetItem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
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
  "priority": 1024,
  "limit": 1024
}
```




