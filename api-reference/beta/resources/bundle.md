---
author: JeremyKelley
ms.author: jeremyke
title: tipo de recurso Bundle
description: Faceta descrevendo um driveItem que é um agrupamento lógico de outros driveItems
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 596dc8a77ce5b1e580b14e3e5c56c9e985b0dfbf
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932637"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="6b090-103">tipo de recurso Bundle</span><span class="sxs-lookup"><span data-stu-id="6b090-103">bundle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b090-104">Um pacote é um agrupamento lógico de arquivos usados para compartilhar vários arquivos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6b090-104">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="6b090-105">Ela é representada por uma entidade [driveItem][] que contém `bundle` uma faceta e pode ser compartilhada da mesma maneira que qualquer outra driveItem.</span><span class="sxs-lookup"><span data-stu-id="6b090-105">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="6b090-106">A `bundle` faceta em um [driveItem][] identifica um item como um pacote e agrupa informações específicas de pacote em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="6b090-106">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="6b090-107">Ele só é incluído nos recursos do [driveItem][] retornados do ponto de extremidade de **pacotes** .</span><span class="sxs-lookup"><span data-stu-id="6b090-107">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="6b090-108">Observe que o `bundle` tipo de recurso em si não é uma entidade própria e é apenas uma faceta em um [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="6b090-108">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="6b090-109">A `bundles` coleção em uma [unidade][] é do tipo [driveItem][], e `bundle`não.</span><span class="sxs-lookup"><span data-stu-id="6b090-109">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="6b090-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b090-110">Methods</span></span>

|                        <span data-ttu-id="6b090-111">Método</span><span class="sxs-lookup"><span data-stu-id="6b090-111">Method</span></span>             |         <span data-ttu-id="6b090-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b090-112">Return type</span></span>      | <span data-ttu-id="6b090-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b090-113">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="6b090-114">[Listar pacotes][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="6b090-114">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="6b090-115">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6b090-115">[driveItem][] collection</span></span> | <span data-ttu-id="6b090-116">Listar todos os pacotes em uma unidade</span><span class="sxs-lookup"><span data-stu-id="6b090-116">List all bundles in a drive</span></span> |
| <span data-ttu-id="6b090-117">[Obter pacote][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="6b090-117">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="6b090-118">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6b090-118">[driveItem][]</span></span>            | <span data-ttu-id="6b090-119">Obter metadados de pacote</span><span class="sxs-lookup"><span data-stu-id="6b090-119">Get bundle metadata</span></span> |
| <span data-ttu-id="6b090-120">[Criar pacote][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="6b090-120">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="6b090-121">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6b090-121">[driveItem][]</span></span>            | <span data-ttu-id="6b090-122">Criar um novo pacote</span><span class="sxs-lookup"><span data-stu-id="6b090-122">Create a new bundle</span></span> |
| <span data-ttu-id="6b090-123">[Adicionar item][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="6b090-123">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="6b090-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b090-124">None</span></span>                     | <span data-ttu-id="6b090-125">Adicionar um [driveItem][] a um pacote existente</span><span class="sxs-lookup"><span data-stu-id="6b090-125">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="6b090-126">[Remover item][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="6b090-126">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="6b090-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b090-127">None</span></span>                     | <span data-ttu-id="6b090-128">Remover um [driveItem][] de um pacote existente</span><span class="sxs-lookup"><span data-stu-id="6b090-128">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="6b090-129">[Pacote de atualização][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="6b090-129">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="6b090-130">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6b090-130">[driveItem][]</span></span>            | <span data-ttu-id="6b090-131">Atualizar metadados do pacote</span><span class="sxs-lookup"><span data-stu-id="6b090-131">Update bundle metadata</span></span> |
| <span data-ttu-id="6b090-132">[Excluir pacote][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="6b090-132">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="6b090-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b090-133">None</span></span>                     | <span data-ttu-id="6b090-134">Excluir pacote</span><span class="sxs-lookup"><span data-stu-id="6b090-134">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="6b090-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b090-135">Properties</span></span>

| <span data-ttu-id="6b090-136">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6b090-136">Property name</span></span> | <span data-ttu-id="6b090-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b090-137">Type</span></span>      | <span data-ttu-id="6b090-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b090-138">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="6b090-139">childCount</span><span class="sxs-lookup"><span data-stu-id="6b090-139">childCount</span></span>    | <span data-ttu-id="6b090-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6b090-140">Int32</span></span>     | <span data-ttu-id="6b090-141">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="6b090-141">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="6b090-142">album</span><span class="sxs-lookup"><span data-stu-id="6b090-142">album</span></span>         | <span data-ttu-id="6b090-143">[album][]</span><span class="sxs-lookup"><span data-stu-id="6b090-143">[album][]</span></span> | <span data-ttu-id="6b090-144">Se o pacote for um [álbum][], a `album` propriedade será incluída</span><span class="sxs-lookup"><span data-stu-id="6b090-144">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b090-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b090-145">JSON representation</span></span>

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
