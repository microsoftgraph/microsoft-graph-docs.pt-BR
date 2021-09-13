---
title: Tipo de recurso policySet
description: Uma classe que contém as propriedades usadas para PolicySet.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3216acbfaf03e0edc61eb87cbe8419c22227f9b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074882"
---
# <a name="policyset-resource-type"></a>Tipo de recurso policySet

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para PolicySet.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar policySets](../api/intune-policyset-policyset-list.md)|[Coleção policySet](../resources/intune-policyset-policyset.md)|Listar propriedades e relações dos [objetos policySet.](../resources/intune-policyset-policyset.md)|
|[Obter policySet](../api/intune-policyset-policyset-get.md)|[policySet](../resources/intune-policyset-policyset.md)|Leia propriedades e relações do [objeto policySet.](../resources/intune-policyset-policyset.md)|
|[Criar policySet](../api/intune-policyset-policyset-create.md)|[policySet](../resources/intune-policyset-policyset.md)|Crie um novo [objeto policySet.](../resources/intune-policyset-policyset.md)|
|[Excluir policySet](../api/intune-policyset-policyset-delete.md)|Nenhum|Exclui um [policySet](../resources/intune-policyset-policyset.md).|
|[Atualizar policySet](../api/intune-policyset-policyset-update.md)|[policySet](../resources/intune-policyset-policyset.md)|Atualize as propriedades de um [objeto policySet.](../resources/intune-policyset-policyset.md)|
|[ação de atualização](../api/intune-policyset-policyset-update.md)|Nenhuma|Ainda não documentado|
|[Ação getPolicySets](../api/intune-policyset-policyset-getpolicysets.md)|[Coleção policySet](../resources/intune-policyset-policyset.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do PolicySet.|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySet.|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySet.|
|displayName|String|DisplayName do PolicySet.|
|description|Cadeia de caracteres|Descrição do PolicySet.|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status de validação/atribuição do PolicySet. Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Conjunto de cadeias de caracteres|Marcas da implantação guiada|
|roleScopeTags|Conjunto de cadeias de caracteres|RoleScopeTags do PolicySet|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Atribuições do PolicySet.|
|itens|[Coleção policySetItem](../resources/intune-policyset-policysetitem.md)|Itens do PolicySet com contagem máxima 100.|

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



