---
author: JeremyKelley
ms.date: 09/10/2017
title: Imagem
ms.localizationpriority: medium
description: O recurso Image agrupa propriedades relacionadas a imagens em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5ccc3baf969199161936ffd635790c56ab75363
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089722"
---
# <a name="image-resource-type"></a>Tipo de recurso Image

Namespace: microsoft.graph

O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.

**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.

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

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->

