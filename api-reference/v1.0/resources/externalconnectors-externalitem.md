---
title: Tipo de recurso externalItem
description: Um item adicionado a uma conexão Graph Microsoft.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e50a494898faa377123e96238dee0bf1109d798d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123444"
---
# <a name="externalitem-resource-type"></a>Tipo de recurso externalItem

Namespace: microsoft.graph.externalConnectors

Um item adicionado a uma conexão microsoft Graph [.](externalconnectors-externalconnection.md) 

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar externalItem](../api/externalconnectors-externalitem-create.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Crie um novo [objeto externalItem.](../resources/externalconnectors-externalitem.md)|
|[Obter externalItem](../api/externalconnectors-externalitem-get.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Leia as propriedades e as relações de um [objeto externalItem.](../resources/externalconnectors-externalitem.md)|
|[Atualizar externalItem](../api/externalconnectors-externalitem-update.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Atualize as propriedades de [um objeto externalItem.](../resources/externalconnectors-externalitem.md)|
|[Excluir externalItem](../api/externalconnectors-externalitem-delete.md)|Nenhum(a)|Exclui um [objeto externalItem.](../resources/externalconnectors-externalitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acl|[Coleção microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)|Uma matriz de entradas de controle de acesso. Cada entrada especifica o acesso concedido a um usuário ou grupo. Obrigatório.|
|conteúdo|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|Uma representação em texto sem texto do conteúdo do item. O texto nesta propriedade é indexado em texto completo. Opcional.|
|id|Cadeia de caracteres|ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnectors-externalconnection.md). Deve ser alfanumérico e um máximo de 128 caracteres. Obrigatório.|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|Um pacote de propriedades com as propriedades do item. As propriedades DEVEM estar em conformidade [com o esquema](externalconnectors-schema.md) definido para [externalConnection](externalconnectors-externalconnection.md). Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "openType": false
}
-->
```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ],
  "id": "String (identifier)",
  "properties": {
    "@odata.type": "microsoft.graph.externalConnectors.properties"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
  }
}
```

