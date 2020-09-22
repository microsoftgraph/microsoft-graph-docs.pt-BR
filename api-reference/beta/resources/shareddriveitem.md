---
author: JeremyKelley
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a2e1252437608d474e92346ed0aaba4a3a50053d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060024"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="f4864-103">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="f4864-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="f4864-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4864-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4864-105">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f4864-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4864-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4864-106">JSON representation</span></span>

<span data-ttu-id="f4864-107">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="f4864-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="f4864-108">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="f4864-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4864-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4864-109">Properties</span></span>

| <span data-ttu-id="f4864-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4864-110">Property</span></span> | <span data-ttu-id="f4864-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4864-111">Type</span></span>                          | <span data-ttu-id="f4864-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4864-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="f4864-113">id</span><span class="sxs-lookup"><span data-stu-id="f4864-113">id</span></span>       | <span data-ttu-id="f4864-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4864-114">String</span></span>                        | <span data-ttu-id="f4864-115">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="f4864-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="f4864-116">name</span><span class="sxs-lookup"><span data-stu-id="f4864-116">name</span></span>     | <span data-ttu-id="f4864-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4864-117">String</span></span>                        | <span data-ttu-id="f4864-118">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f4864-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="f4864-119">owner</span><span class="sxs-lookup"><span data-stu-id="f4864-119">owner</span></span>    | [<span data-ttu-id="f4864-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f4864-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="f4864-121">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="f4864-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4864-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f4864-122">Relationships</span></span>

| <span data-ttu-id="f4864-123">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="f4864-123">Relationship name</span></span> | <span data-ttu-id="f4864-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4864-124">Type</span></span>                | <span data-ttu-id="f4864-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4864-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="f4864-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4864-126">**driveItem**</span></span>     | <span data-ttu-id="f4864-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4864-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="f4864-128">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="f4864-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="f4864-129">**list**</span><span class="sxs-lookup"><span data-stu-id="f4864-129">**list**</span></span>          | <span data-ttu-id="f4864-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="f4864-130">[**list**][list]</span></span>           | <span data-ttu-id="f4864-131">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="f4864-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="f4864-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="f4864-132">**listItem**</span></span>      | <span data-ttu-id="f4864-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="f4864-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="f4864-134">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="f4864-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="f4864-135">**permissão**</span><span class="sxs-lookup"><span data-stu-id="f4864-135">**permission**</span></span>    | <span data-ttu-id="f4864-136">[**autorização**][permission]</span><span class="sxs-lookup"><span data-stu-id="f4864-136">[**permission**][permission]</span></span> | <span data-ttu-id="f4864-137">Usado para acessar a **permissão** que representa o link de compartilhamento subjacente</span><span class="sxs-lookup"><span data-stu-id="f4864-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="f4864-138">**site**</span><span class="sxs-lookup"><span data-stu-id="f4864-138">**site**</span></span>          | <span data-ttu-id="f4864-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="f4864-139">[**site**][site]</span></span>           | <span data-ttu-id="f4864-140">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="f4864-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="f4864-141">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="f4864-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="f4864-142">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="f4864-142">Relationship name</span></span> | <span data-ttu-id="f4864-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4864-143">Type</span></span>                         | <span data-ttu-id="f4864-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4864-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="f4864-145">**items**</span><span class="sxs-lookup"><span data-stu-id="f4864-145">**items**</span></span>         | <span data-ttu-id="f4864-146">coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4864-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="f4864-147">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f4864-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="f4864-148">Não é possível enumerar esta coleção.</span><span class="sxs-lookup"><span data-stu-id="f4864-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f4864-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4864-149">**driveItem**</span></span>     | <span data-ttu-id="f4864-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4864-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="f4864-151">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="f4864-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="f4864-152">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4864-152">Methods</span></span>

| <span data-ttu-id="f4864-153">Método</span><span class="sxs-lookup"><span data-stu-id="f4864-153">Method</span></span>                                  | <span data-ttu-id="f4864-154">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="f4864-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="f4864-155">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="f4864-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="f4864-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="f4864-156">Remarks</span></span>

<span data-ttu-id="f4864-157">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f4864-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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


