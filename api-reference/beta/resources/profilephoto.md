---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD). Os dados binários não são codificados em base-64.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: dbaff3f61e7c430ae77ec10bea66a9c11dabaf05
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812033"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="0e67e-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0e67e-104">profilePhoto resource type</span></span>

<span data-ttu-id="0e67e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e67e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e67e-p102">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD). Os dados binários não são codificados em base-64.</span><span class="sxs-lookup"><span data-stu-id="0e67e-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD). It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="0e67e-108">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="0e67e-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="0e67e-109">No AAD, as fotos podem ser qualquer dimensão.</span><span class="sxs-lookup"><span data-stu-id="0e67e-109">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="0e67e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e67e-110">Methods</span></span>

| <span data-ttu-id="0e67e-111">Método</span><span class="sxs-lookup"><span data-stu-id="0e67e-111">Method</span></span>       | <span data-ttu-id="0e67e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e67e-112">Return Type</span></span>  |<span data-ttu-id="0e67e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e67e-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e67e-114">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0e67e-114">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="0e67e-115">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0e67e-115">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="0e67e-116">Obtenha a **profilePhoto** específica ou seus metadados (propriedades **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="0e67e-116">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="0e67e-117">Update</span><span class="sxs-lookup"><span data-stu-id="0e67e-117">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="0e67e-118">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0e67e-118">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="0e67e-p104">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="0e67e-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e67e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e67e-122">Properties</span></span>
| <span data-ttu-id="0e67e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e67e-123">Property</span></span>     | <span data-ttu-id="0e67e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e67e-124">Type</span></span>   |<span data-ttu-id="0e67e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e67e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e67e-126">id</span><span class="sxs-lookup"><span data-stu-id="0e67e-126">id</span></span>|<span data-ttu-id="0e67e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e67e-127">string</span></span>|<span data-ttu-id="0e67e-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e67e-128">Read-only.</span></span>|
|<span data-ttu-id="0e67e-129">height</span><span class="sxs-lookup"><span data-stu-id="0e67e-129">height</span></span>|<span data-ttu-id="0e67e-130">int32</span><span class="sxs-lookup"><span data-stu-id="0e67e-130">int32</span></span>|<span data-ttu-id="0e67e-p105">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e67e-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="0e67e-133">width</span><span class="sxs-lookup"><span data-stu-id="0e67e-133">width</span></span>|<span data-ttu-id="0e67e-134">int32</span><span class="sxs-lookup"><span data-stu-id="0e67e-134">int32</span></span>|<span data-ttu-id="0e67e-p106">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e67e-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e67e-137">Relações</span><span class="sxs-lookup"><span data-stu-id="0e67e-137">Relationships</span></span>
<span data-ttu-id="0e67e-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e67e-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0e67e-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e67e-139">JSON representation</span></span>

<span data-ttu-id="0e67e-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e67e-140">Here is a JSON representation of the resource.</span></span>

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
