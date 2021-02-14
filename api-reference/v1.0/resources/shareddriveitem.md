---
author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b00703b1fea7689eae942ffb790e8d65672b89b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238873"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="b29a5-103">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="b29a5-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="b29a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b29a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b29a5-105">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b29a5-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b29a5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b29a5-106">JSON representation</span></span>

<span data-ttu-id="b29a5-107">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="b29a5-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="b29a5-108">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="b29a5-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b29a5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b29a5-109">Properties</span></span>

| <span data-ttu-id="b29a5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b29a5-110">Property</span></span> | <span data-ttu-id="b29a5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b29a5-111">Type</span></span>                          | <span data-ttu-id="b29a5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b29a5-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="b29a5-113">id</span><span class="sxs-lookup"><span data-stu-id="b29a5-113">id</span></span>       | <span data-ttu-id="b29a5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b29a5-114">String</span></span>                        | <span data-ttu-id="b29a5-115">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="b29a5-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="b29a5-116">name</span><span class="sxs-lookup"><span data-stu-id="b29a5-116">name</span></span>     | <span data-ttu-id="b29a5-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b29a5-117">String</span></span>                        | <span data-ttu-id="b29a5-118">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b29a5-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="b29a5-119">owner</span><span class="sxs-lookup"><span data-stu-id="b29a5-119">owner</span></span>    | [<span data-ttu-id="b29a5-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b29a5-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="b29a5-121">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="b29a5-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b29a5-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b29a5-122">Relationships</span></span>

| <span data-ttu-id="b29a5-123">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b29a5-123">Relationship name</span></span> | <span data-ttu-id="b29a5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b29a5-124">Type</span></span>                | <span data-ttu-id="b29a5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b29a5-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="b29a5-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="b29a5-126">**driveItem**</span></span>     | <span data-ttu-id="b29a5-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="b29a5-127">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="b29a5-128">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="b29a5-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="b29a5-129">**list**</span><span class="sxs-lookup"><span data-stu-id="b29a5-129">**list**</span></span>          | <span data-ttu-id="b29a5-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="b29a5-130">[**list**][list]</span></span>        | <span data-ttu-id="b29a5-131">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="b29a5-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="b29a5-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="b29a5-132">**listItem**</span></span>      | <span data-ttu-id="b29a5-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="b29a5-133">[**listItem**][listItem]</span></span>    | <span data-ttu-id="b29a5-134">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="b29a5-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="b29a5-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="b29a5-135">**permission**</span></span>    | <span data-ttu-id="b29a5-136">[**permission**][permission]</span><span class="sxs-lookup"><span data-stu-id="b29a5-136">[**permission**][permission]</span></span> | <span data-ttu-id="b29a5-137">Usado para acessar a permissão **que** representa o link de compartilhamento subjacente</span><span class="sxs-lookup"><span data-stu-id="b29a5-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="b29a5-138">**site**</span><span class="sxs-lookup"><span data-stu-id="b29a5-138">**site**</span></span>          | <span data-ttu-id="b29a5-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="b29a5-139">[**site**][site]</span></span>        | <span data-ttu-id="b29a5-140">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="b29a5-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="b29a5-141">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="b29a5-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="b29a5-142">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b29a5-142">Relationship name</span></span> | <span data-ttu-id="b29a5-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="b29a5-143">Type</span></span>                         | <span data-ttu-id="b29a5-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="b29a5-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="b29a5-145">**items**</span><span class="sxs-lookup"><span data-stu-id="b29a5-145">**items**</span></span>         | <span data-ttu-id="b29a5-146">[**Coleção driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="b29a5-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="b29a5-147">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="b29a5-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="b29a5-148">Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="b29a5-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="b29a5-149">**root**</span><span class="sxs-lookup"><span data-stu-id="b29a5-149">**root**</span></span>          | <span data-ttu-id="b29a5-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="b29a5-150">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="b29a5-151">Usado para acessar o **driveItem subjacente.**</span><span class="sxs-lookup"><span data-stu-id="b29a5-151">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="b29a5-152">Preterido – use `driveItem` em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b29a5-152">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="b29a5-153">Métodos</span><span class="sxs-lookup"><span data-stu-id="b29a5-153">Methods</span></span>

| <span data-ttu-id="b29a5-154">Método</span><span class="sxs-lookup"><span data-stu-id="b29a5-154">Method</span></span>                                  | <span data-ttu-id="b29a5-155">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="b29a5-155">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="b29a5-156">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="b29a5-156">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="b29a5-157">Comentários</span><span class="sxs-lookup"><span data-stu-id="b29a5-157">Remarks</span></span>

<span data-ttu-id="b29a5-158">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b29a5-158">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

