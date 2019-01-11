---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou um contato do Outlook acessado a partir do Exchange Online ou no Windows Azure Active Directory (AAD). É dados binários não codificados em base 64.
localization_priority: Normal
ms.openlocfilehash: 7754d70c4e59b13b1b0003022ddc0f185cc18ae2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837062"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="5dd21-104">Tipo de recurso de profilePhoto</span><span class="sxs-lookup"><span data-stu-id="5dd21-104">profilePhoto resource type</span></span>

> <span data-ttu-id="5dd21-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5dd21-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dd21-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5dd21-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5dd21-107">Uma foto de perfil de um usuário, grupo ou um contato do Outlook acessado a partir do Exchange Online ou no Windows Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="5dd21-107">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="5dd21-108">É dados binários não codificados em base 64.</span><span class="sxs-lookup"><span data-stu-id="5dd21-108">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="5dd21-109">Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="5dd21-109">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="5dd21-110">Em AAD, fotos podem ser qualquer dimensão.</span><span class="sxs-lookup"><span data-stu-id="5dd21-110">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="5dd21-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="5dd21-111">Methods</span></span>

| <span data-ttu-id="5dd21-112">Método</span><span class="sxs-lookup"><span data-stu-id="5dd21-112">Method</span></span>       | <span data-ttu-id="5dd21-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5dd21-113">Return Type</span></span>  |<span data-ttu-id="5dd21-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dd21-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5dd21-115">Get profilePhoto</span><span class="sxs-lookup"><span data-stu-id="5dd21-115">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="5dd21-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="5dd21-116">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="5dd21-117">Obtenha o especificado **profilePhoto** ou seus metadados (**profilePhoto** propriedades).</span><span class="sxs-lookup"><span data-stu-id="5dd21-117">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="5dd21-118">Update</span><span class="sxs-lookup"><span data-stu-id="5dd21-118">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="5dd21-119">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="5dd21-119">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="5dd21-p105">Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.</span><span class="sxs-lookup"><span data-stu-id="5dd21-p105">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="5dd21-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5dd21-123">Properties</span></span>
| <span data-ttu-id="5dd21-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dd21-124">Property</span></span>     | <span data-ttu-id="5dd21-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dd21-125">Type</span></span>   |<span data-ttu-id="5dd21-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dd21-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dd21-127">id</span><span class="sxs-lookup"><span data-stu-id="5dd21-127">id</span></span>|<span data-ttu-id="5dd21-128">string</span><span class="sxs-lookup"><span data-stu-id="5dd21-128">string</span></span>|<span data-ttu-id="5dd21-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5dd21-129">Read-only.</span></span>|
|<span data-ttu-id="5dd21-130">height</span><span class="sxs-lookup"><span data-stu-id="5dd21-130">height</span></span>|<span data-ttu-id="5dd21-131">int32</span><span class="sxs-lookup"><span data-stu-id="5dd21-131">int32</span></span>|<span data-ttu-id="5dd21-p106">A altura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5dd21-p106">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="5dd21-134">width</span><span class="sxs-lookup"><span data-stu-id="5dd21-134">width</span></span>|<span data-ttu-id="5dd21-135">int32</span><span class="sxs-lookup"><span data-stu-id="5dd21-135">int32</span></span>|<span data-ttu-id="5dd21-p107">A largura da foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5dd21-p107">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dd21-138">Relações</span><span class="sxs-lookup"><span data-stu-id="5dd21-138">Relationships</span></span>
<span data-ttu-id="5dd21-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dd21-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5dd21-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5dd21-140">JSON representation</span></span>

<span data-ttu-id="5dd21-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5dd21-141">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
