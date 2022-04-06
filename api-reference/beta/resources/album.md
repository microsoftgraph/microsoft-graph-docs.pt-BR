---
author: JeremyKelley
title: tipo de recurso de álbum
description: Faceta descrevendo um pacote que é um álbum de fotos.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0f35eea761a467ce1a733f07fca5c33a218be030
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723219"
---
# <a name="album-resource-type"></a>tipo de recurso de álbum

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um álbum de fotos é uma maneira de agrupar virtualmente [driveItemsdriveItem][] [com][] facetas de foto juntas em um [pacote][]. Os pacotes desse tipo terão a propriedade **album** definida no recurso [bundle][] .

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo   | Descrição                                                            |
| :--------------- | :----- | :--------------------------------------------------------------------- |
| coverImageItemId | String | Identificador exclusivo do [driveItem][] que é a capa do álbum. |

**Observação:** Se um **coverImageItemId** não tiver sido definido antes, as miniaturas de um álbum serão escolhidas automaticamente.
Depois **que coverImageItemId** for definido, as miniaturas de um álbum sempre serão o item associado a essa id. Você pode substituir a capa padrão por PATCHing o [item] [do pacote e] definir a **propriedade coverImageItemId** `album` na id de uma imagem contida no álbum.
Para remover uma capa de conjunto personalizado, você pode definir a **propriedade coverImageItemId** como nula e uma padrão será escolhida automaticamente novamente.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[Agrupar]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
