---
title: tipo de recurso de esquema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências Graph Microsoft.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5ca338e6e2d2da30e555223c3257da7d7f2f497d1a2a15a9436ed5b8568575bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189790"
---
# <a name="schema-resource-type"></a>tipo de recurso de esquema

Namespace: microsoft.graph.externalConnectors

O [esquema](externalconnectors-externalconnection.md) de conexão determina como seu conteúdo externo será usado em várias experiências Graph Microsoft. O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão, juntamente com seus atributos, rótulos e aliases. Você deve registrá-lo antes de adicionar itens na conexão.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar esquema](../api/externalconnectors-schema-create.md)|[schema](../resources/externalconnectors-schema.md)|Crie um novo [objeto de esquema.](../resources/externalconnectors-schema.md)|
|[Obter esquema](../api/externalconnectors-schema-get.md)|[schema](../resources/externalconnectors-schema.md)|Leia as propriedades e as relações de um [objeto de esquema.](../resources/externalconnectors-schema.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|baseType|String|Deve ser definida como `microsoft.graph.externalConnector.externalItem`. Obrigatório.|
|properties|[coleção property](../resources/externalconnectors-property.md)|As propriedades definidas para os itens na conexão. O número mínimo de propriedades é um, o máximo é 128.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "openType": false
}
-->
``` json
{
  "baseType": "String",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

