---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 0d0c5a34d12fe467196c0616befc7376835b632c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481724"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="5ea96-102">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="5ea96-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="5ea96-103">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5ea96-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ea96-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ea96-104">JSON representation</span></span>

<span data-ttu-id="5ea96-105">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="5ea96-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="5ea96-106">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="5ea96-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="5ea96-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ea96-107">Properties</span></span>

| <span data-ttu-id="5ea96-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ea96-108">Property</span></span> | <span data-ttu-id="5ea96-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea96-109">Type</span></span>                          | <span data-ttu-id="5ea96-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea96-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="5ea96-111">id</span><span class="sxs-lookup"><span data-stu-id="5ea96-111">id</span></span>       | <span data-ttu-id="5ea96-112">String</span><span class="sxs-lookup"><span data-stu-id="5ea96-112">String</span></span>                        | <span data-ttu-id="5ea96-113">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="5ea96-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="5ea96-114">name</span><span class="sxs-lookup"><span data-stu-id="5ea96-114">name</span></span>     | <span data-ttu-id="5ea96-115">String</span><span class="sxs-lookup"><span data-stu-id="5ea96-115">String</span></span>                        | <span data-ttu-id="5ea96-116">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5ea96-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="5ea96-117">owner</span><span class="sxs-lookup"><span data-stu-id="5ea96-117">owner</span></span>    | [<span data-ttu-id="5ea96-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="5ea96-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="5ea96-119">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="5ea96-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5ea96-120">Relações</span><span class="sxs-lookup"><span data-stu-id="5ea96-120">Relationships</span></span>

| <span data-ttu-id="5ea96-121">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="5ea96-121">Relationship name</span></span> | <span data-ttu-id="5ea96-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea96-122">Type</span></span>                | <span data-ttu-id="5ea96-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea96-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="5ea96-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="5ea96-124">**driveItem**</span></span>     | <span data-ttu-id="5ea96-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="5ea96-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="5ea96-126">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="5ea96-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="5ea96-127">**list**</span><span class="sxs-lookup"><span data-stu-id="5ea96-127">**list**</span></span>          | <span data-ttu-id="5ea96-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="5ea96-128">[**list**][list]</span></span>        | <span data-ttu-id="5ea96-129">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="5ea96-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="5ea96-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="5ea96-130">**listItem**</span></span>      | <span data-ttu-id="5ea96-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="5ea96-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="5ea96-132">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="5ea96-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="5ea96-133">**site**</span><span class="sxs-lookup"><span data-stu-id="5ea96-133">**site**</span></span>          | <span data-ttu-id="5ea96-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="5ea96-134">[**site**][site]</span></span>        | <span data-ttu-id="5ea96-135">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="5ea96-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="5ea96-136">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="5ea96-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="5ea96-137">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="5ea96-137">Relationship name</span></span> | <span data-ttu-id="5ea96-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea96-138">Type</span></span>                         | <span data-ttu-id="5ea96-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea96-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="5ea96-140">**items**</span><span class="sxs-lookup"><span data-stu-id="5ea96-140">**items**</span></span>         | <span data-ttu-id="5ea96-141">Coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="5ea96-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="5ea96-142">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="5ea96-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="5ea96-143">Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="5ea96-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="5ea96-144">**root**</span><span class="sxs-lookup"><span data-stu-id="5ea96-144">**root**</span></span>          | <span data-ttu-id="5ea96-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="5ea96-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="5ea96-146">Usado para acessar o **driveItem**subjacente.</span><span class="sxs-lookup"><span data-stu-id="5ea96-146">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="5ea96-147">PreTerido-- `driveItem` use em vez disso.</span><span class="sxs-lookup"><span data-stu-id="5ea96-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="5ea96-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ea96-148">Methods</span></span>

| <span data-ttu-id="5ea96-149">Método</span><span class="sxs-lookup"><span data-stu-id="5ea96-149">Method</span></span>                                  | <span data-ttu-id="5ea96-150">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="5ea96-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="5ea96-151">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="5ea96-151">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="5ea96-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="5ea96-152">Remarks</span></span>

<span data-ttu-id="5ea96-153">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5ea96-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
