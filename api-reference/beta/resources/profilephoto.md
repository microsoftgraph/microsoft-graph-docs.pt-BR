---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD). Seus dados binários não são codificados em base 64.
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563259"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="bdea3-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="bdea3-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdea3-105">Uma foto de perfil de um usuário, grupo ou contato do Outlook acessado a partir do Exchange Online ou do Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="bdea3-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="bdea3-106">Seus dados binários não são codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="bdea3-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="bdea3-107">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="bdea3-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="bdea3-108">No AAD, as fotos podem ser qualquer dimensão.</span><span class="sxs-lookup"><span data-stu-id="bdea3-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="bdea3-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="bdea3-109">Methods</span></span>

| <span data-ttu-id="bdea3-110">Método</span><span class="sxs-lookup"><span data-stu-id="bdea3-110">Method</span></span>       | <span data-ttu-id="bdea3-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bdea3-111">Return Type</span></span>  |<span data-ttu-id="bdea3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdea3-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdea3-113">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="bdea3-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="bdea3-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="bdea3-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="bdea3-115">Obtenha a **profilePhoto** específica ou seus metadados (propriedades **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="bdea3-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="bdea3-116">Update</span><span class="sxs-lookup"><span data-stu-id="bdea3-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="bdea3-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="bdea3-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="bdea3-p104">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="bdea3-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="bdea3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdea3-121">Properties</span></span>
| <span data-ttu-id="bdea3-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdea3-122">Property</span></span>     | <span data-ttu-id="bdea3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdea3-123">Type</span></span>   |<span data-ttu-id="bdea3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdea3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdea3-125">id</span><span class="sxs-lookup"><span data-stu-id="bdea3-125">id</span></span>|<span data-ttu-id="bdea3-126">string</span><span class="sxs-lookup"><span data-stu-id="bdea3-126">string</span></span>|<span data-ttu-id="bdea3-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdea3-127">Read-only.</span></span>|
|<span data-ttu-id="bdea3-128">height</span><span class="sxs-lookup"><span data-stu-id="bdea3-128">height</span></span>|<span data-ttu-id="bdea3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="bdea3-129">int32</span></span>|<span data-ttu-id="bdea3-p105">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdea3-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="bdea3-132">width</span><span class="sxs-lookup"><span data-stu-id="bdea3-132">width</span></span>|<span data-ttu-id="bdea3-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bdea3-133">int32</span></span>|<span data-ttu-id="bdea3-p106">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdea3-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdea3-136">Relações</span><span class="sxs-lookup"><span data-stu-id="bdea3-136">Relationships</span></span>
<span data-ttu-id="bdea3-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdea3-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bdea3-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdea3-138">JSON representation</span></span>

<span data-ttu-id="bdea3-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdea3-139">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
