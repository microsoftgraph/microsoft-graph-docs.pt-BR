---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ef54be828c9094c76c215c66c79fd2c1453503dc
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757227"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="10a59-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="10a59-104">profilePhoto resource type</span></span>

<span data-ttu-id="10a59-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a59-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10a59-p102">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="10a59-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="10a59-108">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="10a59-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="10a59-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="10a59-109">Methods</span></span>

| <span data-ttu-id="10a59-110">Método</span><span class="sxs-lookup"><span data-stu-id="10a59-110">Method</span></span>       | <span data-ttu-id="10a59-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10a59-111">Return Type</span></span>  |<span data-ttu-id="10a59-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a59-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10a59-113">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="10a59-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="10a59-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="10a59-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="10a59-115">Obtenha a **profilePhoto** especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="10a59-115">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="10a59-116">Update</span><span class="sxs-lookup"><span data-stu-id="10a59-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="10a59-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="10a59-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="10a59-p103">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="10a59-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="10a59-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10a59-121">Properties</span></span>
| <span data-ttu-id="10a59-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10a59-122">Property</span></span>     | <span data-ttu-id="10a59-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="10a59-123">Type</span></span>   |<span data-ttu-id="10a59-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a59-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10a59-125">id</span><span class="sxs-lookup"><span data-stu-id="10a59-125">id</span></span>|<span data-ttu-id="10a59-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10a59-126">string</span></span>|<span data-ttu-id="10a59-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10a59-127">Read-only.</span></span>|
|<span data-ttu-id="10a59-128">height</span><span class="sxs-lookup"><span data-stu-id="10a59-128">height</span></span>|<span data-ttu-id="10a59-129">int32</span><span class="sxs-lookup"><span data-stu-id="10a59-129">int32</span></span>|<span data-ttu-id="10a59-p104">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10a59-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="10a59-132">width</span><span class="sxs-lookup"><span data-stu-id="10a59-132">width</span></span>|<span data-ttu-id="10a59-133">int32</span><span class="sxs-lookup"><span data-stu-id="10a59-133">int32</span></span>|<span data-ttu-id="10a59-p105">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10a59-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10a59-136">Relações</span><span class="sxs-lookup"><span data-stu-id="10a59-136">Relationships</span></span>
<span data-ttu-id="10a59-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10a59-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="10a59-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10a59-138">JSON representation</span></span>

<span data-ttu-id="10a59-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10a59-139">Here is a JSON representation of the resource.</span></span>

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
