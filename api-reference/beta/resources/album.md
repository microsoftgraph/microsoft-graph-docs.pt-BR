---
author: JeremyKelley
ms.author: jeremyke
title: tipo de recurso do álbum
description: Faceta descrevendo um pacote que é um álbum de fotos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 60d653db52f71de6fe4079df25223b393ea18da3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508356"
---
# <a name="album-resource-type"></a>tipo de recurso do álbum

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um álbum de fotos é uma maneira de agrupar virtualmente o [driveItems][driveItem] com facetas de [fotos][] em um [pacote][]. Os pacotes desse tipo terão a propriedade **Album** definida no recurso [Bundle][] .

## <a name="properties"></a>Propriedades

| Nome da propriedade     | Tipo   | Descrição
|:------------------|:-------|:------------------------------------------------
| coverImageItemId | String | Identificador exclusivo do [driveItem][] que é a tampa do álbum.

**Observação:** Se um **coverImageItemId** não tiver sido definido antes, as miniaturas de um álbum serão escolhidas automaticamente.
Após o **coverImageItemId** ter sido definido, as miniaturas de um álbum sempre serão o item associado a essa ID. Você pode substituir a capa padrão, CORRIGIndo o [][pacote] de itens do pacote e definindo a propriedade **coverImageItemId** no `album` para a ID de uma imagem contida no álbum.
Para remover uma tampa de conjunto personalizado, você pode definir a propriedade **coverImageItemId** como NULL, e um padrão será escolhido automaticamente.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[pacote]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
