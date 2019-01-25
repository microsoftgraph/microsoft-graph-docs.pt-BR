---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 22e449d725b94b7be458261e82cfde0b5d6fdf9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524118"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="fe001-102">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="fe001-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe001-103">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="fe001-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe001-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe001-104">JSON representation</span></span>

<span data-ttu-id="fe001-105">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="fe001-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="fe001-106">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="fe001-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fe001-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe001-107">Properties</span></span>

| <span data-ttu-id="fe001-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe001-108">Property</span></span> | <span data-ttu-id="fe001-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe001-109">Type</span></span>                          | <span data-ttu-id="fe001-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe001-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="fe001-111">id</span><span class="sxs-lookup"><span data-stu-id="fe001-111">id</span></span>       | <span data-ttu-id="fe001-112">String</span><span class="sxs-lookup"><span data-stu-id="fe001-112">String</span></span>                        | <span data-ttu-id="fe001-113">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="fe001-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="fe001-114">name</span><span class="sxs-lookup"><span data-stu-id="fe001-114">name</span></span>     | <span data-ttu-id="fe001-115">String</span><span class="sxs-lookup"><span data-stu-id="fe001-115">String</span></span>                        | <span data-ttu-id="fe001-116">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="fe001-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="fe001-117">owner</span><span class="sxs-lookup"><span data-stu-id="fe001-117">owner</span></span>    | [<span data-ttu-id="fe001-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fe001-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="fe001-119">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="fe001-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fe001-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fe001-120">Relationships</span></span>

| <span data-ttu-id="fe001-121">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="fe001-121">Relationship name</span></span> | <span data-ttu-id="fe001-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe001-122">Type</span></span>                | <span data-ttu-id="fe001-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe001-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="fe001-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="fe001-124">**driveItem**</span></span>     | <span data-ttu-id="fe001-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="fe001-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="fe001-126">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="fe001-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="fe001-127">**list**</span><span class="sxs-lookup"><span data-stu-id="fe001-127">**list**</span></span>          | <span data-ttu-id="fe001-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="fe001-128">[**list**][list]</span></span>           | <span data-ttu-id="fe001-129">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="fe001-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="fe001-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="fe001-130">**listItem**</span></span>      | <span data-ttu-id="fe001-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="fe001-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="fe001-132">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="fe001-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="fe001-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="fe001-133">**permission**</span></span>    | <span data-ttu-id="fe001-134">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="fe001-134">[**permission**][permission]</span></span> | <span data-ttu-id="fe001-135">Usado para acessar a **permissão** que representa o link subjacente de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="fe001-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="fe001-136">**site**</span><span class="sxs-lookup"><span data-stu-id="fe001-136">**site**</span></span>          | <span data-ttu-id="fe001-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="fe001-137">[**site**][site]</span></span>           | <span data-ttu-id="fe001-138">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="fe001-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="fe001-139">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="fe001-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="fe001-140">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="fe001-140">Relationship name</span></span> | <span data-ttu-id="fe001-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe001-141">Type</span></span>                         | <span data-ttu-id="fe001-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe001-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="fe001-143">**items**</span><span class="sxs-lookup"><span data-stu-id="fe001-143">**items**</span></span>         | <span data-ttu-id="fe001-144">Coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="fe001-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="fe001-145">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="fe001-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="fe001-146">Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="fe001-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="fe001-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="fe001-147">**driveItem**</span></span>     | <span data-ttu-id="fe001-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="fe001-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="fe001-149">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="fe001-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="fe001-150">Métodos</span><span class="sxs-lookup"><span data-stu-id="fe001-150">Methods</span></span>

| <span data-ttu-id="fe001-151">Método</span><span class="sxs-lookup"><span data-stu-id="fe001-151">Method</span></span>                                  | <span data-ttu-id="fe001-152">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="fe001-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="fe001-153">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="fe001-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="fe001-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="fe001-154">Remarks</span></span>

<span data-ttu-id="fe001-155">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fe001-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
