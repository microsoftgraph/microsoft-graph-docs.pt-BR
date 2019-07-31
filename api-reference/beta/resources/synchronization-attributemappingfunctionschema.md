---
title: tipo de recurso attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0222a01f2bcea819624d1dcb9f53da7ea0b86b25
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007988"
---
# <a name="attributemappingfunctionschema-resource-type"></a>tipo de recurso attributeMappingFunctionSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve uma função que pode ser usada em um [mapeamento de atributo](synchronization-attributemapping.md) para transformar valores durante a sincronização.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)|Listar funções de mapeamento de atributos com suporte.|

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:-------------------------|:---------------|
|name                        |String                    |Nome do operador. |
|parameters                  |coleção [attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)  |Conjunto de parâmetros de função.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
