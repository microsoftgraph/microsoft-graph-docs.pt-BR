---
title: tipo de recurso conditionalAccessSessionControls
description: Representa um tipo complexo de controles de sessão que é aplicado após a entrada.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 317120eb7c4138d955bf8a35030375180d5a1631
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638544"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="064ae-103">tipo de recurso conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="064ae-103">conditionalAccessSessionControls resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="064ae-104">Representa os controles de sessão que são aplicados após a entrada.</span><span class="sxs-lookup"><span data-stu-id="064ae-104">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="064ae-105">Todos os controles de sessão herdam de [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="064ae-105">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="064ae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="064ae-106">Properties</span></span>

| <span data-ttu-id="064ae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="064ae-107">Property</span></span>     | <span data-ttu-id="064ae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="064ae-108">Type</span></span>        | <span data-ttu-id="064ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="064ae-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="064ae-110">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="064ae-110">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="064ae-111">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="064ae-111">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="064ae-112">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="064ae-112">Session control to enforce application restrictions.</span></span> <span data-ttu-id="064ae-113">Somente o Exchange Online e o SharePoint Online dão suporte a esse controle de sessão.</span><span class="sxs-lookup"><span data-stu-id="064ae-113">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="064ae-114">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="064ae-114">cloudAppSecurity</span></span>|[<span data-ttu-id="064ae-115">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="064ae-115">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="064ae-116">Controle de sessão para aplicar o Cloud app Security.</span><span class="sxs-lookup"><span data-stu-id="064ae-116">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="064ae-117">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="064ae-117">persistentBrowser</span></span>|[<span data-ttu-id="064ae-118">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="064ae-118">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="064ae-119">Controle de sessão para definir se deseja persistir cookies ou não.</span><span class="sxs-lookup"><span data-stu-id="064ae-119">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="064ae-120">Todos os aplicativos devem ser selecionados para que esse controle de sessão funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="064ae-120">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="064ae-121">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="064ae-121">signInFrequency</span></span>|[<span data-ttu-id="064ae-122">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="064ae-122">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="064ae-123">Controle de sessão para impor a frequência de entrada.</span><span class="sxs-lookup"><span data-stu-id="064ae-123">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="064ae-124">Relações</span><span class="sxs-lookup"><span data-stu-id="064ae-124">Relationships</span></span>

<span data-ttu-id="064ae-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="064ae-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="064ae-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="064ae-126">JSON representation</span></span>

<span data-ttu-id="064ae-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="064ae-127">The following is a JSON representation of the resource.</span></span>

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