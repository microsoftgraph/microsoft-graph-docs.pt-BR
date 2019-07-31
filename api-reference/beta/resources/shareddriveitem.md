---
author: JeremyKelley
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7d5af60c4ba5c67046909f6998d298444fa06d51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965156"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="38c51-103">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="38c51-103">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38c51-104">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="38c51-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="38c51-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38c51-105">JSON representation</span></span>

<span data-ttu-id="38c51-106">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="38c51-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="38c51-107">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="38c51-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="38c51-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38c51-108">Properties</span></span>

| <span data-ttu-id="38c51-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38c51-109">Property</span></span> | <span data-ttu-id="38c51-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="38c51-110">Type</span></span>                          | <span data-ttu-id="38c51-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="38c51-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="38c51-112">id</span><span class="sxs-lookup"><span data-stu-id="38c51-112">id</span></span>       | <span data-ttu-id="38c51-113">String</span><span class="sxs-lookup"><span data-stu-id="38c51-113">String</span></span>                        | <span data-ttu-id="38c51-114">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="38c51-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="38c51-115">name</span><span class="sxs-lookup"><span data-stu-id="38c51-115">name</span></span>     | <span data-ttu-id="38c51-116">String</span><span class="sxs-lookup"><span data-stu-id="38c51-116">String</span></span>                        | <span data-ttu-id="38c51-117">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="38c51-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="38c51-118">owner</span><span class="sxs-lookup"><span data-stu-id="38c51-118">owner</span></span>    | [<span data-ttu-id="38c51-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="38c51-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="38c51-120">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="38c51-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="38c51-121">Relações</span><span class="sxs-lookup"><span data-stu-id="38c51-121">Relationships</span></span>

| <span data-ttu-id="38c51-122">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="38c51-122">Relationship name</span></span> | <span data-ttu-id="38c51-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="38c51-123">Type</span></span>                | <span data-ttu-id="38c51-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="38c51-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="38c51-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="38c51-125">**driveItem**</span></span>     | <span data-ttu-id="38c51-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="38c51-126">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="38c51-127">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="38c51-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="38c51-128">**list**</span><span class="sxs-lookup"><span data-stu-id="38c51-128">**list**</span></span>          | <span data-ttu-id="38c51-129">[**lista**][list]</span><span class="sxs-lookup"><span data-stu-id="38c51-129">[**list**][list]</span></span>           | <span data-ttu-id="38c51-130">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="38c51-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="38c51-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="38c51-131">**listItem**</span></span>      | <span data-ttu-id="38c51-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="38c51-132">[**listItem**][listItem]</span></span>   | <span data-ttu-id="38c51-133">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="38c51-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="38c51-134">**permissão**</span><span class="sxs-lookup"><span data-stu-id="38c51-134">**permission**</span></span>    | <span data-ttu-id="38c51-135">[**autorização**][permission]</span><span class="sxs-lookup"><span data-stu-id="38c51-135">[**permission**][permission]</span></span> | <span data-ttu-id="38c51-136">Usado para acessar a **permissão** que representa o link de compartilhamento subjacente</span><span class="sxs-lookup"><span data-stu-id="38c51-136">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="38c51-137">**site**</span><span class="sxs-lookup"><span data-stu-id="38c51-137">**site**</span></span>          | <span data-ttu-id="38c51-138">[**no**][site]</span><span class="sxs-lookup"><span data-stu-id="38c51-138">[**site**][site]</span></span>           | <span data-ttu-id="38c51-139">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="38c51-139">Used to access the underlying **site**</span></span>

<span data-ttu-id="38c51-140">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="38c51-140">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="38c51-141">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="38c51-141">Relationship name</span></span> | <span data-ttu-id="38c51-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="38c51-142">Type</span></span>                         | <span data-ttu-id="38c51-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="38c51-143">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="38c51-144">**items**</span><span class="sxs-lookup"><span data-stu-id="38c51-144">**items**</span></span>         | <span data-ttu-id="38c51-145">coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="38c51-145">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="38c51-146">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="38c51-146">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="38c51-147">Não é possível enumerar esta coleção.</span><span class="sxs-lookup"><span data-stu-id="38c51-147">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="38c51-148">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="38c51-148">**driveItem**</span></span>     | <span data-ttu-id="38c51-149">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="38c51-149">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="38c51-150">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="38c51-150">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="38c51-151">Métodos</span><span class="sxs-lookup"><span data-stu-id="38c51-151">Methods</span></span>

| <span data-ttu-id="38c51-152">Método</span><span class="sxs-lookup"><span data-stu-id="38c51-152">Method</span></span>                                  | <span data-ttu-id="38c51-153">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="38c51-153">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="38c51-154">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="38c51-154">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="38c51-155">Comentários</span><span class="sxs-lookup"><span data-stu-id="38c51-155">Remarks</span></span>

<span data-ttu-id="38c51-156">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="38c51-156">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
