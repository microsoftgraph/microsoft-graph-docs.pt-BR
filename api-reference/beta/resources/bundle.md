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
# <a name="bundle-resource-type"></a><span data-ttu-id="e618e-103">tipo de recurso Bundle</span><span class="sxs-lookup"><span data-stu-id="e618e-103">bundle resource type</span></span>

<span data-ttu-id="e618e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e618e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e618e-105">Um pacote é um agrupamento lógico de arquivos usados para compartilhar vários arquivos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="e618e-105">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="e618e-106">Ela é representada por uma entidade [driveItem][] que contém `bundle` uma faceta e pode ser compartilhada da mesma maneira que qualquer outra driveItem.</span><span class="sxs-lookup"><span data-stu-id="e618e-106">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="e618e-107">A `bundle` faceta em um [driveItem][] identifica um item como um pacote e agrupa informações específicas de pacote em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="e618e-107">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="e618e-108">Ele só é incluído nos recursos do [driveItem][] retornados do ponto de extremidade de **pacotes** .</span><span class="sxs-lookup"><span data-stu-id="e618e-108">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="e618e-109">Observe que o `bundle` tipo de recurso em si não é uma entidade própria e é apenas uma faceta em um [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="e618e-109">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="e618e-110">A `bundles` coleção em uma [unidade][] é do tipo [driveItem][], e `bundle`não.</span><span class="sxs-lookup"><span data-stu-id="e618e-110">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="e618e-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="e618e-111">Methods</span></span>

|                        <span data-ttu-id="e618e-112">Método</span><span class="sxs-lookup"><span data-stu-id="e618e-112">Method</span></span>             |         <span data-ttu-id="e618e-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e618e-113">Return type</span></span>      | <span data-ttu-id="e618e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e618e-114">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="e618e-115">[Listar pacotes][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="e618e-115">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="e618e-116">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e618e-116">[driveItem][] collection</span></span> | <span data-ttu-id="e618e-117">Listar todos os pacotes em uma unidade</span><span class="sxs-lookup"><span data-stu-id="e618e-117">List all bundles in a drive</span></span> |
| <span data-ttu-id="e618e-118">[Obter pacote][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="e618e-118">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="e618e-119">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e618e-119">[driveItem][]</span></span>            | <span data-ttu-id="e618e-120">Obter metadados de pacote</span><span class="sxs-lookup"><span data-stu-id="e618e-120">Get bundle metadata</span></span> |
| <span data-ttu-id="e618e-121">[Criar pacote][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="e618e-121">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="e618e-122">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e618e-122">[driveItem][]</span></span>            | <span data-ttu-id="e618e-123">Criar um novo pacote</span><span class="sxs-lookup"><span data-stu-id="e618e-123">Create a new bundle</span></span> |
| <span data-ttu-id="e618e-124">[Adicionar item][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="e618e-124">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="e618e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e618e-125">None</span></span>                     | <span data-ttu-id="e618e-126">Adicionar um [driveItem][] a um pacote existente</span><span class="sxs-lookup"><span data-stu-id="e618e-126">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="e618e-127">[Remover item][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="e618e-127">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="e618e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e618e-128">None</span></span>                     | <span data-ttu-id="e618e-129">Remover um [driveItem][] de um pacote existente</span><span class="sxs-lookup"><span data-stu-id="e618e-129">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="e618e-130">[Pacote de atualização][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="e618e-130">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="e618e-131">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e618e-131">[driveItem][]</span></span>            | <span data-ttu-id="e618e-132">Atualizar metadados do pacote</span><span class="sxs-lookup"><span data-stu-id="e618e-132">Update bundle metadata</span></span> |
| <span data-ttu-id="e618e-133">[Excluir pacote][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="e618e-133">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="e618e-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e618e-134">None</span></span>                     | <span data-ttu-id="e618e-135">Excluir pacote</span><span class="sxs-lookup"><span data-stu-id="e618e-135">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="e618e-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e618e-136">Properties</span></span>

| <span data-ttu-id="e618e-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e618e-137">Property name</span></span> | <span data-ttu-id="e618e-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="e618e-138">Type</span></span>      | <span data-ttu-id="e618e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="e618e-139">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="e618e-140">childCount</span><span class="sxs-lookup"><span data-stu-id="e618e-140">childCount</span></span>    | <span data-ttu-id="e618e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e618e-141">Int32</span></span>     | <span data-ttu-id="e618e-142">Número de filhos imediatamente neste contêiner.</span><span class="sxs-lookup"><span data-stu-id="e618e-142">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="e618e-143">album</span><span class="sxs-lookup"><span data-stu-id="e618e-143">album</span></span>         | <span data-ttu-id="e618e-144">[album][]</span><span class="sxs-lookup"><span data-stu-id="e618e-144">[album][]</span></span> | <span data-ttu-id="e618e-145">Se o pacote for um [álbum][], a `album` propriedade será incluída</span><span class="sxs-lookup"><span data-stu-id="e618e-145">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="e618e-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e618e-146">JSON representation</span></span>

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
