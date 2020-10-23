---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: f5166cafff64a7050b89bbd7f70cba66f429646d
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742353"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="166b8-103">tipo de recurso identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="166b8-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="166b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="166b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="166b8-105">Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD) e em um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="166b8-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="166b8-106">Configurar os atributos de fluxo de usuário no seu Azure AD ou no Azure AD B2C permite que você colete informações sobre um usuário durante a inscrição.</span><span class="sxs-lookup"><span data-stu-id="166b8-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="166b8-107">Você pode optar por coletar um conjunto de atributos interno. Por exemplo, o nome, o sobrenome, a cidade e o CEP.</span><span class="sxs-lookup"><span data-stu-id="166b8-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="166b8-108">Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório.</span><span class="sxs-lookup"><span data-stu-id="166b8-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="166b8-109">Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="166b8-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="166b8-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="166b8-110">Methods</span></span>

| <span data-ttu-id="166b8-111">Método</span><span class="sxs-lookup"><span data-stu-id="166b8-111">Method</span></span>       | <span data-ttu-id="166b8-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="166b8-112">Return Type</span></span>  |<span data-ttu-id="166b8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="166b8-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="166b8-114">Lista</span><span class="sxs-lookup"><span data-stu-id="166b8-114">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="166b8-115">coleção identityUserFlowAttributes </span><span class="sxs-lookup"><span data-stu-id="166b8-115">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="166b8-116">Recuperar todos os atributos internos de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="166b8-116">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="166b8-117">Create</span><span class="sxs-lookup"><span data-stu-id="166b8-117">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="166b8-118">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="166b8-118">identityUserFlowAttribute</span></span>|<span data-ttu-id="166b8-119">Criar um novo atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="166b8-119">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="166b8-120">Get</span><span class="sxs-lookup"><span data-stu-id="166b8-120">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="166b8-121">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="166b8-121">identityUserFlowAttribute</span></span>|<span data-ttu-id="166b8-122">Recuperar as propriedades de um atributo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="166b8-122">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="166b8-123">Atualizar</span><span class="sxs-lookup"><span data-stu-id="166b8-123">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="166b8-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="166b8-124">None</span></span>|<span data-ttu-id="166b8-125">Atualizar um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="166b8-125">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="166b8-126">Excluir</span><span class="sxs-lookup"><span data-stu-id="166b8-126">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="166b8-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="166b8-127">None</span></span>|<span data-ttu-id="166b8-128">Excluir um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="166b8-128">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="166b8-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="166b8-129">Properties</span></span>

|<span data-ttu-id="166b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="166b8-130">Property</span></span>|<span data-ttu-id="166b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="166b8-131">Type</span></span>|<span data-ttu-id="166b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="166b8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="166b8-133">id</span><span class="sxs-lookup"><span data-stu-id="166b8-133">id</span></span>|<span data-ttu-id="166b8-134">String</span><span class="sxs-lookup"><span data-stu-id="166b8-134">String</span></span>|<span data-ttu-id="166b8-135">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="166b8-135">The identifier of the user flow attribute.</span></span> <span data-ttu-id="166b8-136">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="166b8-136">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="166b8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="166b8-137">displayName</span></span>|<span data-ttu-id="166b8-138">String</span><span class="sxs-lookup"><span data-stu-id="166b8-138">String</span></span>|<span data-ttu-id="166b8-139">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="166b8-139">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="166b8-140">description</span><span class="sxs-lookup"><span data-stu-id="166b8-140">description</span></span>|<span data-ttu-id="166b8-141">String</span><span class="sxs-lookup"><span data-stu-id="166b8-141">String</span></span>|<span data-ttu-id="166b8-142">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="166b8-142">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="166b8-143">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="166b8-143">userFlowAttributeType</span></span>|<span data-ttu-id="166b8-144">String</span><span class="sxs-lookup"><span data-stu-id="166b8-144">String</span></span>|<span data-ttu-id="166b8-145">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="166b8-145">The type of the user flow attribute.</span></span> <span data-ttu-id="166b8-146">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="166b8-146">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="166b8-147">Dependendo do tipo de atributo, os valores dessa propriedade serão `builtIn` ou `custom`.</span><span class="sxs-lookup"><span data-stu-id="166b8-147">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="166b8-148">dataType</span><span class="sxs-lookup"><span data-stu-id="166b8-148">dataType</span></span>|<span data-ttu-id="166b8-149">String</span><span class="sxs-lookup"><span data-stu-id="166b8-149">String</span></span>|<span data-ttu-id="166b8-150">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="166b8-150">The data type of the user flow attribute.</span></span> <span data-ttu-id="166b8-151">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="166b8-151">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="166b8-152">Os valores com suporte para **tipo de dados** são:</span><span class="sxs-lookup"><span data-stu-id="166b8-152">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="166b8-153">`string` -indica que o tipo de dados para identityUserFlowAttribute é uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="166b8-153">`string` - denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="166b8-154">`boolean` -indica que o tipo de dados para identityUserFlowAttribute é um booleano.</span><span class="sxs-lookup"><span data-stu-id="166b8-154">`boolean` - denotes that the dataType for the identityUserFlowAttribute is a Boolean.</span></span></li><li><span data-ttu-id="166b8-155">`int64` -indica que o tipo de dados para identityUserFlowAttribute é um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="166b8-155">`int64` - denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="json-representation"></a><span data-ttu-id="166b8-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="166b8-156">JSON representation</span></span>

<span data-ttu-id="166b8-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="166b8-157">The following is a JSON representation of the resource.</span></span>

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
