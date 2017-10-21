---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pacote
ms.openlocfilehash: 33be73ed79438bdf28b76747b6efb79290be8d0c
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="package-resource-type"></a>Tipo de recurso de pacote

O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.

Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.

DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| Nome da Propriedade | Tipo   | Descrição                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **type**      | string | Uma cadeia de caracteres indicando o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada. |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
