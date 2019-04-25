---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: 163bbb9595da84628a0e9d8ca449fdafbf4089b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565062"
---
# <a name="fieldvalueset-resource"></a>Recurso de FieldValueSet

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
