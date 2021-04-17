---
title: Tipo de recurso identityCustomUserFlowAttribute
description: Representa um atributo de fluxo de usuário personalizado em locatários do Azure Active Directory que podem ser usados em fluxos de usuário de autoatenduro.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a07ea64be3cf5a215c43271982b7fdfce3f6662
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882644"
---
# <a name="identitycustomuserflowattribute-resource-type"></a><span data-ttu-id="26700-103">Tipo de recurso identityCustomUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="26700-103">identityCustomUserFlowAttribute resource type</span></span>

<span data-ttu-id="26700-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26700-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26700-105">Representa um atributo de fluxo de usuário personalizado em locatários do Azure Active Directory que podem ser usados em fluxos de usuário de autoatenduro.</span><span class="sxs-lookup"><span data-stu-id="26700-105">Represents a custom user flow attribute in Azure Active Directory tenants that can be used in your self-service sign-up user flows.</span></span> <span data-ttu-id="26700-106">Esses atributos não podem ser modificados e são somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26700-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="26700-107">Herda de [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="26700-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="26700-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26700-108">Properties</span></span>

|<span data-ttu-id="26700-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26700-109">Property</span></span>|<span data-ttu-id="26700-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26700-110">Type</span></span>|<span data-ttu-id="26700-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26700-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26700-112">id</span><span class="sxs-lookup"><span data-stu-id="26700-112">id</span></span>|<span data-ttu-id="26700-113">String</span><span class="sxs-lookup"><span data-stu-id="26700-113">String</span></span>|<span data-ttu-id="26700-114">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="26700-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="26700-115">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="26700-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="26700-116">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="26700-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="26700-117">displayName</span><span class="sxs-lookup"><span data-stu-id="26700-117">displayName</span></span>|<span data-ttu-id="26700-118">String</span><span class="sxs-lookup"><span data-stu-id="26700-118">String</span></span>|<span data-ttu-id="26700-119">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="26700-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="26700-120">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="26700-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="26700-121">description</span><span class="sxs-lookup"><span data-stu-id="26700-121">description</span></span>|<span data-ttu-id="26700-122">String</span><span class="sxs-lookup"><span data-stu-id="26700-122">String</span></span>|<span data-ttu-id="26700-123">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="26700-123">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="26700-124">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="26700-124">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="26700-125">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="26700-125">userFlowAttributeType</span></span>|<span data-ttu-id="26700-126">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="26700-126">identityUserFlowAttributeType</span></span>|<span data-ttu-id="26700-127">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="26700-127">The type of the user flow attribute.</span></span> <span data-ttu-id="26700-128">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="26700-128">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="26700-129">O valor dessa propriedade será `custom` .</span><span class="sxs-lookup"><span data-stu-id="26700-129">The value for this property will be `custom`.</span></span> <span data-ttu-id="26700-130">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="26700-130">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>|
|<span data-ttu-id="26700-131">dataType</span><span class="sxs-lookup"><span data-stu-id="26700-131">dataType</span></span>|<span data-ttu-id="26700-132">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="26700-132">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="26700-133">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="26700-133">The data type of the user flow attribute.</span></span> <span data-ttu-id="26700-134">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="26700-134">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="26700-135">Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="26700-135">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="26700-136">Herdado [de identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="26700-136">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="26700-137">Relações</span><span class="sxs-lookup"><span data-stu-id="26700-137">Relationships</span></span>

<span data-ttu-id="26700-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26700-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26700-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26700-139">JSON representation</span></span>

<span data-ttu-id="26700-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26700-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityCustomUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityCustomUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
