---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 99b6d6dc3bd15ea84c4a8507981acd9c8ac2eb6f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130785"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="ec22b-103">Tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="ec22b-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="ec22b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec22b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec22b-105">Representa controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="ec22b-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="ec22b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec22b-106">Properties</span></span>

| <span data-ttu-id="ec22b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec22b-107">Property</span></span> | <span data-ttu-id="ec22b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec22b-108">Type</span></span> | <span data-ttu-id="ec22b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec22b-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="ec22b-110">operator</span><span class="sxs-lookup"><span data-stu-id="ec22b-110">operator</span></span> | <span data-ttu-id="ec22b-111">String</span><span class="sxs-lookup"><span data-stu-id="ec22b-111">String</span></span> | <span data-ttu-id="ec22b-112">Define a relação dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="ec22b-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="ec22b-113">Valores possíveis: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="ec22b-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="ec22b-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="ec22b-114">builtInControls</span></span> | <span data-ttu-id="ec22b-115">String collection</span><span class="sxs-lookup"><span data-stu-id="ec22b-115">String collection</span></span> | <span data-ttu-id="ec22b-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="ec22b-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="ec22b-117">Valores possíveis: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` .</span><span class="sxs-lookup"><span data-stu-id="ec22b-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="ec22b-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="ec22b-118">customAuthenticationFactors</span></span> | <span data-ttu-id="ec22b-119">String collection</span><span class="sxs-lookup"><span data-stu-id="ec22b-119">String collection</span></span> | <span data-ttu-id="ec22b-120">Lista de IDs de controles personalizados exigidas pela política.</span><span class="sxs-lookup"><span data-stu-id="ec22b-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="ec22b-121">Para obter mais informações, consulte [Controles personalizados.](/azure/active-directory/conditional-access/controls)</span><span class="sxs-lookup"><span data-stu-id="ec22b-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="ec22b-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="ec22b-122">termsOfUse</span></span> | <span data-ttu-id="ec22b-123">String collection</span><span class="sxs-lookup"><span data-stu-id="ec22b-123">String collection</span></span> | <span data-ttu-id="ec22b-124">Lista de [IDs de](/graph/api/resources/agreement) termos de uso exigida pela política.</span><span class="sxs-lookup"><span data-stu-id="ec22b-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="ec22b-125">Considerações especiais ao usar `passwordChange` como um controle</span><span class="sxs-lookup"><span data-stu-id="ec22b-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="ec22b-126">Considere o seguinte ao usar o `passwordChange` controle:</span><span class="sxs-lookup"><span data-stu-id="ec22b-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="ec22b-127">`passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador.</span><span class="sxs-lookup"><span data-stu-id="ec22b-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="ec22b-128">Essa combinação garante que a senha seja atualizada de maneira segura.</span><span class="sxs-lookup"><span data-stu-id="ec22b-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="ec22b-129">`passwordChange` deve ser usado em uma política que contém `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="ec22b-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="ec22b-130">Isso foi projetado para permitir cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.</span><span class="sxs-lookup"><span data-stu-id="ec22b-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="ec22b-131">A política deve direcionar `all` aplicativos e não excluir aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ec22b-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="ec22b-132">A política não pode conter nenhuma outra condição, exceto `users` e `applications` `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="ec22b-132">The policy cannot contain any other condition except `users`, `applications` and `userRiskLevels`.</span></span>

## <a name="relationships"></a><span data-ttu-id="ec22b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="ec22b-133">Relationships</span></span>

<span data-ttu-id="ec22b-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec22b-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec22b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec22b-135">JSON representation</span></span>

<span data-ttu-id="ec22b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec22b-136">The following is a JSON representation of the resource.</span></span>

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
