---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 721830c8a4160046bb4ffd09e2812c4e0f95167d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015299"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="3c283-103">tipo de recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="3c283-103">userTeamwork resource type</span></span>

<span data-ttu-id="3c283-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c283-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c283-105">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="3c283-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="3c283-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c283-106">Properties</span></span>

| <span data-ttu-id="3c283-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c283-107">Property</span></span> | <span data-ttu-id="3c283-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c283-108">Type</span></span> | <span data-ttu-id="3c283-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c283-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3c283-110">id</span><span class="sxs-lookup"><span data-stu-id="3c283-110">id</span></span>|<span data-ttu-id="3c283-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c283-111">string</span></span>| <span data-ttu-id="3c283-112">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="3c283-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3c283-113">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="3c283-113">Relationships</span></span>

| <span data-ttu-id="3c283-114">Relação</span><span class="sxs-lookup"><span data-stu-id="3c283-114">Relationship</span></span> | <span data-ttu-id="3c283-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c283-115">Type</span></span> | <span data-ttu-id="3c283-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c283-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3c283-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="3c283-117">installedApps</span></span>|<span data-ttu-id="3c283-118">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="3c283-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="3c283-119">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="3c283-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c283-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c283-120">JSON representation</span></span>

<span data-ttu-id="3c283-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c283-121">The following is a JSON representation of the resource.</span></span>

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

