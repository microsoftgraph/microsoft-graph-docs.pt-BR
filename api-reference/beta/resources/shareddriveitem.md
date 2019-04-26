---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 3c0fa155088e39d69d52d4b14f33662d92666ed6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343189"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="78e8a-102">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="78e8a-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78e8a-103">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="78e8a-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="78e8a-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78e8a-104">JSON representation</span></span>

<span data-ttu-id="78e8a-105">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="78e8a-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="78e8a-106">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="78e8a-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="78e8a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78e8a-107">Properties</span></span>

| <span data-ttu-id="78e8a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78e8a-108">Property</span></span> | <span data-ttu-id="78e8a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="78e8a-109">Type</span></span>                          | <span data-ttu-id="78e8a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e8a-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="78e8a-111">id</span><span class="sxs-lookup"><span data-stu-id="78e8a-111">id</span></span>       | <span data-ttu-id="78e8a-112">String</span><span class="sxs-lookup"><span data-stu-id="78e8a-112">String</span></span>                        | <span data-ttu-id="78e8a-113">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="78e8a-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="78e8a-114">name</span><span class="sxs-lookup"><span data-stu-id="78e8a-114">name</span></span>     | <span data-ttu-id="78e8a-115">String</span><span class="sxs-lookup"><span data-stu-id="78e8a-115">String</span></span>                        | <span data-ttu-id="78e8a-116">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="78e8a-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="78e8a-117">owner</span><span class="sxs-lookup"><span data-stu-id="78e8a-117">owner</span></span>    | [<span data-ttu-id="78e8a-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="78e8a-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="78e8a-119">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="78e8a-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="78e8a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="78e8a-120">Relationships</span></span>

| <span data-ttu-id="78e8a-121">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="78e8a-121">Relationship name</span></span> | <span data-ttu-id="78e8a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="78e8a-122">Type</span></span>                | <span data-ttu-id="78e8a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e8a-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="78e8a-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="78e8a-124">**driveItem**</span></span>     | <span data-ttu-id="78e8a-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="78e8a-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="78e8a-126">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="78e8a-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="78e8a-127">**list**</span><span class="sxs-lookup"><span data-stu-id="78e8a-127">**list**</span></span>          | <span data-ttu-id="78e8a-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="78e8a-128">[**list**][list]</span></span>           | <span data-ttu-id="78e8a-129">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="78e8a-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="78e8a-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="78e8a-130">**listItem**</span></span>      | <span data-ttu-id="78e8a-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="78e8a-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="78e8a-132">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="78e8a-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="78e8a-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="78e8a-133">**permission**</span></span>    | <span data-ttu-id="78e8a-134">[**autorização**][permission]</span><span class="sxs-lookup"><span data-stu-id="78e8a-134">[**permission**][permission]</span></span> | <span data-ttu-id="78e8a-135">Usado para acessar a **permissão** que representa o link de compartilhamento subjacente</span><span class="sxs-lookup"><span data-stu-id="78e8a-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="78e8a-136">**site**</span><span class="sxs-lookup"><span data-stu-id="78e8a-136">**site**</span></span>          | <span data-ttu-id="78e8a-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="78e8a-137">[**site**][site]</span></span>           | <span data-ttu-id="78e8a-138">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="78e8a-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="78e8a-139">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="78e8a-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="78e8a-140">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="78e8a-140">Relationship name</span></span> | <span data-ttu-id="78e8a-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="78e8a-141">Type</span></span>                         | <span data-ttu-id="78e8a-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e8a-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="78e8a-143">**items**</span><span class="sxs-lookup"><span data-stu-id="78e8a-143">**items**</span></span>         | <span data-ttu-id="78e8a-144">Coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="78e8a-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="78e8a-145">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="78e8a-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="78e8a-146">Não é possível enumerar esta coleção.</span><span class="sxs-lookup"><span data-stu-id="78e8a-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="78e8a-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="78e8a-147">**driveItem**</span></span>     | <span data-ttu-id="78e8a-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="78e8a-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="78e8a-149">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="78e8a-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="78e8a-150">Métodos</span><span class="sxs-lookup"><span data-stu-id="78e8a-150">Methods</span></span>

| <span data-ttu-id="78e8a-151">Método</span><span class="sxs-lookup"><span data-stu-id="78e8a-151">Method</span></span>                                  | <span data-ttu-id="78e8a-152">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="78e8a-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="78e8a-153">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="78e8a-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="78e8a-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="78e8a-154">Remarks</span></span>

<span data-ttu-id="78e8a-155">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="78e8a-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": []
}
-->
