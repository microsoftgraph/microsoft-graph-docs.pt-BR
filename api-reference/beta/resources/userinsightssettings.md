---
title: Tipo de recurso userInsightsSettings
description: Representa as configurações de privacidade do usuário para insights de item e informações de horários de reunião.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5ecc9277d0bd98df99387a5dd222998074c6eb1b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109060"
---
# <a name="userinsightssettings-resource-type"></a><span data-ttu-id="7ac11-103">Tipo de recurso userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7ac11-103">userInsightsSettings resource type</span></span>

<span data-ttu-id="7ac11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac11-105">Representa as configurações de privacidade do usuário [para o itemInsights](iteminsights.md) e informações sobre horários [de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="7ac11-105">Represents user privacy settings for [itemInsights](iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) .</span></span> <span data-ttu-id="7ac11-106">Use esse recurso para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e dos horários de reunião de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ac11-106">Use this resource to disable/enable calculation and visibility of item insights and meeting hours insights of a user.</span></span> 

- <span data-ttu-id="7ac11-107">Insights de item: calcula a relação entre usuários e itens, como documentos ou sites em Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7ac11-107">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="7ac11-108">Insights do horário de reunião: calcula o horário de reunião do calendário de uma pessoa com base nas atividades no Word, Excel, PowerPoint, email e Outlook calendário no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7ac11-108">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

<span data-ttu-id="7ac11-109">Use o [recurso itemInsightsSettings](iteminsightssettings.md) para desabilitar/habilitar o cálculo e a visibilidade das percepções do item e do horário de reunião em um nível de organização.</span><span class="sxs-lookup"><span data-stu-id="7ac11-109">Use the [itemInsightsSettings](iteminsightssettings.md) resource to disable/enable calculation and visibility of item insights and meeting hours insights at an organization level.</span></span>

## <a name="methods"></a><span data-ttu-id="7ac11-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ac11-110">Methods</span></span>

| <span data-ttu-id="7ac11-111">Método</span><span class="sxs-lookup"><span data-stu-id="7ac11-111">Method</span></span>                                                 | <span data-ttu-id="7ac11-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ac11-112">Return Type</span></span>                                                   | <span data-ttu-id="7ac11-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac11-113">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="7ac11-114">Get</span><span class="sxs-lookup"><span data-stu-id="7ac11-114">Get</span></span>](../api/userinsightssettings-get.md)       | [<span data-ttu-id="7ac11-115">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7ac11-115">userInsightsSettings</span></span>](userinsightssettings.md) | <span data-ttu-id="7ac11-116">Leia as propriedades de **um objeto userinsightssettings.**</span><span class="sxs-lookup"><span data-stu-id="7ac11-116">Read the properties of a **userinsightssettings** object.</span></span>  |
| [<span data-ttu-id="7ac11-117">Atualizar</span><span class="sxs-lookup"><span data-stu-id="7ac11-117">Update</span></span>](../api/userinsightssettings-update.md) | [<span data-ttu-id="7ac11-118">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="7ac11-118">userInsightsSettings</span></span>](userinsightssettings.md) | <span data-ttu-id="7ac11-119">Atualize as propriedades de **um objeto userinsightssettings.**</span><span class="sxs-lookup"><span data-stu-id="7ac11-119">Update the properties of a **userinsightssettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ac11-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ac11-120">Properties</span></span>
| <span data-ttu-id="7ac11-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac11-121">Property</span></span>                   | <span data-ttu-id="7ac11-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac11-122">Type</span></span>                                                  | <span data-ttu-id="7ac11-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac11-123">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7ac11-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7ac11-124">isEnabled</span></span>     | <span data-ttu-id="7ac11-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ac11-125">Boolean</span></span>  |  <span data-ttu-id="7ac11-126">`true` se os insights **de item do usuárioInsights** e de horas de reunião estão habilitados; `false` se o item do **usuárioInights** e as percepções do horário de reunião estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="7ac11-126">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="7ac11-127">O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="7ac11-127">Default is `true`.</span></span> <span data-ttu-id="7ac11-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7ac11-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ac11-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ac11-129">JSON representation</span></span>

<span data-ttu-id="7ac11-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ac11-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.userInsightsSettings"
}-->

```json
{
  "isEnabled": "Boolean"
}
```


