---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6ef5bb1ddf0944e7d61ab5321ae50e766713326c
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060442"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="f1287-103">tipo de recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="f1287-103">userTeamwork resource type</span></span>

<span data-ttu-id="f1287-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1287-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1287-105">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="f1287-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="f1287-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1287-106">Properties</span></span>

| <span data-ttu-id="f1287-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1287-107">Property</span></span> | <span data-ttu-id="f1287-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1287-108">Type</span></span> | <span data-ttu-id="f1287-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1287-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f1287-110">id</span><span class="sxs-lookup"><span data-stu-id="f1287-110">id</span></span>|<span data-ttu-id="f1287-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1287-111">string</span></span>| <span data-ttu-id="f1287-112">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="f1287-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f1287-113">Relações</span><span class="sxs-lookup"><span data-stu-id="f1287-113">Relationships</span></span>

| <span data-ttu-id="f1287-114">Relação</span><span class="sxs-lookup"><span data-stu-id="f1287-114">Relationship</span></span> | <span data-ttu-id="f1287-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1287-115">Type</span></span> | <span data-ttu-id="f1287-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1287-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f1287-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="f1287-117">installedApps</span></span>|<span data-ttu-id="f1287-118">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="f1287-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="f1287-119">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="f1287-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1287-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1287-120">JSON representation</span></span>

<span data-ttu-id="f1287-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1287-121">The following is a JSON representation of the resource.</span></span>

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


