---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: baee7eebd3abcaa8376440fb0b20cbe5c69df880
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035053"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="692ec-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="692ec-104">profilePhoto resource type</span></span>
<span data-ttu-id="692ec-p102">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="692ec-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="692ec-107">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="692ec-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="692ec-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="692ec-108">Methods</span></span>

| <span data-ttu-id="692ec-109">Método</span><span class="sxs-lookup"><span data-stu-id="692ec-109">Method</span></span>       | <span data-ttu-id="692ec-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="692ec-110">Return Type</span></span>  |<span data-ttu-id="692ec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="692ec-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="692ec-112">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="692ec-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="692ec-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="692ec-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="692ec-114">Obtenha a **profilePhoto** especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="692ec-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="692ec-115">Update</span><span class="sxs-lookup"><span data-stu-id="692ec-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="692ec-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="692ec-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="692ec-p103">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="692ec-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="692ec-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="692ec-120">Properties</span></span>
| <span data-ttu-id="692ec-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="692ec-121">Property</span></span>     | <span data-ttu-id="692ec-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="692ec-122">Type</span></span>   |<span data-ttu-id="692ec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="692ec-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="692ec-124">id</span><span class="sxs-lookup"><span data-stu-id="692ec-124">id</span></span>|<span data-ttu-id="692ec-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="692ec-125">string</span></span>|<span data-ttu-id="692ec-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="692ec-126">Read-only.</span></span>|
|<span data-ttu-id="692ec-127">height</span><span class="sxs-lookup"><span data-stu-id="692ec-127">height</span></span>|<span data-ttu-id="692ec-128">int32</span><span class="sxs-lookup"><span data-stu-id="692ec-128">int32</span></span>|<span data-ttu-id="692ec-p104">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="692ec-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="692ec-131">width</span><span class="sxs-lookup"><span data-stu-id="692ec-131">width</span></span>|<span data-ttu-id="692ec-132">int32</span><span class="sxs-lookup"><span data-stu-id="692ec-132">int32</span></span>|<span data-ttu-id="692ec-p105">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="692ec-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="692ec-135">Relações</span><span class="sxs-lookup"><span data-stu-id="692ec-135">Relationships</span></span>
<span data-ttu-id="692ec-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="692ec-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="692ec-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="692ec-137">JSON representation</span></span>

<span data-ttu-id="692ec-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="692ec-138">Here is a JSON representation of the resource.</span></span>

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
