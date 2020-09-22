---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD). Os dados binários não são codificados em base-64.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: a7f23f67c65f039d79057f26269c55e5b563c11c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029082"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="1ec20-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="1ec20-104">profilePhoto resource type</span></span>

<span data-ttu-id="1ec20-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ec20-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ec20-p102">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD). Os dados binários não são codificados em base-64.</span><span class="sxs-lookup"><span data-stu-id="1ec20-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD). It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="1ec20-108">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="1ec20-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="1ec20-109">No AAD, as fotos podem ser qualquer dimensão.</span><span class="sxs-lookup"><span data-stu-id="1ec20-109">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="1ec20-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="1ec20-110">Methods</span></span>

| <span data-ttu-id="1ec20-111">Método</span><span class="sxs-lookup"><span data-stu-id="1ec20-111">Method</span></span>       | <span data-ttu-id="1ec20-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ec20-112">Return Type</span></span>  |<span data-ttu-id="1ec20-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ec20-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ec20-114">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="1ec20-114">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="1ec20-115">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="1ec20-115">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="1ec20-116">Obtenha a **profilePhoto** específica ou seus metadados (propriedades **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="1ec20-116">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="1ec20-117">Update</span><span class="sxs-lookup"><span data-stu-id="1ec20-117">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="1ec20-118">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="1ec20-118">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="1ec20-p104">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="1ec20-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ec20-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ec20-122">Properties</span></span>
| <span data-ttu-id="1ec20-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ec20-123">Property</span></span>     | <span data-ttu-id="1ec20-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ec20-124">Type</span></span>   |<span data-ttu-id="1ec20-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ec20-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ec20-126">id</span><span class="sxs-lookup"><span data-stu-id="1ec20-126">id</span></span>|<span data-ttu-id="1ec20-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ec20-127">string</span></span>|<span data-ttu-id="1ec20-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ec20-128">Read-only.</span></span>|
|<span data-ttu-id="1ec20-129">height</span><span class="sxs-lookup"><span data-stu-id="1ec20-129">height</span></span>|<span data-ttu-id="1ec20-130">int32</span><span class="sxs-lookup"><span data-stu-id="1ec20-130">int32</span></span>|<span data-ttu-id="1ec20-p105">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ec20-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="1ec20-133">width</span><span class="sxs-lookup"><span data-stu-id="1ec20-133">width</span></span>|<span data-ttu-id="1ec20-134">int32</span><span class="sxs-lookup"><span data-stu-id="1ec20-134">int32</span></span>|<span data-ttu-id="1ec20-p106">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ec20-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ec20-137">Relações</span><span class="sxs-lookup"><span data-stu-id="1ec20-137">Relationships</span></span>
<span data-ttu-id="1ec20-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ec20-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1ec20-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ec20-139">JSON representation</span></span>

<span data-ttu-id="1ec20-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ec20-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


