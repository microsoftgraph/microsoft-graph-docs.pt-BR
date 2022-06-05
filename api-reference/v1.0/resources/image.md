---
author: JeremyKelley
title: tipo de recurso de imagem
ms.localizationpriority: medium
description: O recurso de imagem agrupa propriedades relacionadas à imagem em uma única estrutura.
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 1c457a139504615cde6e21628e82c8875a47b6a9
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900524"
---
# <a name="image-resource-type"></a>tipo de recurso de imagem

Namespace: microsoft.graph

O **recurso de** imagem agrupa propriedades relacionadas à imagem em uma única estrutura.
Se um [**driveItem**](driveitem.md) tiver uma faceta de  imagem não nula, o item representará uma imagem de bitmap.

>**Nota:** Se o serviço não puder determinar a largura e a altura da imagem, o recurso **de** imagem poderá estar vazio.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo  | Descrição                                |
|:-----------|:------|:-------------------------------------------|
| **height** | Int32 | Opcional. A altura da imagem em pixels. Somente leitura. |
| **width**  | Int32 | Opcional. A largura da imagem em pixels. Somente leitura.  |

## <a name="remarks"></a>Comentários

No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo.

Para obter mais informações sobre as facetas em um DriveItem, consulte [driveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->

