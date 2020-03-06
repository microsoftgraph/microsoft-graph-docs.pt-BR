---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9864d982e58304c684b267c59ec1925aec8baeff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533732"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="94ad1-103">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="94ad1-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="94ad1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94ad1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94ad1-105">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94ad1-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="94ad1-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94ad1-106">JSON representation</span></span>

<span data-ttu-id="94ad1-107">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="94ad1-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="94ad1-108">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="94ad1-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="94ad1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94ad1-109">Properties</span></span>

| <span data-ttu-id="94ad1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94ad1-110">Property</span></span> | <span data-ttu-id="94ad1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="94ad1-111">Type</span></span>                          | <span data-ttu-id="94ad1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="94ad1-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="94ad1-113">id</span><span class="sxs-lookup"><span data-stu-id="94ad1-113">id</span></span>       | <span data-ttu-id="94ad1-114">String</span><span class="sxs-lookup"><span data-stu-id="94ad1-114">String</span></span>                        | <span data-ttu-id="94ad1-115">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="94ad1-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="94ad1-116">nome</span><span class="sxs-lookup"><span data-stu-id="94ad1-116">name</span></span>     | <span data-ttu-id="94ad1-117">String</span><span class="sxs-lookup"><span data-stu-id="94ad1-117">String</span></span>                        | <span data-ttu-id="94ad1-118">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94ad1-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="94ad1-119">owner</span><span class="sxs-lookup"><span data-stu-id="94ad1-119">owner</span></span>    | [<span data-ttu-id="94ad1-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="94ad1-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="94ad1-121">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="94ad1-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="94ad1-122">Relações</span><span class="sxs-lookup"><span data-stu-id="94ad1-122">Relationships</span></span>

| <span data-ttu-id="94ad1-123">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="94ad1-123">Relationship name</span></span> | <span data-ttu-id="94ad1-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="94ad1-124">Type</span></span>                | <span data-ttu-id="94ad1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="94ad1-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="94ad1-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="94ad1-126">**driveItem**</span></span>     | <span data-ttu-id="94ad1-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="94ad1-127">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="94ad1-128">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="94ad1-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="94ad1-129">**list**</span><span class="sxs-lookup"><span data-stu-id="94ad1-129">**list**</span></span>          | <span data-ttu-id="94ad1-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="94ad1-130">[**list**][list]</span></span>        | <span data-ttu-id="94ad1-131">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="94ad1-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="94ad1-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="94ad1-132">**listItem**</span></span>      | <span data-ttu-id="94ad1-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="94ad1-133">[**listItem**][listItem]</span></span>    | <span data-ttu-id="94ad1-134">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="94ad1-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="94ad1-135">**site**</span><span class="sxs-lookup"><span data-stu-id="94ad1-135">**site**</span></span>          | <span data-ttu-id="94ad1-136">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="94ad1-136">[**site**][site]</span></span>        | <span data-ttu-id="94ad1-137">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="94ad1-137">Used to access the underlying **site**</span></span>

<span data-ttu-id="94ad1-138">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="94ad1-138">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="94ad1-139">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="94ad1-139">Relationship name</span></span> | <span data-ttu-id="94ad1-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="94ad1-140">Type</span></span>                         | <span data-ttu-id="94ad1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="94ad1-141">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="94ad1-142">**items**</span><span class="sxs-lookup"><span data-stu-id="94ad1-142">**items**</span></span>         | <span data-ttu-id="94ad1-143">coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="94ad1-143">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="94ad1-144">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="94ad1-144">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="94ad1-145">Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="94ad1-145">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="94ad1-146">**root**</span><span class="sxs-lookup"><span data-stu-id="94ad1-146">**root**</span></span>          | <span data-ttu-id="94ad1-147">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="94ad1-147">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="94ad1-148">Usado para acessar o **driveItem**subjacente.</span><span class="sxs-lookup"><span data-stu-id="94ad1-148">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="94ad1-149">Preterido-- `driveItem` use em vez disso.</span><span class="sxs-lookup"><span data-stu-id="94ad1-149">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="94ad1-150">Métodos</span><span class="sxs-lookup"><span data-stu-id="94ad1-150">Methods</span></span>

| <span data-ttu-id="94ad1-151">Método</span><span class="sxs-lookup"><span data-stu-id="94ad1-151">Method</span></span>                                  | <span data-ttu-id="94ad1-152">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="94ad1-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="94ad1-153">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="94ad1-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="94ad1-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="94ad1-154">Remarks</span></span>

<span data-ttu-id="94ad1-155">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="94ad1-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
