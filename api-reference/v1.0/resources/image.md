---
author: JeremyKelley
ms.date: 09/10/2017
title: Imagem
localization_priority: Normal
description: O recurso Image agrupa propriedades relacionadas a imagens em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8667c3750556ed429a88b8b7b19a09c03481b394c2a59d14085566bd8fee1192
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231793"
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

