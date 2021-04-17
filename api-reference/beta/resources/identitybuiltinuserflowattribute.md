---
title: Tipo de recurso identityBuiltInUserFlowAttribute
description: Representa um atributo de fluxo de usuário integrado em locatários do Azure Active Directory que podem ser usados em fluxos de usuário de autoatendido.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e3d6c9eef25f428734214854d28a342f9c4f59dd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882645"
---
# <a name="identitybuiltinuserflowattribute-resource-type"></a><span data-ttu-id="8ccbb-103">Tipo de recurso identityBuiltInUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="8ccbb-103">identityBuiltInUserFlowAttribute resource type</span></span>

<span data-ttu-id="8ccbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ccbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ccbb-105">Representa um atributo de fluxo de usuário integrado em locatários do Azure Active Directory que podem ser usados em fluxos de usuário de autoatendido.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-105">Represents a built-in user flow attribute in Azure Active Directory tenants that can be used in your self-service sign-up user flows.</span></span> <span data-ttu-id="8ccbb-106">Esses atributos não podem ser modificados e são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="8ccbb-107">Herda de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="8ccbb-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8ccbb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ccbb-108">Properties</span></span>

|<span data-ttu-id="8ccbb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ccbb-109">Property</span></span>|<span data-ttu-id="8ccbb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ccbb-110">Type</span></span>|<span data-ttu-id="8ccbb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ccbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ccbb-112">id</span><span class="sxs-lookup"><span data-stu-id="8ccbb-112">id</span></span>|<span data-ttu-id="8ccbb-113">String</span><span class="sxs-lookup"><span data-stu-id="8ccbb-113">String</span></span>|<span data-ttu-id="8ccbb-114">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="8ccbb-115">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="8ccbb-116">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="8ccbb-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="8ccbb-117">displayName</span><span class="sxs-lookup"><span data-stu-id="8ccbb-117">displayName</span></span>|<span data-ttu-id="8ccbb-118">String</span><span class="sxs-lookup"><span data-stu-id="8ccbb-118">String</span></span>|<span data-ttu-id="8ccbb-119">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="8ccbb-120">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="8ccbb-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="8ccbb-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-121">Read-only.</span></span>|
|<span data-ttu-id="8ccbb-122">description</span><span class="sxs-lookup"><span data-stu-id="8ccbb-122">description</span></span>|<span data-ttu-id="8ccbb-123">String</span><span class="sxs-lookup"><span data-stu-id="8ccbb-123">String</span></span>|<span data-ttu-id="8ccbb-124">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-124">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="8ccbb-125">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="8ccbb-125">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="8ccbb-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-126">Read-only.</span></span>|
|<span data-ttu-id="8ccbb-127">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="8ccbb-127">userFlowAttributeType</span></span>|<span data-ttu-id="8ccbb-128">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="8ccbb-128">identityUserFlowAttributeType</span></span>|<span data-ttu-id="8ccbb-129">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-129">The type of the user flow attribute.</span></span> <span data-ttu-id="8ccbb-130">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-130">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="8ccbb-131">O valor dessa propriedade será `builtIn` .</span><span class="sxs-lookup"><span data-stu-id="8ccbb-131">The value for this property will be `builtIn`.</span></span> <span data-ttu-id="8ccbb-132">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="8ccbb-132">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="8ccbb-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-133">Read-only.</span></span>|
|<span data-ttu-id="8ccbb-134">dataType</span><span class="sxs-lookup"><span data-stu-id="8ccbb-134">dataType</span></span>|<span data-ttu-id="8ccbb-135">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="8ccbb-135">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="8ccbb-136">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-136">The data type of the user flow attribute.</span></span> <span data-ttu-id="8ccbb-137">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-137">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="8ccbb-138">Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-138">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="8ccbb-139">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="8ccbb-139">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="8ccbb-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ccbb-141">Relações</span><span class="sxs-lookup"><span data-stu-id="8ccbb-141">Relationships</span></span>

<span data-ttu-id="8ccbb-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ccbb-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ccbb-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ccbb-143">JSON representation</span></span>

<span data-ttu-id="8ccbb-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ccbb-144">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityBuiltInUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
