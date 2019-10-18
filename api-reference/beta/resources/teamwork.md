---
title: tipo de recurso de trabalho em equipe
description: Um contêiner dos recursos do Microsoft Teams disponíveis para a organização.
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7a72e34fc3d9d02a36e34295f7d4469536506df3
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908590"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="52f52-103">tipo de recurso de trabalho em equipe</span><span class="sxs-lookup"><span data-stu-id="52f52-103">teamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f52-104">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização.</span><span class="sxs-lookup"><span data-stu-id="52f52-104">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="52f52-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52f52-105">Properties</span></span>

| <span data-ttu-id="52f52-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52f52-106">Property</span></span> | <span data-ttu-id="52f52-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="52f52-107">Type</span></span> | <span data-ttu-id="52f52-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f52-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="52f52-109">id</span><span class="sxs-lookup"><span data-stu-id="52f52-109">id</span></span>|<span data-ttu-id="52f52-110">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52f52-110">string</span></span>| <span data-ttu-id="52f52-111">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="52f52-111">A globally unique identifier (GUID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="52f52-112">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="52f52-112">Relationships</span></span>

| <span data-ttu-id="52f52-113">Relação</span><span class="sxs-lookup"><span data-stu-id="52f52-113">Relationship</span></span> | <span data-ttu-id="52f52-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="52f52-114">Type</span></span> | <span data-ttu-id="52f52-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f52-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="52f52-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="52f52-116">installedApps</span></span>|<span data-ttu-id="52f52-117">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="52f52-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="52f52-118">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="52f52-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52f52-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52f52-119">JSON representation</span></span>

<span data-ttu-id="52f52-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52f52-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="52f52-121">Confira Também</span><span class="sxs-lookup"><span data-stu-id="52f52-121">See Also</span></span>

- [<span data-ttu-id="52f52-122">recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="52f52-122">userTeamwork resource</span></span>](userteamwork.md)
