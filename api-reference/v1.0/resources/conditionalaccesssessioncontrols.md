---
title: Tipo de recurso conditionalAccessSessionControls
description: Representa um tipo complexo de controles de sessão que é imposto após a logon.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7e41def74a1654b20e1aa3618abdc6518e774045
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135930"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="a68db-103">Tipo de recurso conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="a68db-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="a68db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a68db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a68db-105">Representa os controles de sessão que são aplicados após a logon.</span><span class="sxs-lookup"><span data-stu-id="a68db-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="a68db-106">Todos os controles de sessão [herdam de conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="a68db-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a68db-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a68db-107">Properties</span></span>

| <span data-ttu-id="a68db-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a68db-108">Property</span></span>     | <span data-ttu-id="a68db-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a68db-109">Type</span></span>        | <span data-ttu-id="a68db-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a68db-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a68db-111">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="a68db-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="a68db-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="a68db-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="a68db-113">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a68db-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="a68db-114">Somente o Exchange Online e o SharePoint Online suportam esse controle de sessão.</span><span class="sxs-lookup"><span data-stu-id="a68db-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="a68db-115">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="a68db-115">cloudAppSecurity</span></span>|[<span data-ttu-id="a68db-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="a68db-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="a68db-117">Controle de sessão para aplicar a segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="a68db-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="a68db-118">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="a68db-118">persistentBrowser</span></span>|[<span data-ttu-id="a68db-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="a68db-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="a68db-120">Controle de sessão para definir se os cookies serão persistentes ou não.</span><span class="sxs-lookup"><span data-stu-id="a68db-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="a68db-121">Todos os aplicativos devem ser selecionados para que esse controle de sessão funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="a68db-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="a68db-122">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="a68db-122">signInFrequency</span></span>|[<span data-ttu-id="a68db-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="a68db-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="a68db-124">Controle de sessão para impor a frequência de login.</span><span class="sxs-lookup"><span data-stu-id="a68db-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a68db-125">Relações</span><span class="sxs-lookup"><span data-stu-id="a68db-125">Relationships</span></span>

<span data-ttu-id="a68db-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a68db-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a68db-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a68db-127">JSON representation</span></span>

<span data-ttu-id="a68db-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a68db-128">The following is a JSON representation of the resource.</span></span>

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

