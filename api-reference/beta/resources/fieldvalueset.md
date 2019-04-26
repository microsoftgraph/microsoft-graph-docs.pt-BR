---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: 4f8b193045bdc7c4e0286067c46c31693a66dfb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340237"
---
# <a name="fieldvalueset-resource"></a>Recurso de FieldValueSet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os valores de coluna em um recurso [listItem](listitem.md).

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **fieldValueSet**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": []
}
-->
