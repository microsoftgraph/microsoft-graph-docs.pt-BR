---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: b146fdf0f7ee2e2037fcb1d36511d0afa503005b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480625"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="d755c-102">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="d755c-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d755c-103">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d755c-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d755c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d755c-104">JSON representation</span></span>

<span data-ttu-id="d755c-105">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="d755c-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="d755c-106">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="d755c-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d755c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d755c-107">Properties</span></span>

| <span data-ttu-id="d755c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d755c-108">Property</span></span> | <span data-ttu-id="d755c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d755c-109">Type</span></span>                          | <span data-ttu-id="d755c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d755c-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="d755c-111">id</span><span class="sxs-lookup"><span data-stu-id="d755c-111">id</span></span>       | <span data-ttu-id="d755c-112">String</span><span class="sxs-lookup"><span data-stu-id="d755c-112">String</span></span>                        | <span data-ttu-id="d755c-113">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="d755c-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="d755c-114">name</span><span class="sxs-lookup"><span data-stu-id="d755c-114">name</span></span>     | <span data-ttu-id="d755c-115">String</span><span class="sxs-lookup"><span data-stu-id="d755c-115">String</span></span>                        | <span data-ttu-id="d755c-116">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d755c-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="d755c-117">owner</span><span class="sxs-lookup"><span data-stu-id="d755c-117">owner</span></span>    | [<span data-ttu-id="d755c-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d755c-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="d755c-119">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="d755c-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d755c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d755c-120">Relationships</span></span>

| <span data-ttu-id="d755c-121">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="d755c-121">Relationship name</span></span> | <span data-ttu-id="d755c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d755c-122">Type</span></span>                | <span data-ttu-id="d755c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d755c-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="d755c-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d755c-124">**driveItem**</span></span>     | <span data-ttu-id="d755c-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d755c-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="d755c-126">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="d755c-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="d755c-127">**list**</span><span class="sxs-lookup"><span data-stu-id="d755c-127">**list**</span></span>          | <span data-ttu-id="d755c-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="d755c-128">[**list**][list]</span></span>           | <span data-ttu-id="d755c-129">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="d755c-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="d755c-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="d755c-130">**listItem**</span></span>      | <span data-ttu-id="d755c-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="d755c-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="d755c-132">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="d755c-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="d755c-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="d755c-133">**permission**</span></span>    | <span data-ttu-id="d755c-134">[**autorização**][permission]</span><span class="sxs-lookup"><span data-stu-id="d755c-134">[**permission**][permission]</span></span> | <span data-ttu-id="d755c-135">Usado para acessar a **permissão** que representa o link de compartilhamento subjacente</span><span class="sxs-lookup"><span data-stu-id="d755c-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="d755c-136">**site**</span><span class="sxs-lookup"><span data-stu-id="d755c-136">**site**</span></span>          | <span data-ttu-id="d755c-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="d755c-137">[**site**][site]</span></span>           | <span data-ttu-id="d755c-138">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="d755c-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="d755c-139">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="d755c-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="d755c-140">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="d755c-140">Relationship name</span></span> | <span data-ttu-id="d755c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="d755c-141">Type</span></span>                         | <span data-ttu-id="d755c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="d755c-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="d755c-143">**items**</span><span class="sxs-lookup"><span data-stu-id="d755c-143">**items**</span></span>         | <span data-ttu-id="d755c-144">Coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d755c-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="d755c-145">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="d755c-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="d755c-146">Não é possível enumerar esta coleção.</span><span class="sxs-lookup"><span data-stu-id="d755c-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="d755c-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d755c-147">**driveItem**</span></span>     | <span data-ttu-id="d755c-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d755c-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="d755c-149">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="d755c-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="d755c-150">Métodos</span><span class="sxs-lookup"><span data-stu-id="d755c-150">Methods</span></span>

| <span data-ttu-id="d755c-151">Método</span><span class="sxs-lookup"><span data-stu-id="d755c-151">Method</span></span>                                  | <span data-ttu-id="d755c-152">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="d755c-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="d755c-153">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="d755c-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="d755c-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="d755c-154">Remarks</span></span>

<span data-ttu-id="d755c-155">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d755c-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareddriveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
