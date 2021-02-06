---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6d8717c1ca8fcd9113b8aeacb5a4a1cefce8df8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130470"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="1c49e-103">Tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="1c49e-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="1c49e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c49e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c49e-105">Representa controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="1c49e-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="1c49e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c49e-106">Properties</span></span>

| <span data-ttu-id="1c49e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c49e-107">Property</span></span> | <span data-ttu-id="1c49e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c49e-108">Type</span></span> | <span data-ttu-id="1c49e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c49e-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="1c49e-110">operator</span><span class="sxs-lookup"><span data-stu-id="1c49e-110">operator</span></span> | <span data-ttu-id="1c49e-111">String</span><span class="sxs-lookup"><span data-stu-id="1c49e-111">String</span></span> | <span data-ttu-id="1c49e-112">Define a relação dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="1c49e-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="1c49e-113">Valores possíveis: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="1c49e-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="1c49e-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="1c49e-114">builtInControls</span></span> | <span data-ttu-id="1c49e-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c49e-115">String collection</span></span> | <span data-ttu-id="1c49e-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="1c49e-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="1c49e-117">Valores possíveis: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` .</span><span class="sxs-lookup"><span data-stu-id="1c49e-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="1c49e-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="1c49e-118">customAuthenticationFactors</span></span> | <span data-ttu-id="1c49e-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c49e-119">String collection</span></span> | <span data-ttu-id="1c49e-120">Lista de IDs de controles personalizados exigidas pela política.</span><span class="sxs-lookup"><span data-stu-id="1c49e-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="1c49e-121">Saiba mais sobre controles personalizados aqui: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="1c49e-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="1c49e-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="1c49e-122">termsOfUse</span></span> | <span data-ttu-id="1c49e-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c49e-123">String collection</span></span> | <span data-ttu-id="1c49e-124">Lista de [IDs de](agreement.md) termos de uso exigida pela política.</span><span class="sxs-lookup"><span data-stu-id="1c49e-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="1c49e-125">Considerações especiais ao usar `passwordChange` como um controle</span><span class="sxs-lookup"><span data-stu-id="1c49e-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="1c49e-126">Considere o seguinte ao usar o `passwordChange` controle:</span><span class="sxs-lookup"><span data-stu-id="1c49e-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="1c49e-127">`passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador.</span><span class="sxs-lookup"><span data-stu-id="1c49e-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="1c49e-128">Essa combinação garante que a senha seja atualizada de forma segura.</span><span class="sxs-lookup"><span data-stu-id="1c49e-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="1c49e-129">`passwordChange` deve ser usado em uma política que contém `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="1c49e-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="1c49e-130">Isso foi projetado para permitir cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.</span><span class="sxs-lookup"><span data-stu-id="1c49e-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="1c49e-131">A política deve direcionar `all` aplicativos e não excluir aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1c49e-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="1c49e-132">A política não pode conter nenhuma outra condição.</span><span class="sxs-lookup"><span data-stu-id="1c49e-132">The policy cannot contain any other condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="1c49e-133">Relações</span><span class="sxs-lookup"><span data-stu-id="1c49e-133">Relationships</span></span>

<span data-ttu-id="1c49e-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c49e-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c49e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c49e-135">JSON representation</span></span>

<span data-ttu-id="1c49e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c49e-136">The following is a JSON representation of the resource.</span></span>

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


