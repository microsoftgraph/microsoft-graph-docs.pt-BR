---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d68ceff79856b23f2d86b2c57a6278b7c6ad7e9d
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908583"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="9eed9-103">tipo de recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="9eed9-103">userTeamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eed9-104">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="9eed9-104">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="9eed9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9eed9-105">Properties</span></span>

| <span data-ttu-id="9eed9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9eed9-106">Property</span></span> | <span data-ttu-id="9eed9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eed9-107">Type</span></span> | <span data-ttu-id="9eed9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eed9-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9eed9-109">id</span><span class="sxs-lookup"><span data-stu-id="9eed9-109">id</span></span>|<span data-ttu-id="9eed9-110">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9eed9-110">string</span></span>| <span data-ttu-id="9eed9-111">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="9eed9-111">A globally unique identifier (GUID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="9eed9-112">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9eed9-112">Relationships</span></span>

| <span data-ttu-id="9eed9-113">Relação</span><span class="sxs-lookup"><span data-stu-id="9eed9-113">Relationship</span></span> | <span data-ttu-id="9eed9-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eed9-114">Type</span></span> | <span data-ttu-id="9eed9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eed9-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9eed9-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="9eed9-116">installedApps</span></span>|<span data-ttu-id="9eed9-117">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="9eed9-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="9eed9-118">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="9eed9-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9eed9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9eed9-119">JSON representation</span></span>

<span data-ttu-id="9eed9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9eed9-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTeamwork",
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
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
