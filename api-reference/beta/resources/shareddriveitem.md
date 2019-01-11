---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: d20656351725f23d4fd4c00b65fdc88fe2f449b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853064"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="d6ae2-102">Tipo de recurso SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="d6ae2-102">SharedDriveItem resource type</span></span>

> <span data-ttu-id="d6ae2-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6ae2-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6ae2-105">O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6ae2-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6ae2-106">JSON representation</span></span>

<span data-ttu-id="d6ae2-107">Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="d6ae2-108">O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d6ae2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6ae2-109">Properties</span></span>

| <span data-ttu-id="d6ae2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6ae2-110">Property</span></span> | <span data-ttu-id="d6ae2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ae2-111">Type</span></span>                          | <span data-ttu-id="d6ae2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ae2-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="d6ae2-113">id</span><span class="sxs-lookup"><span data-stu-id="d6ae2-113">id</span></span>       | <span data-ttu-id="d6ae2-114">String</span><span class="sxs-lookup"><span data-stu-id="d6ae2-114">String</span></span>                        | <span data-ttu-id="d6ae2-115">O identificador exclusivo do compartilhamento que está sendo acessado.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="d6ae2-116">name</span><span class="sxs-lookup"><span data-stu-id="d6ae2-116">name</span></span>     | <span data-ttu-id="d6ae2-117">String</span><span class="sxs-lookup"><span data-stu-id="d6ae2-117">String</span></span>                        | <span data-ttu-id="d6ae2-118">O nome de exibição do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="d6ae2-119">owner</span><span class="sxs-lookup"><span data-stu-id="d6ae2-119">owner</span></span>    | [<span data-ttu-id="d6ae2-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d6ae2-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="d6ae2-121">Informações sobre o proprietário do item compartilhado que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d6ae2-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d6ae2-122">Relationships</span></span>

| <span data-ttu-id="d6ae2-123">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="d6ae2-123">Relationship name</span></span> | <span data-ttu-id="d6ae2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ae2-124">Type</span></span>                | <span data-ttu-id="d6ae2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ae2-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="d6ae2-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-126">**driveItem**</span></span>     | <span data-ttu-id="d6ae2-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="d6ae2-128">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="d6ae2-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="d6ae2-129">**list**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-129">**list**</span></span>          | <span data-ttu-id="d6ae2-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-130">[**list**][list]</span></span>           | <span data-ttu-id="d6ae2-131">Usado para acessar a **lista** subjacente</span><span class="sxs-lookup"><span data-stu-id="d6ae2-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="d6ae2-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-132">**listItem**</span></span>      | <span data-ttu-id="d6ae2-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="d6ae2-134">Usado para acessar o **listItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="d6ae2-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="d6ae2-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-135">**permission**</span></span>    | <span data-ttu-id="d6ae2-136">[**permissão**][permission]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-136">[**permission**][permission]</span></span> | <span data-ttu-id="d6ae2-137">Usado para acessar a **permissão** que representa o link subjacente de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="d6ae2-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="d6ae2-138">**site**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-138">**site**</span></span>          | <span data-ttu-id="d6ae2-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-139">[**site**][site]</span></span>           | <span data-ttu-id="d6ae2-140">Usado para acessar o **site** subjacente</span><span class="sxs-lookup"><span data-stu-id="d6ae2-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="d6ae2-141">Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="d6ae2-142">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="d6ae2-142">Relationship name</span></span> | <span data-ttu-id="d6ae2-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ae2-143">Type</span></span>                         | <span data-ttu-id="d6ae2-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ae2-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="d6ae2-145">**items**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-145">**items**</span></span>         | <span data-ttu-id="d6ae2-146">Coleção [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="d6ae2-147">Todos os driveItems contidos na raiz de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="d6ae2-148">Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="d6ae2-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="d6ae2-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d6ae2-149">**driveItem**</span></span>     | <span data-ttu-id="d6ae2-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d6ae2-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="d6ae2-151">Usado para acessar o **driveItem** subjacente</span><span class="sxs-lookup"><span data-stu-id="d6ae2-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="d6ae2-152">Métodos</span><span class="sxs-lookup"><span data-stu-id="d6ae2-152">Methods</span></span>

| <span data-ttu-id="d6ae2-153">Método</span><span class="sxs-lookup"><span data-stu-id="d6ae2-153">Method</span></span>                                  | <span data-ttu-id="d6ae2-154">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="d6ae2-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="d6ae2-155">Obter item compartilhado</span><span class="sxs-lookup"><span data-stu-id="d6ae2-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="d6ae2-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6ae2-156">Remarks</span></span>

<span data-ttu-id="d6ae2-157">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d6ae2-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
