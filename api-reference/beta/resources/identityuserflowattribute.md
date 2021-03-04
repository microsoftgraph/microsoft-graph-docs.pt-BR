---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 3e8707627b09784972a1a578fe4b6b84a623f4dd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440238"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="adc81-103">tipo de recurso identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="adc81-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="adc81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adc81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adc81-105">Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD) e em um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="adc81-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="adc81-106">Configurar os atributos de fluxo de usuário no seu Azure AD ou no Azure AD B2C permite que você colete informações sobre um usuário durante a inscrição.</span><span class="sxs-lookup"><span data-stu-id="adc81-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="adc81-107">Você pode optar por coletar um conjunto de atributos interno. Por exemplo, o nome, o sobrenome, a cidade e o CEP.</span><span class="sxs-lookup"><span data-stu-id="adc81-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="adc81-108">Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório.</span><span class="sxs-lookup"><span data-stu-id="adc81-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="adc81-109">Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="adc81-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="adc81-110">Methods</span><span class="sxs-lookup"><span data-stu-id="adc81-110">Methods</span></span>

| <span data-ttu-id="adc81-111">Método</span><span class="sxs-lookup"><span data-stu-id="adc81-111">Method</span></span>       | <span data-ttu-id="adc81-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="adc81-112">Return Type</span></span>  |<span data-ttu-id="adc81-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="adc81-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="adc81-114">List</span><span class="sxs-lookup"><span data-stu-id="adc81-114">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="adc81-115">coleção identityUserFlowAttributes </span><span class="sxs-lookup"><span data-stu-id="adc81-115">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="adc81-116">Recuperar todos os atributos internos de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="adc81-116">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="adc81-117">Create</span><span class="sxs-lookup"><span data-stu-id="adc81-117">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="adc81-118">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="adc81-118">identityUserFlowAttribute</span></span>|<span data-ttu-id="adc81-119">Criar um novo atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="adc81-119">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="adc81-120">Get</span><span class="sxs-lookup"><span data-stu-id="adc81-120">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="adc81-121">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="adc81-121">identityUserFlowAttribute</span></span>|<span data-ttu-id="adc81-122">Recuperar as propriedades de um atributo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="adc81-122">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="adc81-123">Atualizar</span><span class="sxs-lookup"><span data-stu-id="adc81-123">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="adc81-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="adc81-124">None</span></span>|<span data-ttu-id="adc81-125">Atualizar um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="adc81-125">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="adc81-126">Delete</span><span class="sxs-lookup"><span data-stu-id="adc81-126">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="adc81-127">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="adc81-127">None</span></span>|<span data-ttu-id="adc81-128">Excluir um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="adc81-128">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="adc81-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="adc81-129">Properties</span></span>

|<span data-ttu-id="adc81-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adc81-130">Property</span></span>|<span data-ttu-id="adc81-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="adc81-131">Type</span></span>|<span data-ttu-id="adc81-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="adc81-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adc81-133">id</span><span class="sxs-lookup"><span data-stu-id="adc81-133">id</span></span>|<span data-ttu-id="adc81-134">String</span><span class="sxs-lookup"><span data-stu-id="adc81-134">String</span></span>|<span data-ttu-id="adc81-135">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="adc81-135">The identifier of the user flow attribute.</span></span> <span data-ttu-id="adc81-136">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="adc81-136">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="adc81-137">displayName</span><span class="sxs-lookup"><span data-stu-id="adc81-137">displayName</span></span>|<span data-ttu-id="adc81-138">String</span><span class="sxs-lookup"><span data-stu-id="adc81-138">String</span></span>|<span data-ttu-id="adc81-139">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="adc81-139">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="adc81-140">descrição</span><span class="sxs-lookup"><span data-stu-id="adc81-140">description</span></span>|<span data-ttu-id="adc81-141">String</span><span class="sxs-lookup"><span data-stu-id="adc81-141">String</span></span>|<span data-ttu-id="adc81-142">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="adc81-142">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="adc81-143">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="adc81-143">userFlowAttributeType</span></span>|<span data-ttu-id="adc81-144">String</span><span class="sxs-lookup"><span data-stu-id="adc81-144">String</span></span>|<span data-ttu-id="adc81-145">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="adc81-145">The type of the user flow attribute.</span></span> <span data-ttu-id="adc81-146">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="adc81-146">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="adc81-147">Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom`.</span><span class="sxs-lookup"><span data-stu-id="adc81-147">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="adc81-148">dataType</span><span class="sxs-lookup"><span data-stu-id="adc81-148">dataType</span></span>|<span data-ttu-id="adc81-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adc81-149">String</span></span>|<span data-ttu-id="adc81-150">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="adc81-150">The data type of the user flow attribute.</span></span> <span data-ttu-id="adc81-151">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="adc81-151">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="adc81-152">Os valores com suporte para **tipo de dados** são:</span><span class="sxs-lookup"><span data-stu-id="adc81-152">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="adc81-153">`string` -indica que o tipo de dados para identityUserFlowAttribute é uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="adc81-153">`string` - denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="adc81-154">`boolean` -indica que o tipo de dados para identityUserFlowAttribute é um booleano.</span><span class="sxs-lookup"><span data-stu-id="adc81-154">`boolean` - denotes that the dataType for the identityUserFlowAttribute is a Boolean.</span></span></li><li><span data-ttu-id="adc81-155">`int64` -indica que o tipo de dados para identityUserFlowAttribute é um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="adc81-155">`int64` - denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="json-representation"></a><span data-ttu-id="adc81-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="adc81-156">JSON representation</span></span>

<span data-ttu-id="adc81-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="adc81-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```json
{
    "@odata.type": "#microsoft.graph.identityUserFlowAttribute",
    "id": "String (identifier)",
    "displayName": "String",
    "description": "String",
    "userFlowAttributeType": "String",
    "dataType": "String"
}
```
