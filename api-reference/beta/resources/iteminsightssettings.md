---
title: tipo de recurso itemInsightsSettings
description: Representa as configurações de privacidade de informações.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c84b2397c938997a3285d16612d090ae22444580
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522712"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="c2ece-103">tipo de recurso itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="c2ece-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ece-104">Representa as configurações de privacidade para as [idéias](iteminsights.md) e a configuração de privacidade para as ideias de horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="c2ece-104">Represents privacy settings for [itemInsights](iteminsights.md) and privacy setting for meeting hours insights.</span></span> <span data-ttu-id="c2ece-105">Use esta API para desabilitar/habilitar o cálculo e a visibilidade de insights de itens e de horas de reunião.</span><span class="sxs-lookup"><span data-stu-id="c2ece-105">Use this API to disable/enable calculation and visibility of item insights and meeting hours insights.</span></span> 

- <span data-ttu-id="c2ece-106">Insights de item: calcula a relação entre usuários e itens, como documentos ou sites no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c2ece-106">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="c2ece-107">Observações de horário de reunião: calcula as horas de reunião de calendário de uma pessoa com base nas atividades no Word, Excel, PowerPoint, email e calendário do Outlook no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c2ece-107">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

> [!NOTE]
> <span data-ttu-id="c2ece-108">Horas de reunião as ideias estão implantando para clientes que começam de novembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="c2ece-108">Meeting hours insights are rolling out to customers starting November 2020.</span></span> 

## <a name="methods"></a><span data-ttu-id="c2ece-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c2ece-109">Methods</span></span>

| <span data-ttu-id="c2ece-110">Método</span><span class="sxs-lookup"><span data-stu-id="c2ece-110">Method</span></span>       | <span data-ttu-id="c2ece-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c2ece-111">Return Type</span></span> | <span data-ttu-id="c2ece-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ece-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="c2ece-113">Get</span><span class="sxs-lookup"><span data-stu-id="c2ece-113">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="c2ece-114">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="c2ece-114">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="c2ece-115">Ler as propriedades de um objeto **itemInsightsSettings** .</span><span class="sxs-lookup"><span data-stu-id="c2ece-115">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="c2ece-116">Update</span><span class="sxs-lookup"><span data-stu-id="c2ece-116">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="c2ece-117">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="c2ece-117">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="c2ece-118">Atualize um objeto **itemInsightsSettings** .</span><span class="sxs-lookup"><span data-stu-id="c2ece-118">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="c2ece-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2ece-119">Properties</span></span>
| <span data-ttu-id="c2ece-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2ece-120">Property</span></span>   | <span data-ttu-id="c2ece-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2ece-121">Type</span></span>|<span data-ttu-id="c2ece-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ece-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2ece-123">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="c2ece-123">isEnabledInOrganization</span></span>|<span data-ttu-id="c2ece-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ece-124">Boolean</span></span>| <span data-ttu-id="c2ece-125">`true` Se o item de organização insights estiver habilitado; `false` se o item de organização insights estiver desabilitado para todos os usuários sem exceções.</span><span class="sxs-lookup"><span data-stu-id="c2ece-125">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="c2ece-126">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="c2ece-126">Default is `true`.</span></span> <span data-ttu-id="c2ece-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c2ece-127">Optional.</span></span>|
|<span data-ttu-id="c2ece-128">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="c2ece-128">disabledForGroup</span></span>|<span data-ttu-id="c2ece-129">String</span><span class="sxs-lookup"><span data-stu-id="c2ece-129">String</span></span>| <span data-ttu-id="c2ece-130">A ID de um grupo do Azure AD, do qual as insights do item dos membros estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="c2ece-130">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="c2ece-131">O padrão é `empty`.</span><span class="sxs-lookup"><span data-stu-id="c2ece-131">Default is `empty`.</span></span> <span data-ttu-id="c2ece-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c2ece-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2ece-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2ece-133">JSON representation</span></span>

<span data-ttu-id="c2ece-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c2ece-134">Here is a JSON representation of the resource</span></span>
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


