---
title: tipo de recurso itemInsightsSettings
description: Representa as configurações de privacidade de informações.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3be5fa87fd6c2623126437fccb1ea43b7bc275f2
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427519"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="7e7d2-103">tipo de recurso itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7e7d2-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e7d2-104">Representa as configurações de [privacidade para os](iteminsights.md)itens que configuram a visibilidade de insights derivadas do Microsoft Graph, entre usuários e outros itens (como documentos ou sites) no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-104">Represents privacy settings for [itemInsights](iteminsights.md), which configure the visibility of insights derived from Microsoft Graph, between users and other items (such as documents or sites) in Microsoft 365.</span></span>

## <a name="methods"></a><span data-ttu-id="7e7d2-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7e7d2-105">Methods</span></span>

| <span data-ttu-id="7e7d2-106">Método</span><span class="sxs-lookup"><span data-stu-id="7e7d2-106">Method</span></span>       | <span data-ttu-id="7e7d2-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7e7d2-107">Return Type</span></span> | <span data-ttu-id="7e7d2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e7d2-108">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="7e7d2-109">Get</span><span class="sxs-lookup"><span data-stu-id="7e7d2-109">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="7e7d2-110">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7e7d2-110">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="7e7d2-111">Ler as propriedades de um objeto **itemInsightsSettings** .</span><span class="sxs-lookup"><span data-stu-id="7e7d2-111">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="7e7d2-112">Update</span><span class="sxs-lookup"><span data-stu-id="7e7d2-112">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="7e7d2-113">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7e7d2-113">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="7e7d2-114">Atualize um objeto **itemInsightsSettings** .</span><span class="sxs-lookup"><span data-stu-id="7e7d2-114">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="7e7d2-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e7d2-115">Properties</span></span>
| <span data-ttu-id="7e7d2-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e7d2-116">Property</span></span>   | <span data-ttu-id="7e7d2-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e7d2-117">Type</span></span>|<span data-ttu-id="7e7d2-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e7d2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e7d2-119">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="7e7d2-119">isEnabledInOrganization</span></span>|<span data-ttu-id="7e7d2-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e7d2-120">Boolean</span></span>| <span data-ttu-id="7e7d2-121">`true`Se o item de organização insights estiver habilitado; `false`se o item de organização insights estiver desabilitado para todos os usuários sem exceções.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-121">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="7e7d2-122">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-122">Default is `true`.</span></span> <span data-ttu-id="7e7d2-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-123">Optional.</span></span>|
|<span data-ttu-id="7e7d2-124">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="7e7d2-124">disabledForGroup</span></span>|<span data-ttu-id="7e7d2-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e7d2-125">String</span></span>| <span data-ttu-id="7e7d2-126">A ID de um grupo do Azure AD, do qual as insights do item dos membros estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-126">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="7e7d2-127">O padrão é `empty`.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-127">Default is `empty`.</span></span> <span data-ttu-id="7e7d2-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7e7d2-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e7d2-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e7d2-129">JSON representation</span></span>

<span data-ttu-id="7e7d2-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7e7d2-130">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.itemInsightsSettings"
}-->

```json
{
  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```
