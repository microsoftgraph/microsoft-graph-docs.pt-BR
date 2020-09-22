---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2802689810c03a4ce9931cc0c4f478d1674cfc2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057753"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="479d1-103">tipo de recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="479d1-103">userTeamwork resource type</span></span>

<span data-ttu-id="479d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="479d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="479d1-105">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="479d1-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="479d1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="479d1-106">Properties</span></span>

| <span data-ttu-id="479d1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="479d1-107">Property</span></span> | <span data-ttu-id="479d1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="479d1-108">Type</span></span> | <span data-ttu-id="479d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="479d1-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="479d1-110">id</span><span class="sxs-lookup"><span data-stu-id="479d1-110">id</span></span>|<span data-ttu-id="479d1-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="479d1-111">string</span></span>| <span data-ttu-id="479d1-112">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="479d1-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="479d1-113">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="479d1-113">Relationships</span></span>

| <span data-ttu-id="479d1-114">Relação</span><span class="sxs-lookup"><span data-stu-id="479d1-114">Relationship</span></span> | <span data-ttu-id="479d1-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="479d1-115">Type</span></span> | <span data-ttu-id="479d1-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="479d1-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="479d1-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="479d1-117">installedApps</span></span>|<span data-ttu-id="479d1-118">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="479d1-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="479d1-119">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="479d1-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="479d1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="479d1-120">JSON representation</span></span>

<span data-ttu-id="479d1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="479d1-121">The following is a JSON representation of the resource.</span></span>

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


