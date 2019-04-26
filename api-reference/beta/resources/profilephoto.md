---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD). Seus dados binários não são codificados em base 64.
localization_priority: Normal
ms.openlocfilehash: edff2919192403b41096a6f9dfcd6dbdcf1446ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344061"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="305da-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="305da-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="305da-105">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="305da-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="305da-106">Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="305da-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="305da-107">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="305da-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="305da-108">No AAD, as fotos podem ser qualquer dimensão.</span><span class="sxs-lookup"><span data-stu-id="305da-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="305da-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="305da-109">Methods</span></span>

| <span data-ttu-id="305da-110">Método</span><span class="sxs-lookup"><span data-stu-id="305da-110">Method</span></span>       | <span data-ttu-id="305da-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="305da-111">Return Type</span></span>  |<span data-ttu-id="305da-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="305da-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="305da-113">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="305da-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="305da-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="305da-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="305da-115">Obtenha a **profilePhoto** específica ou seus metadados (propriedades **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="305da-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="305da-116">Update</span><span class="sxs-lookup"><span data-stu-id="305da-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="305da-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="305da-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="305da-p104">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="305da-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="305da-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="305da-121">Properties</span></span>
| <span data-ttu-id="305da-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="305da-122">Property</span></span>     | <span data-ttu-id="305da-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="305da-123">Type</span></span>   |<span data-ttu-id="305da-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="305da-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="305da-125">id</span><span class="sxs-lookup"><span data-stu-id="305da-125">id</span></span>|<span data-ttu-id="305da-126">string</span><span class="sxs-lookup"><span data-stu-id="305da-126">string</span></span>|<span data-ttu-id="305da-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="305da-127">Read-only.</span></span>|
|<span data-ttu-id="305da-128">height</span><span class="sxs-lookup"><span data-stu-id="305da-128">height</span></span>|<span data-ttu-id="305da-129">Int32</span><span class="sxs-lookup"><span data-stu-id="305da-129">int32</span></span>|<span data-ttu-id="305da-p105">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="305da-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="305da-132">width</span><span class="sxs-lookup"><span data-stu-id="305da-132">width</span></span>|<span data-ttu-id="305da-133">Int32</span><span class="sxs-lookup"><span data-stu-id="305da-133">int32</span></span>|<span data-ttu-id="305da-p106">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="305da-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="305da-136">Relações</span><span class="sxs-lookup"><span data-stu-id="305da-136">Relationships</span></span>
<span data-ttu-id="305da-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="305da-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="305da-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="305da-138">JSON representation</span></span>

<span data-ttu-id="305da-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="305da-139">Here is a JSON representation of the resource.</span></span>

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
