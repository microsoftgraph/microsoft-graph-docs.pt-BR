---
title: tipo de recurso de trabalho em equipe
description: Um contêiner dos recursos do Microsoft Teams disponíveis para a organização.
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1d44520fd680bbfb67d4a756b24e1533a64041b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046332"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="fb652-103">tipo de recurso de trabalho em equipe</span><span class="sxs-lookup"><span data-stu-id="fb652-103">teamwork resource type</span></span>

<span data-ttu-id="fb652-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb652-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb652-105">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização.</span><span class="sxs-lookup"><span data-stu-id="fb652-105">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="fb652-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb652-106">Properties</span></span>

| <span data-ttu-id="fb652-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb652-107">Property</span></span> | <span data-ttu-id="fb652-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb652-108">Type</span></span> | <span data-ttu-id="fb652-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb652-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fb652-110">id</span><span class="sxs-lookup"><span data-stu-id="fb652-110">id</span></span>|<span data-ttu-id="fb652-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb652-111">string</span></span>| <span data-ttu-id="fb652-112">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="fb652-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fb652-113">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="fb652-113">Relationships</span></span>

| <span data-ttu-id="fb652-114">Relação</span><span class="sxs-lookup"><span data-stu-id="fb652-114">Relationship</span></span> | <span data-ttu-id="fb652-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb652-115">Type</span></span> | <span data-ttu-id="fb652-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb652-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fb652-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="fb652-117">installedApps</span></span>|<span data-ttu-id="fb652-118">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="fb652-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="fb652-119">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="fb652-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb652-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb652-120">JSON representation</span></span>

<span data-ttu-id="fb652-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb652-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fb652-122">Confira Também</span><span class="sxs-lookup"><span data-stu-id="fb652-122">See Also</span></span>

- [<span data-ttu-id="fb652-123">recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="fb652-123">userTeamwork resource</span></span>](userteamwork.md)


