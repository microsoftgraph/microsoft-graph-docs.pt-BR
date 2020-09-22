---
title: tipo de recurso conditionalAccessSessionControls
description: Representa um tipo complexo de controles de sessão que é aplicado após a entrada.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78c9ab3c3b5a55623ba13e1f7ce6d28a9425ded5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057007"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="010c7-103">tipo de recurso conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="010c7-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="010c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="010c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="010c7-105">Representa os controles de sessão que são aplicados após a entrada.</span><span class="sxs-lookup"><span data-stu-id="010c7-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="010c7-106">Todos os controles de sessão herdam de [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="010c7-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="010c7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="010c7-107">Properties</span></span>

| <span data-ttu-id="010c7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="010c7-108">Property</span></span>     | <span data-ttu-id="010c7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="010c7-109">Type</span></span>        | <span data-ttu-id="010c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="010c7-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="010c7-111">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="010c7-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="010c7-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="010c7-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="010c7-113">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="010c7-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="010c7-114">Somente o Exchange Online e o SharePoint Online dão suporte a esse controle de sessão.</span><span class="sxs-lookup"><span data-stu-id="010c7-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="010c7-115">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="010c7-115">cloudAppSecurity</span></span>|[<span data-ttu-id="010c7-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="010c7-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="010c7-117">Controle de sessão para aplicar o Cloud app Security.</span><span class="sxs-lookup"><span data-stu-id="010c7-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="010c7-118">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="010c7-118">persistentBrowser</span></span>|[<span data-ttu-id="010c7-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="010c7-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="010c7-120">Controle de sessão para definir se deseja persistir cookies ou não.</span><span class="sxs-lookup"><span data-stu-id="010c7-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="010c7-121">Todos os aplicativos devem ser selecionados para que esse controle de sessão funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="010c7-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="010c7-122">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="010c7-122">signInFrequency</span></span>|[<span data-ttu-id="010c7-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="010c7-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="010c7-124">Controle de sessão para impor a frequência de entrada.</span><span class="sxs-lookup"><span data-stu-id="010c7-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="010c7-125">Relações</span><span class="sxs-lookup"><span data-stu-id="010c7-125">Relationships</span></span>

<span data-ttu-id="010c7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="010c7-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="010c7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="010c7-127">JSON representation</span></span>

<span data-ttu-id="010c7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="010c7-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "applicationEnforcedRestrictions",
    "persistentBrowser",
    "cloudAppSecurity",
    "signInFrequency"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessSessionControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

