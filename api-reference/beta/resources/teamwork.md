---
title: tipo de recurso de trabalho em equipe
description: Um contêiner dos recursos do Microsoft Teams disponíveis para a organização.
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 439a4c5234d6442c2394dc8154b08d7cce2e5c69
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060451"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="f1819-103">tipo de recurso de trabalho em equipe</span><span class="sxs-lookup"><span data-stu-id="f1819-103">teamwork resource type</span></span>

<span data-ttu-id="f1819-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1819-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1819-105">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização.</span><span class="sxs-lookup"><span data-stu-id="f1819-105">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="f1819-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1819-106">Properties</span></span>

| <span data-ttu-id="f1819-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1819-107">Property</span></span> | <span data-ttu-id="f1819-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1819-108">Type</span></span> | <span data-ttu-id="f1819-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1819-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f1819-110">id</span><span class="sxs-lookup"><span data-stu-id="f1819-110">id</span></span>|<span data-ttu-id="f1819-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1819-111">string</span></span>| <span data-ttu-id="f1819-112">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="f1819-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f1819-113">Relações</span><span class="sxs-lookup"><span data-stu-id="f1819-113">Relationships</span></span>

| <span data-ttu-id="f1819-114">Relação</span><span class="sxs-lookup"><span data-stu-id="f1819-114">Relationship</span></span> | <span data-ttu-id="f1819-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1819-115">Type</span></span> | <span data-ttu-id="f1819-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1819-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f1819-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="f1819-117">installedApps</span></span>|<span data-ttu-id="f1819-118">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="f1819-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="f1819-119">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="f1819-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1819-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1819-120">JSON representation</span></span>

<span data-ttu-id="f1819-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1819-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f1819-122">Confira Também</span><span class="sxs-lookup"><span data-stu-id="f1819-122">See Also</span></span>

- [<span data-ttu-id="f1819-123">recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="f1819-123">userTeamwork resource</span></span>](userteamwork.md)


