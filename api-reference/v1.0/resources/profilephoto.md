---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.
localization_priority: Priority
ms.openlocfilehash: b1901928a97356b2a9808a446d34981fd74bf456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876563"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="71f04-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="71f04-104">profilePhoto resource type</span></span>
<span data-ttu-id="71f04-p102">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="71f04-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="71f04-107">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="71f04-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="71f04-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="71f04-108">Methods</span></span>

| <span data-ttu-id="71f04-109">Método</span><span class="sxs-lookup"><span data-stu-id="71f04-109">Method</span></span>       | <span data-ttu-id="71f04-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71f04-110">Return Type</span></span>  |<span data-ttu-id="71f04-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71f04-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71f04-112">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="71f04-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="71f04-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="71f04-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="71f04-114">Obtenha a **profilePhoto** especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="71f04-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="71f04-115">Update</span><span class="sxs-lookup"><span data-stu-id="71f04-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="71f04-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="71f04-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="71f04-p103">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="71f04-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="71f04-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71f04-120">Properties</span></span>
| <span data-ttu-id="71f04-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71f04-121">Property</span></span>     | <span data-ttu-id="71f04-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="71f04-122">Type</span></span>   |<span data-ttu-id="71f04-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="71f04-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71f04-124">id</span><span class="sxs-lookup"><span data-stu-id="71f04-124">id</span></span>|<span data-ttu-id="71f04-125">string</span><span class="sxs-lookup"><span data-stu-id="71f04-125">string</span></span>|<span data-ttu-id="71f04-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71f04-126">Read-only.</span></span>|
|<span data-ttu-id="71f04-127">height</span><span class="sxs-lookup"><span data-stu-id="71f04-127">height</span></span>|<span data-ttu-id="71f04-128">int32</span><span class="sxs-lookup"><span data-stu-id="71f04-128">int32</span></span>|<span data-ttu-id="71f04-p104">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71f04-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="71f04-131">width</span><span class="sxs-lookup"><span data-stu-id="71f04-131">width</span></span>|<span data-ttu-id="71f04-132">int32</span><span class="sxs-lookup"><span data-stu-id="71f04-132">int32</span></span>|<span data-ttu-id="71f04-p105">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71f04-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71f04-135">Relações</span><span class="sxs-lookup"><span data-stu-id="71f04-135">Relationships</span></span>
<span data-ttu-id="71f04-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71f04-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="71f04-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71f04-137">JSON representation</span></span>

<span data-ttu-id="71f04-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71f04-138">Here is a JSON representation of the resource.</span></span>

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
