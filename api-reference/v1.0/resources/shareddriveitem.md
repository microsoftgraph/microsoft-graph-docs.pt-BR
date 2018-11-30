---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 32317a9bd2a75e8edde7967ef939c7a1a4b316fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006367"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="f38f3-102">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="f38f3-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="f38f3-103">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f38f3-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f38f3-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f38f3-104">JSON representation</span></span>

<span data-ttu-id="f38f3-105">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="f38f3-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="f38f3-106">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="f38f3-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f38f3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f38f3-107">Properties</span></span>

| <span data-ttu-id="f38f3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f38f3-108">Property</span></span> | <span data-ttu-id="f38f3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38f3-109">Type</span></span>                          | <span data-ttu-id="f38f3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38f3-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="f38f3-111">id</span><span class="sxs-lookup"><span data-stu-id="f38f3-111">id</span></span>       | <span data-ttu-id="f38f3-112">String</span><span class="sxs-lookup"><span data-stu-id="f38f3-112">String</span></span>                        | <span data-ttu-id="f38f3-113">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="f38f3-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="f38f3-114">name</span><span class="sxs-lookup"><span data-stu-id="f38f3-114">name</span></span>     | <span data-ttu-id="f38f3-115">String</span><span class="sxs-lookup"><span data-stu-id="f38f3-115">String</span></span>                        | <span data-ttu-id="f38f3-116">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f38f3-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="f38f3-117">owner</span><span class="sxs-lookup"><span data-stu-id="f38f3-117">owner</span></span>    | [<span data-ttu-id="f38f3-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f38f3-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="f38f3-119">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="f38f3-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f38f3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f38f3-120">Relationships</span></span>

| <span data-ttu-id="f38f3-121">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="f38f3-121">Relationship name</span></span> | <span data-ttu-id="f38f3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38f3-122">Type</span></span>                | <span data-ttu-id="f38f3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38f3-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="f38f3-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f38f3-124">**driveItem**</span></span>     | <span data-ttu-id="f38f3-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f38f3-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="f38f3-126">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="f38f3-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="f38f3-127">**list**</span><span class="sxs-lookup"><span data-stu-id="f38f3-127">**list**</span></span>          | <span data-ttu-id="f38f3-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="f38f3-128">[**list**][list]</span></span>        | <span data-ttu-id="f38f3-129">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="f38f3-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="f38f3-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="f38f3-130">**listItem**</span></span>      | <span data-ttu-id="f38f3-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="f38f3-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="f38f3-132">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="f38f3-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="f38f3-133">**site**</span><span class="sxs-lookup"><span data-stu-id="f38f3-133">**site**</span></span>          | <span data-ttu-id="f38f3-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="f38f3-134">[**site**][site]</span></span>        | <span data-ttu-id="f38f3-135">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="f38f3-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="f38f3-136">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="f38f3-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="f38f3-137">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="f38f3-137">Relationship name</span></span> | <span data-ttu-id="f38f3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38f3-138">Type</span></span>                         | <span data-ttu-id="f38f3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38f3-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="f38f3-140">**items**</span><span class="sxs-lookup"><span data-stu-id="f38f3-140">**items**</span></span>         | <span data-ttu-id="f38f3-141">Coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f38f3-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="f38f3-142">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f38f3-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="f38f3-143">Não é possível enumerar esta coleção.</span><span class="sxs-lookup"><span data-stu-id="f38f3-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f38f3-144">**root**</span><span class="sxs-lookup"><span data-stu-id="f38f3-144">**root**</span></span>          | <span data-ttu-id="f38f3-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f38f3-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="f38f3-146">Usado para acessar o subjacente **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="f38f3-146">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="f38f3-147">Preterido – use `driveItem` em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f38f3-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="f38f3-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="f38f3-148">Methods</span></span>

| <span data-ttu-id="f38f3-149">Método</span><span class="sxs-lookup"><span data-stu-id="f38f3-149">Method</span></span>                                  | <span data-ttu-id="f38f3-150">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="f38f3-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="f38f3-151">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="f38f3-151">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="f38f3-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="f38f3-152">Remarks</span></span>

<span data-ttu-id="f38f3-153">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f38f3-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
