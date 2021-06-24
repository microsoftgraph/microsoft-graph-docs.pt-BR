---
title: Tipo de recurso itemInsightsSettings
description: Representa configurações de privacidade para itemInsights.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80ca42440bcf365e051d9fb25fbc088af8a7f4bb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108821"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="6d07f-103">Tipo de recurso itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="6d07f-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d07f-104">Representa configurações de privacidade para [itemInsights](iteminsights.md) e configuração de privacidade para insights [de horário de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="6d07f-104">Represents privacy settings for [itemInsights](iteminsights.md) and privacy setting for [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) .</span></span> <span data-ttu-id="6d07f-105">Use essa API para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e dos horários de reunião.</span><span class="sxs-lookup"><span data-stu-id="6d07f-105">Use this API to disable/enable calculation and visibility of item insights and meeting hours insights.</span></span> 

- <span data-ttu-id="6d07f-106">Insights de item: calcula a relação entre usuários e itens, como documentos ou sites em Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d07f-106">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="6d07f-107">Insights do horário de reunião: calcula o horário de reunião do calendário de uma pessoa com base nas atividades no Word, Excel, PowerPoint, email e Outlook calendário no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d07f-107">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

<span data-ttu-id="6d07f-108">Use o [recurso userInsightsSettings](userinsightssettings.md) para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e dos insights do horário de reunião de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6d07f-108">Use the [userInsightsSettings](userinsightssettings.md) resource to disable/enable calculation and visibility of item insights and meeting hours insights of a user.</span></span>

## <a name="methods"></a><span data-ttu-id="6d07f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="6d07f-109">Methods</span></span>

| <span data-ttu-id="6d07f-110">Método</span><span class="sxs-lookup"><span data-stu-id="6d07f-110">Method</span></span>       | <span data-ttu-id="6d07f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6d07f-111">Return Type</span></span> | <span data-ttu-id="6d07f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d07f-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="6d07f-113">Get</span><span class="sxs-lookup"><span data-stu-id="6d07f-113">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="6d07f-114">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="6d07f-114">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="6d07f-115">Leia as propriedades de um **objeto itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="6d07f-115">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="6d07f-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6d07f-116">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="6d07f-117">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="6d07f-117">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="6d07f-118">Atualizar um **objeto itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="6d07f-118">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6d07f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d07f-119">Properties</span></span>
| <span data-ttu-id="6d07f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d07f-120">Property</span></span>   | <span data-ttu-id="6d07f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d07f-121">Type</span></span>|<span data-ttu-id="6d07f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d07f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d07f-123">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="6d07f-123">isEnabledInOrganization</span></span>|<span data-ttu-id="6d07f-124">Booleano</span><span class="sxs-lookup"><span data-stu-id="6d07f-124">Boolean</span></span>| <span data-ttu-id="6d07f-125">`true` se as percepções do item da organização estão habilitadas; `false` se as percepções do item da organização estão desabilitadas para todos os usuários sem exceções.</span><span class="sxs-lookup"><span data-stu-id="6d07f-125">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="6d07f-126">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="6d07f-126">Default is `true`.</span></span> <span data-ttu-id="6d07f-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6d07f-127">Optional.</span></span>|
|<span data-ttu-id="6d07f-128">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="6d07f-128">disabledForGroup</span></span>|<span data-ttu-id="6d07f-129">String</span><span class="sxs-lookup"><span data-stu-id="6d07f-129">String</span></span>| <span data-ttu-id="6d07f-130">A ID de um grupo do Azure AD, do qual as informações do item dos membros estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="6d07f-130">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="6d07f-131">O padrão é `empty`.</span><span class="sxs-lookup"><span data-stu-id="6d07f-131">Default is `empty`.</span></span> <span data-ttu-id="6d07f-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6d07f-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d07f-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d07f-133">JSON representation</span></span>

<span data-ttu-id="6d07f-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d07f-134">Here is a JSON representation of the resource</span></span>
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


