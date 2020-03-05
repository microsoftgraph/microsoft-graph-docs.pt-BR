---
author: JeremyKelley
ms.author: jeremyke
title: tipo de recurso Bundle
description: Faceta descrevendo um driveItem que é um agrupamento lógico de outros driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ae03674970c8861c7d1c158e62662d9691e74789
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507863"
---
# <a name="bundle-resource-type"></a>tipo de recurso Bundle

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um pacote é um agrupamento lógico de arquivos usados para compartilhar vários arquivos ao mesmo tempo. Ela é representada por uma entidade [driveItem][] que contém `bundle` uma faceta e pode ser compartilhada da mesma maneira que qualquer outra driveItem.

A `bundle` faceta em um [driveItem][] identifica um item como um pacote e agrupa informações específicas de pacote em uma única estrutura. Ele só é incluído nos recursos do [driveItem][] retornados do ponto de extremidade de **pacotes** .

Observe que o `bundle` tipo de recurso em si não é uma entidade própria e é apenas uma faceta em um [driveItem][]. A `bundles` coleção em uma [unidade][] é do tipo [driveItem][], e `bundle`não.

## <a name="methods"></a>Métodos

|                        Método             |         Tipo de retorno      | Descrição        |
| :---------------------------------------- | :----------------------- | :------------------|
| [Listar pacotes][bundle-list]               | Coleção [driveItem][] | Listar todos os pacotes em uma unidade |
| [Obter pacote][bundle-get]                  | [driveItem][]            | Obter metadados de pacote |
| [Criar pacote][bundle-create]            | [driveItem][]            | Criar um novo pacote |
| [Adicionar item][bundle-add-item]               | Nenhum                     | Adicionar um [driveItem][] a um pacote existente |
| [Remover item][bundle-remove-item]         | Nenhum                     | Remover um [driveItem][] de um pacote existente |
| [Pacote de atualização][bundle-update]            | [driveItem][]            | Atualizar metadados do pacote |
| [Excluir pacote][bundle-delete]            | Nenhum                     | Excluir pacote |


## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo      | Descrição
|:--------------|:----------|:------------------------------------------------
| childCount    | Int32     | Número de filhos imediatamente neste contêiner.
| album         | [album][] | Se o pacote for um [álbum][], a `album` propriedade será incluída

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
