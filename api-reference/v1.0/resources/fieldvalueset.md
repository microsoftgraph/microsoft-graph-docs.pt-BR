---
author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
ms.localizationpriority: medium
description: Representa os valores de coluna em um recurso listItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59124bdf897bb7a388c54d57a151fd5383502421
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036512"
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

