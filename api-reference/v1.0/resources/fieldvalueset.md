---
author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
description: Representa os valores de coluna em um recurso listItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7986fdeb8ef3892ab149f14bc295929361d08971
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240049"
---
# <a name="fieldvalueset-resource"></a>Recurso de FieldValueSet

Namespace: microsoft.graph

Representa os valores de coluna em um recurso [listItem](listitem.md).

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **fieldValueSet**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
      "optionalProperties": ["Author", "AuthorLookupId", "Name", "Color", "Quantity" ],
       "baseType": "microsoft.graph.entity", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a>Propriedades

Cada campo de usuário visível em **listItem** é retornado como um par de nome e valor em **fieldValueSet**.
O exemplo acima é para uma lista que contém quatro colunas **Autor**, **Nome**, **Cor** e **Quantidade**.

Campos de pesquisa (como `Author` acima) não são retornados por padrão.
Em vez disso, o servidor retorna um campo 'LookupId' (como `AuthorLookupId` acima) referenciando o listItem direcionado na pesquisa.
O nome do campo 'LookupId' é o nome do campo original seguido de `LookupId`.

Até 12 campos de pesquisa podem ser solicitados em uma única consulta.
O servidor retornará valores de pesquisa se sua solicitação incluir uma instrução `select` com os campos necessários.
Exemplo:

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

você pode solicitar até 12 campos de pesquisa em uma única consulta, além de qualquer número de campos normais.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->

