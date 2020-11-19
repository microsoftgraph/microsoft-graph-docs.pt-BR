---
title: tipo de recurso policyset
description: Uma classe que contém as propriedades usadas para Policyset.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f94f9f85dbad85b803a8fc4656aa658b3d6372ad
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256103"
---
# <a name="policyset-resource-type"></a>tipo de recurso policyset

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para Policyset.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar policySets](../api/intune-policyset-policyset-list.md)|coleção [policyset](../resources/intune-policyset-policyset.md)|Listar Propriedades e relações dos objetos [policyset](../resources/intune-policyset-policyset.md) .|
|[Obter policyset](../api/intune-policyset-policyset-get.md)|[policySet](../resources/intune-policyset-policyset.md)|Leia as propriedades e as relações do objeto [policyset](../resources/intune-policyset-policyset.md) .|
|[Criar policyset](../api/intune-policyset-policyset-create.md)|[policySet](../resources/intune-policyset-policyset.md)|Criar um novo objeto [policyset](../resources/intune-policyset-policyset.md) .|
|[Excluir policyset](../api/intune-policyset-policyset-delete.md)|Nenhum|Exclui um [policyset](../resources/intune-policyset-policyset.md).|
|[Atualizar políticas](../api/intune-policyset-policyset-update.md)|[policySet](../resources/intune-policyset-policyset.md)|Atualiza as propriedades de um objeto [policyset](../resources/intune-policyset-policyset.md) .|
|[ação Update](../api/intune-policyset-policyset-update.md)|Nenhuma|Ainda não documentado|
|[ação getPolicySets](../api/intune-policyset-policyset-getpolicysets.md)|coleção [policyset](../resources/intune-policyset-policyset.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do Policyset.|
|createdDateTime|DateTimeOffset|Hora de criação do Policyset.|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação do Policyset.|
|displayName|String|DisplayName do Policyset.|
|description|String|Descrição do Policyset.|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status de validação/atribuição do Policyset. Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro, caso algum tenha ocorrido. Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Coleção de cadeias de caracteres|Marcas da implantação dirigida|
|roleScopeTags|Coleção de cadeias de caracteres|RoleScopeTags do Policyset|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Atribuições de Policyset.|
|items|coleção [policySetItem](../resources/intune-policyset-policysetitem.md)|Itens do Policyset com contagem máxima de 100.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "roleScopeTags": [
    "String"
  ]
}
```




