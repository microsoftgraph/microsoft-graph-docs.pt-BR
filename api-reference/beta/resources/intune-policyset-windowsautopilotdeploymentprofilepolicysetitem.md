---
title: Tipo de recurso windowsAutopilotDeploymentProfilePolicySetItem
description: Uma classe que contém as propriedades usadas para o perfil de implantação do windows autopilot PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdc0df8699de0f6d34e102b8248a47896802f60a
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255212"
---
# <a name="windowsautopilotdeploymentprofilepolicysetitem-resource-type"></a>Tipo de recurso windowsAutopilotDeploymentProfilePolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para o perfil de implantação do windows autopilot PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsAutopilotDeploymentProfilePolicySetItems](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-list.md)|[Coleção windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Listar propriedades e relações dos [objetos windowsAutopilotDeploymentProfilePolicySetItem.](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|
|[Obter windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-get.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Leia propriedades e relações do [objeto windowsAutopilotDeploymentProfilePolicySetItem.](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|
|[Criar windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-create.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Crie um novo [objeto windowsAutopilotDeploymentProfilePolicySetItem.](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|
|[Excluir windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-delete.md)|Nenhum|Exclui um [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).|
|[Atualizar windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-update.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|Atualize as propriedades de um [objeto windowsAutopilotDeploymentProfilePolicySetItem.](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|

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
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
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




