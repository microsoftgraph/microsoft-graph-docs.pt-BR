---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: af3ec2a762fc0252da929d863917ba6cd274ba95
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882783"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="7b6e5-103">tipo de recurso identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="7b6e5-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="7b6e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b6e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b6e5-105">Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7b6e5-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant.</span></span>

<span data-ttu-id="7b6e5-106">Configurar os atributos de fluxo de usuário no seu locatário do Azure AD permite que você colete informações sobre um usuário durante a inscrição.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-106">Configuring user flow attributes in your Azure AD tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="7b6e5-107">Você pode escolher coletar um conjunto interno de atributos.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-107">You can choose to collect a built-in set of attributes.</span></span> <span data-ttu-id="7b6e5-108">Por exemplo, nome, sobrenome, cidade e CEP.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-108">For example, given name, surname, city, and postal code.</span></span> <span data-ttu-id="7b6e5-109">Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-109">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="7b6e5-110">Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="7b6e5-110">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="7b6e5-111">Methods</span><span class="sxs-lookup"><span data-stu-id="7b6e5-111">Methods</span></span>

| <span data-ttu-id="7b6e5-112">Método</span><span class="sxs-lookup"><span data-stu-id="7b6e5-112">Method</span></span>       | <span data-ttu-id="7b6e5-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b6e5-113">Return Type</span></span>  |<span data-ttu-id="7b6e5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b6e5-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b6e5-115">List</span><span class="sxs-lookup"><span data-stu-id="7b6e5-115">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="7b6e5-116">coleção identityUserFlowAttributes </span><span class="sxs-lookup"><span data-stu-id="7b6e5-116">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="7b6e5-117">Recuperar todos os atributos internos de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-117">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="7b6e5-118">Create</span><span class="sxs-lookup"><span data-stu-id="7b6e5-118">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="7b6e5-119">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="7b6e5-119">identityUserFlowAttribute</span></span>|<span data-ttu-id="7b6e5-120">Criar um novo atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-120">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="7b6e5-121">Get</span><span class="sxs-lookup"><span data-stu-id="7b6e5-121">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="7b6e5-122">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="7b6e5-122">identityUserFlowAttribute</span></span>|<span data-ttu-id="7b6e5-123">Recuperar as propriedades de um atributo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-123">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="7b6e5-124">Atualizar</span><span class="sxs-lookup"><span data-stu-id="7b6e5-124">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="7b6e5-125">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="7b6e5-125">None</span></span>|<span data-ttu-id="7b6e5-126">Atualizar um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-126">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="7b6e5-127">Delete</span><span class="sxs-lookup"><span data-stu-id="7b6e5-127">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="7b6e5-128">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="7b6e5-128">None</span></span>|<span data-ttu-id="7b6e5-129">Excluir um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-129">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b6e5-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b6e5-130">Properties</span></span>

|<span data-ttu-id="7b6e5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b6e5-131">Property</span></span>|<span data-ttu-id="7b6e5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b6e5-132">Type</span></span>|<span data-ttu-id="7b6e5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b6e5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b6e5-134">id</span><span class="sxs-lookup"><span data-stu-id="7b6e5-134">id</span></span>|<span data-ttu-id="7b6e5-135">String</span><span class="sxs-lookup"><span data-stu-id="7b6e5-135">String</span></span>|<span data-ttu-id="7b6e5-136">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-136">The identifier of the user flow attribute.</span></span> <span data-ttu-id="7b6e5-137">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-137">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="7b6e5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7b6e5-138">displayName</span></span>|<span data-ttu-id="7b6e5-139">String</span><span class="sxs-lookup"><span data-stu-id="7b6e5-139">String</span></span>|<span data-ttu-id="7b6e5-140">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-140">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="7b6e5-141">descrição</span><span class="sxs-lookup"><span data-stu-id="7b6e5-141">description</span></span>|<span data-ttu-id="7b6e5-142">String</span><span class="sxs-lookup"><span data-stu-id="7b6e5-142">String</span></span>|<span data-ttu-id="7b6e5-143">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-143">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="7b6e5-144">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="7b6e5-144">userFlowAttributeType</span></span>|<span data-ttu-id="7b6e5-145">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="7b6e5-145">identityUserFlowAttributeType</span></span>|<span data-ttu-id="7b6e5-146">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-146">The type of the user flow attribute.</span></span> <span data-ttu-id="7b6e5-147">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-147">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="7b6e5-148">Dependendo do tipo de atributo, os valores desta propriedade serão `builtIn`, `custom` ou `required`.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-148">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="7b6e5-149">dataType</span><span class="sxs-lookup"><span data-stu-id="7b6e5-149">dataType</span></span>|<span data-ttu-id="7b6e5-150">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="7b6e5-150">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="7b6e5-151">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-151">The data type of the user flow attribute.</span></span> <span data-ttu-id="7b6e5-152">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-152">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="7b6e5-153">Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-153">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b6e5-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b6e5-154">JSON representation</span></span>

<span data-ttu-id="7b6e5-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b6e5-155">The following is a JSON representation of the resource.</span></span>

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
