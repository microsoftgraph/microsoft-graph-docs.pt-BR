---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser cumpridos para passar a política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b2dba27c987351619a347a16d20b2a4b88646045
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961283"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="7caae-103">Tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="7caae-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="7caae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7caae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7caae-105">Representa os controles de concessão que devem ser cumpridos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="7caae-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="7caae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7caae-106">Properties</span></span>

| <span data-ttu-id="7caae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7caae-107">Property</span></span> | <span data-ttu-id="7caae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7caae-108">Type</span></span> | <span data-ttu-id="7caae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7caae-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="7caae-110">operator</span><span class="sxs-lookup"><span data-stu-id="7caae-110">operator</span></span> | <span data-ttu-id="7caae-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7caae-111">String</span></span> | <span data-ttu-id="7caae-112">Define a relação dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="7caae-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="7caae-113">Valores possíveis: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="7caae-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="7caae-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="7caae-114">builtInControls</span></span> | <span data-ttu-id="7caae-115">Coleção conditionalAccessGrantControl</span><span class="sxs-lookup"><span data-stu-id="7caae-115">conditionalAccessGrantControl collection</span></span> | <span data-ttu-id="7caae-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="7caae-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="7caae-117">Valores possíveis: `block` , , , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="7caae-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="7caae-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="7caae-118">customAuthenticationFactors</span></span> | <span data-ttu-id="7caae-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7caae-119">String collection</span></span> | <span data-ttu-id="7caae-120">Lista de IDs de controles personalizados exigidas pela política.</span><span class="sxs-lookup"><span data-stu-id="7caae-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="7caae-121">Saiba mais sobre controles personalizados aqui: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="7caae-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="7caae-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="7caae-122">termsOfUse</span></span> | <span data-ttu-id="7caae-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7caae-123">String collection</span></span> | <span data-ttu-id="7caae-124">Lista de [termos de](agreement.md) IDs de uso exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="7caae-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="7caae-125">Considerações especiais ao usar `passwordChange` como um controle</span><span class="sxs-lookup"><span data-stu-id="7caae-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="7caae-126">Considere o seguinte ao usar o `passwordChange` controle:</span><span class="sxs-lookup"><span data-stu-id="7caae-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="7caae-127">`passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador.</span><span class="sxs-lookup"><span data-stu-id="7caae-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="7caae-128">Essa combinação garante que a senha seja atualizada de forma segura.</span><span class="sxs-lookup"><span data-stu-id="7caae-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="7caae-129">`passwordChange` deve ser usado em uma política que contenha `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="7caae-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="7caae-130">Isso foi projetado para habilitar cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.</span><span class="sxs-lookup"><span data-stu-id="7caae-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="7caae-131">A política deve direcionar `all` aplicativos e não excluir aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7caae-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="7caae-132">A política não pode conter nenhuma outra condição.</span><span class="sxs-lookup"><span data-stu-id="7caae-132">The policy cannot contain any other condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="7caae-133">Relações</span><span class="sxs-lookup"><span data-stu-id="7caae-133">Relationships</span></span>

<span data-ttu-id="7caae-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7caae-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7caae-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7caae-135">JSON representation</span></span>

<span data-ttu-id="7caae-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7caae-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


