---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a0084504acbe576a24dac31f77e2617ed5b2c8e9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059352"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="edb07-103">tipo de recurso userTeamwork</span><span class="sxs-lookup"><span data-stu-id="edb07-103">userTeamwork resource type</span></span>

<span data-ttu-id="edb07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edb07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edb07-105">Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="edb07-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="edb07-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edb07-106">Properties</span></span>

| <span data-ttu-id="edb07-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edb07-107">Property</span></span> | <span data-ttu-id="edb07-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="edb07-108">Type</span></span> | <span data-ttu-id="edb07-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="edb07-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="edb07-110">id</span><span class="sxs-lookup"><span data-stu-id="edb07-110">id</span></span>|<span data-ttu-id="edb07-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edb07-111">string</span></span>| <span data-ttu-id="edb07-112">Um identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="edb07-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="edb07-113">Relações</span><span class="sxs-lookup"><span data-stu-id="edb07-113">Relationships</span></span>

| <span data-ttu-id="edb07-114">Relação</span><span class="sxs-lookup"><span data-stu-id="edb07-114">Relationship</span></span> | <span data-ttu-id="edb07-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="edb07-115">Type</span></span> | <span data-ttu-id="edb07-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="edb07-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="edb07-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="edb07-117">installedApps</span></span>|<span data-ttu-id="edb07-118">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="edb07-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="edb07-119">Os aplicativos instalados no escopo pessoal desse usuário.</span><span class="sxs-lookup"><span data-stu-id="edb07-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edb07-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edb07-120">JSON representation</span></span>

<span data-ttu-id="edb07-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edb07-121">The following is a JSON representation of the resource.</span></span>

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

