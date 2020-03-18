---
title: tipo de recurso groupPolicyCategory
description: A entidade de categoria armazena a categoria de uma definição de política de grupo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b754020cc4a7c4f7e9fdf7cc35f74d9dcc4c4c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783120"
---
# <a name="grouppolicycategory-resource-type"></a>tipo de recurso groupPolicyCategory

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de categoria armazena a categoria de uma definição de política de grupo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-get.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Leia as propriedades e as relações do objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .|
|[Atualizar groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-update.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Atualiza as propriedades de um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|A ID da cadeia de caracteres do nome de exibição da categoria|
|IsRoot|Boolean|Define se a categoria é uma categoria raiz|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|primário|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|A categoria pai|
|children|coleção [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|As categorias filhas|
|Definição|coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Os filhos GroupPolicyDefinition imediatos da categoria|
|DefinitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|A ID do arquivo de definição do qual a categoria provém|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



