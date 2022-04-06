---
author: JeremyKelley
title: tipo de recurso bundle
description: Faceta descrevendo um driveItem que é um grupo lógico de outros driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3a17b133e79dfc670b486ca391112b45dbb3acf5
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724133"
---
# <a name="bundle-resource-type"></a>tipo de recurso bundle

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um pacote é um grupo lógico de arquivos usados para compartilhar vários arquivos ao mesmo tempo. Ele é representado por uma [entidade driveItem][] `bundle` que contém uma faceta e pode ser compartilhado da mesma forma que qualquer outro driveItem.

A `bundle` faceta em um [driveItem][] identifica um item como um pacote e agrupa informações específicas do pacote em uma única estrutura. Ele só está incluído nos [recursos driveItem][] **retornados** do ponto de extremidade de pacotes.

Observe que o `bundle` tipo de recurso em si não é uma entidade própria e é apenas uma faceta em [um driveItem][]. A `bundles` coleção em uma [unidade é][] do tipo [driveItem][], não `bundle`.

## <a name="methods"></a>Methods

| Método                            | Tipo de retorno              | Descrição                                    |
| :-------------------------------- | :----------------------- | :--------------------------------------------- |
| [Listar pacotes][bundle-list]       | Coleção [driveItem][] | Listar todos os pacotes em uma unidade                    |
| [Obter pacote][bundle-get]          | [driveItem][]            | Obter metadados de pacote                            |
| [Criar pacote][bundle-create]    | [driveItem][]            | Criar um novo pacote                            |
| [Adicionar item][bundle-add-item]       | Nenhum                     | Adicionar um [driveItem][] a um pacote existente      |
| [Remover item][bundle-remove-item] | Nenhum                     | Remover um [driveItem][] de um pacote existente |
| [Pacote de atualizações][bundle-update]    | [driveItem][]            | Atualizar metadados do pacote                         |
| [Excluir pacote][bundle-delete]    | Nenhum                     | Excluir pacote                                  |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo      | Descrição                                                          |
| :--------- | :-------- | :------------------------------------------------------------------- |
| childCount | Int32     | Número de filhos imediatamente neste contêiner.      |
| album      | [album][] | Se o pacote for um [álbum][], a propriedade `album` será incluída |

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.bundle" } -->

```json
{
  "childCount": 3,
  "album": { "@odata.type": "microsoft.graph.album" },
}
```

[album]: album.md
[drive]: drive.md
[driveItem]: driveItem.md

[bundle-list]: ../api/bundle-list.md
[bundle-get]: ../api/bundle-get.md
[bundle-create]: ../api/drive-post-bundles.md
[bundle-add-item]: ../api/bundle-addItem.md
[bundle-remove-item]: ../api/bundle-removeItem.md
[bundle-update]: ../api/bundle-update.md
[bundle-delete]: ../api/bundle-delete.md
