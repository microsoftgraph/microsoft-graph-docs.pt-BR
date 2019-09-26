---
title: tipo de recurso deviceCompliancePolicyPolicySetItem
description: Uma classe que contém as propriedades usadas para a política de conformidade do dispositivo PolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 988c191771367d1197b8fe1654e2ba2483cdeb19
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199658"
---
# <a name="devicecompliancepolicypolicysetitem-resource-type"></a>tipo de recurso deviceCompliancePolicyPolicySetItem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a política de conformidade do dispositivo PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicyPolicySetItems](../api/intune-policyset-devicecompliancepolicypolicysetitem-list.md)|coleção [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Listar Propriedades e relações dos objetos [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|
|[Obter deviceCompliancePolicyPolicySetItem](../api/intune-policyset-devicecompliancepolicypolicysetitem-get.md)|[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Leia as propriedades e as relações do objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|
|[Criar deviceCompliancePolicyPolicySetItem](../api/intune-policyset-devicecompliancepolicypolicysetitem-create.md)|[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Criar um novo objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|
|[Excluir deviceCompliancePolicyPolicySetItem](../api/intune-policyset-devicecompliancepolicypolicysetitem-delete.md)|Nenhum|Exclui [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).|
|[Atualizar deviceCompliancePolicyPolicySetItem](../api/intune-policyset-devicecompliancepolicypolicysetitem-update.md)|[deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)|Atualiza as propriedades de um objeto [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .|

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
  "@odata.type": "microsoft.graph.deviceCompliancePolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
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



