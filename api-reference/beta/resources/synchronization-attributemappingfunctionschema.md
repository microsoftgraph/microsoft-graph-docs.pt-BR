---
title: tipo de recurso attributeMappingFunctionSchema
description: Descreve uma função que pode ser usada em um mapeamento de atributo para transformar valores durante a sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 16dae5dca65b3d238c2d12fddc2b474e7e03ac0d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219176"
---
# <a name="attributemappingfunctionschema-resource-type"></a>tipo de recurso attributeMappingFunctionSchema

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve uma função que pode ser usada em um [mapeamento de atributo](synchronization-attributemapping.md) para transformar valores durante a sincronização.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | coleção [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)|Listar funções de mapeamento de atributos com suporte.|

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:-------------------------|:---------------|
|nome                        |String                    |Nome do operador. |
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
