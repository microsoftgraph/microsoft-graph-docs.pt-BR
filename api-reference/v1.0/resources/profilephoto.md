---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.
ms.openlocfilehash: c5f74e1dcd48e42a2e17d5a64e6ed4b9e9cca5e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007415"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="7f55e-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7f55e-104">profilePhoto resource type</span></span>
<span data-ttu-id="7f55e-p102">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="7f55e-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="7f55e-107">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="7f55e-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="7f55e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f55e-108">Methods</span></span>

| <span data-ttu-id="7f55e-109">Método</span><span class="sxs-lookup"><span data-stu-id="7f55e-109">Method</span></span>       | <span data-ttu-id="7f55e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f55e-110">Return Type</span></span>  |<span data-ttu-id="7f55e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f55e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f55e-112">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7f55e-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="7f55e-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7f55e-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="7f55e-114">Obtenha a **profilePhoto** especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="7f55e-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="7f55e-115">Update</span><span class="sxs-lookup"><span data-stu-id="7f55e-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="7f55e-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7f55e-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="7f55e-p103">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="7f55e-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f55e-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f55e-120">Properties</span></span>
| <span data-ttu-id="7f55e-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f55e-121">Property</span></span>     | <span data-ttu-id="7f55e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f55e-122">Type</span></span>   |<span data-ttu-id="7f55e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f55e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f55e-124">id</span><span class="sxs-lookup"><span data-stu-id="7f55e-124">id</span></span>|<span data-ttu-id="7f55e-125">string</span><span class="sxs-lookup"><span data-stu-id="7f55e-125">string</span></span>|<span data-ttu-id="7f55e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f55e-126">Read-only.</span></span>|
|<span data-ttu-id="7f55e-127">height</span><span class="sxs-lookup"><span data-stu-id="7f55e-127">height</span></span>|<span data-ttu-id="7f55e-128">int32</span><span class="sxs-lookup"><span data-stu-id="7f55e-128">int32</span></span>|<span data-ttu-id="7f55e-p104">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f55e-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="7f55e-131">width</span><span class="sxs-lookup"><span data-stu-id="7f55e-131">width</span></span>|<span data-ttu-id="7f55e-132">int32</span><span class="sxs-lookup"><span data-stu-id="7f55e-132">int32</span></span>|<span data-ttu-id="7f55e-p105">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f55e-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f55e-135">Relações</span><span class="sxs-lookup"><span data-stu-id="7f55e-135">Relationships</span></span>
<span data-ttu-id="7f55e-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f55e-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7f55e-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f55e-137">JSON representation</span></span>

<span data-ttu-id="7f55e-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f55e-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
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
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
