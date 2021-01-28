---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0b93508db666fc1673f1c8154ef638762a872f3
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013664"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="b485f-103">Tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="b485f-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="b485f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b485f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b485f-105">Representa controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="b485f-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b485f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b485f-106">Properties</span></span>

| <span data-ttu-id="b485f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b485f-107">Property</span></span> | <span data-ttu-id="b485f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b485f-108">Type</span></span> | <span data-ttu-id="b485f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b485f-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="b485f-110">operator</span><span class="sxs-lookup"><span data-stu-id="b485f-110">operator</span></span> | <span data-ttu-id="b485f-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b485f-111">String</span></span> | <span data-ttu-id="b485f-112">Define a relação dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="b485f-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="b485f-113">Valores possíveis: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="b485f-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="b485f-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="b485f-114">builtInControls</span></span> | <span data-ttu-id="b485f-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b485f-115">String collection</span></span> | <span data-ttu-id="b485f-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="b485f-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="b485f-117">Valores possíveis: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` .</span><span class="sxs-lookup"><span data-stu-id="b485f-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="b485f-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="b485f-118">customAuthenticationFactors</span></span> | <span data-ttu-id="b485f-119">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b485f-119">String collection</span></span> | <span data-ttu-id="b485f-120">Lista de IDs de controles personalizados exigidas pela política.</span><span class="sxs-lookup"><span data-stu-id="b485f-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="b485f-121">Para obter mais informações, consulte [Controles personalizados.](/azure/active-directory/conditional-access/controls)</span><span class="sxs-lookup"><span data-stu-id="b485f-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="b485f-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="b485f-122">termsOfUse</span></span> | <span data-ttu-id="b485f-123">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b485f-123">String collection</span></span> | <span data-ttu-id="b485f-124">Lista de [IDs de termos](/graph/api/resources/agreement) de uso exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="b485f-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="b485f-125">Considerações especiais ao usar `passwordChange` como um controle</span><span class="sxs-lookup"><span data-stu-id="b485f-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="b485f-126">Considere o seguinte ao usar o `passwordChange` controle:</span><span class="sxs-lookup"><span data-stu-id="b485f-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="b485f-127">`passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador.</span><span class="sxs-lookup"><span data-stu-id="b485f-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="b485f-128">Essa combinação garante que a senha seja atualizada de forma segura.</span><span class="sxs-lookup"><span data-stu-id="b485f-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="b485f-129">`passwordChange` deve ser usado em uma política que contém `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="b485f-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="b485f-130">Isso foi projetado para permitir cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.</span><span class="sxs-lookup"><span data-stu-id="b485f-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="b485f-131">A política deve direcionar `all` aplicativos e não excluir aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b485f-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="b485f-132">A política não pode conter nenhuma outra condição, exceto `users` e `applications` `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="b485f-132">The policy cannot contain any other condition except `users`, `applications` and `userRiskLevels`.</span></span>

## <a name="relationships"></a><span data-ttu-id="b485f-133">Relações</span><span class="sxs-lookup"><span data-stu-id="b485f-133">Relationships</span></span>

<span data-ttu-id="b485f-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b485f-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b485f-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b485f-135">JSON representation</span></span>

<span data-ttu-id="b485f-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b485f-136">The following is a JSON representation of the resource.</span></span>

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