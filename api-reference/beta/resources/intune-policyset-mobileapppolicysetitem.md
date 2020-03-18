---
title: tipo de recurso mobileAppPolicySetItem
description: Uma classe que contém as propriedades usadas para aplicativos móveis PolicySetItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2e9b9714fb543c0b8cb09df297382f75c259d0ce
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775258"
---
# <a name="mobileapppolicysetitem-resource-type"></a>tipo de recurso mobileAppPolicySetItem

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para aplicativos móveis PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppPolicySetItems](../api/intune-policyset-mobileapppolicysetitem-list.md)|coleção [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Listar Propriedades e relações dos objetos [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Obter mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-get.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Leia as propriedades e as relações do objeto [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Criar mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-create.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Criar um novo objeto [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Excluir mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-delete.md)|Nenhum|Exclui [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).|
|[Atualizar mobileAppPolicySetItem](../api/intune-policyset-mobileapppolicysetitem-update.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Atualiza as propriedades de um objeto [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do MobileAppPolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro, caso algum tenha ocorrido. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Coleção de cadeias de caracteres|Marcas da implantação dirigida herdadas de [policySetItem](../resources/intune-policyset-policysetitem.md)|
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
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



