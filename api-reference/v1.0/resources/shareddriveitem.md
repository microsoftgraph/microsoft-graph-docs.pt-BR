---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f6684e9c266a800f5a76a7085a8af22ea9518e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034332"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="87e3f-103">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="87e3f-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="87e3f-104">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="87e3f-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="87e3f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87e3f-105">JSON representation</span></span>

<span data-ttu-id="87e3f-106">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="87e3f-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="87e3f-107">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="87e3f-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="87e3f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87e3f-108">Properties</span></span>

| <span data-ttu-id="87e3f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87e3f-109">Property</span></span> | <span data-ttu-id="87e3f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e3f-110">Type</span></span>                          | <span data-ttu-id="87e3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87e3f-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="87e3f-112">id</span><span class="sxs-lookup"><span data-stu-id="87e3f-112">id</span></span>       | <span data-ttu-id="87e3f-113">String</span><span class="sxs-lookup"><span data-stu-id="87e3f-113">String</span></span>                        | <span data-ttu-id="87e3f-114">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="87e3f-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="87e3f-115">name</span><span class="sxs-lookup"><span data-stu-id="87e3f-115">name</span></span>     | <span data-ttu-id="87e3f-116">String</span><span class="sxs-lookup"><span data-stu-id="87e3f-116">String</span></span>                        | <span data-ttu-id="87e3f-117">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="87e3f-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="87e3f-118">owner</span><span class="sxs-lookup"><span data-stu-id="87e3f-118">owner</span></span>    | [<span data-ttu-id="87e3f-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="87e3f-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="87e3f-120">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="87e3f-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="87e3f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="87e3f-121">Relationships</span></span>

| <span data-ttu-id="87e3f-122">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="87e3f-122">Relationship name</span></span> | <span data-ttu-id="87e3f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e3f-123">Type</span></span>                | <span data-ttu-id="87e3f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="87e3f-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="87e3f-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="87e3f-125">**driveItem**</span></span>     | <span data-ttu-id="87e3f-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="87e3f-126">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="87e3f-127">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="87e3f-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="87e3f-128">**list**</span><span class="sxs-lookup"><span data-stu-id="87e3f-128">**list**</span></span>          | <span data-ttu-id="87e3f-129">[**lista**][list]</span><span class="sxs-lookup"><span data-stu-id="87e3f-129">[**list**][list]</span></span>        | <span data-ttu-id="87e3f-130">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="87e3f-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="87e3f-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="87e3f-131">**listItem**</span></span>      | <span data-ttu-id="87e3f-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="87e3f-132">[**listItem**][listItem]</span></span>    | <span data-ttu-id="87e3f-133">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="87e3f-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="87e3f-134">**site**</span><span class="sxs-lookup"><span data-stu-id="87e3f-134">**site**</span></span>          | <span data-ttu-id="87e3f-135">[**no**][site]</span><span class="sxs-lookup"><span data-stu-id="87e3f-135">[**site**][site]</span></span>        | <span data-ttu-id="87e3f-136">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="87e3f-136">Used to access the underlying **site**</span></span>

<span data-ttu-id="87e3f-137">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="87e3f-137">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="87e3f-138">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="87e3f-138">Relationship name</span></span> | <span data-ttu-id="87e3f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e3f-139">Type</span></span>                         | <span data-ttu-id="87e3f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="87e3f-140">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="87e3f-141">**items**</span><span class="sxs-lookup"><span data-stu-id="87e3f-141">**items**</span></span>         | <span data-ttu-id="87e3f-142">coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="87e3f-142">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="87e3f-143">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="87e3f-143">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="87e3f-144">Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="87e3f-144">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="87e3f-145">**root**</span><span class="sxs-lookup"><span data-stu-id="87e3f-145">**root**</span></span>          | <span data-ttu-id="87e3f-146">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="87e3f-146">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="87e3f-147">Usado para acessar o **driveItem**subjacente.</span><span class="sxs-lookup"><span data-stu-id="87e3f-147">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="87e3f-148">Preterido-- `driveItem` use em vez disso.</span><span class="sxs-lookup"><span data-stu-id="87e3f-148">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="87e3f-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="87e3f-149">Methods</span></span>

| <span data-ttu-id="87e3f-150">Método</span><span class="sxs-lookup"><span data-stu-id="87e3f-150">Method</span></span>                                  | <span data-ttu-id="87e3f-151">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="87e3f-151">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="87e3f-152">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="87e3f-152">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="87e3f-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="87e3f-153">Remarks</span></span>

<span data-ttu-id="87e3f-154">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="87e3f-154">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
