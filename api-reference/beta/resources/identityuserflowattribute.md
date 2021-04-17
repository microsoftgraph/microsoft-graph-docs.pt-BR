---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: ca8930a5cb11edb1cf7345464666478cfc01bcda
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882597"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="66917-103">tipo de recurso identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="66917-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="66917-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66917-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66917-105">Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD) e em um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="66917-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="66917-106">Configurar os atributos de fluxo de usuário no seu Azure AD ou no Azure AD B2C permite que você colete informações sobre um usuário durante a inscrição.</span><span class="sxs-lookup"><span data-stu-id="66917-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="66917-107">Você pode optar por coletar um conjunto de atributos interno. Por exemplo, o nome, o sobrenome, a cidade e o CEP.</span><span class="sxs-lookup"><span data-stu-id="66917-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="66917-108">Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório.</span><span class="sxs-lookup"><span data-stu-id="66917-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="66917-109">Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="66917-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

<span data-ttu-id="66917-110">[IdentityBuiltInUserFlowAttributes](../resources/identitybuiltinuserflowattribute.md) e [identityCustomUserFlowAttributes](../resources/identitycustomuserflowattribute.md) herdam desse tipo de base.</span><span class="sxs-lookup"><span data-stu-id="66917-110">[identityBuiltInUserFlowAttributes](../resources/identitybuiltinuserflowattribute.md) and [identityCustomUserFlowAttributes](../resources/identitycustomuserflowattribute.md) both inherit from this base type.</span></span>

## <a name="methods"></a><span data-ttu-id="66917-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="66917-111">Methods</span></span>

| <span data-ttu-id="66917-112">Método</span><span class="sxs-lookup"><span data-stu-id="66917-112">Method</span></span>       | <span data-ttu-id="66917-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66917-113">Return Type</span></span>  |<span data-ttu-id="66917-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="66917-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66917-115">List</span><span class="sxs-lookup"><span data-stu-id="66917-115">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="66917-116">coleção identityUserFlowAttributes </span><span class="sxs-lookup"><span data-stu-id="66917-116">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="66917-117">Recuperar todos os atributos internos de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="66917-117">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="66917-118">Create</span><span class="sxs-lookup"><span data-stu-id="66917-118">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="66917-119">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="66917-119">identityUserFlowAttribute</span></span>|<span data-ttu-id="66917-120">Criar um novo atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="66917-120">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="66917-121">Get</span><span class="sxs-lookup"><span data-stu-id="66917-121">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="66917-122">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="66917-122">identityUserFlowAttribute</span></span>|<span data-ttu-id="66917-123">Recuperar as propriedades de um atributo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="66917-123">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="66917-124">Atualizar</span><span class="sxs-lookup"><span data-stu-id="66917-124">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="66917-125">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="66917-125">None</span></span>|<span data-ttu-id="66917-126">Atualizar um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="66917-126">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="66917-127">Delete</span><span class="sxs-lookup"><span data-stu-id="66917-127">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="66917-128">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="66917-128">None</span></span>|<span data-ttu-id="66917-129">Excluir um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="66917-129">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="66917-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66917-130">Properties</span></span>

|<span data-ttu-id="66917-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66917-131">Property</span></span>|<span data-ttu-id="66917-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="66917-132">Type</span></span>|<span data-ttu-id="66917-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="66917-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66917-134">id</span><span class="sxs-lookup"><span data-stu-id="66917-134">id</span></span>|<span data-ttu-id="66917-135">String</span><span class="sxs-lookup"><span data-stu-id="66917-135">String</span></span>|<span data-ttu-id="66917-136">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="66917-136">The identifier of the user flow attribute.</span></span> <span data-ttu-id="66917-137">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="66917-137">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="66917-138">displayName</span><span class="sxs-lookup"><span data-stu-id="66917-138">displayName</span></span>|<span data-ttu-id="66917-139">String</span><span class="sxs-lookup"><span data-stu-id="66917-139">String</span></span>|<span data-ttu-id="66917-140">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="66917-140">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="66917-141">descrição</span><span class="sxs-lookup"><span data-stu-id="66917-141">description</span></span>|<span data-ttu-id="66917-142">String</span><span class="sxs-lookup"><span data-stu-id="66917-142">String</span></span>|<span data-ttu-id="66917-143">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="66917-143">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="66917-144">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="66917-144">userFlowAttributeType</span></span>|<span data-ttu-id="66917-145">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="66917-145">identityUserFlowAttributeType</span></span>|<span data-ttu-id="66917-146">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="66917-146">The type of the user flow attribute.</span></span> <span data-ttu-id="66917-147">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="66917-147">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="66917-148">Dependendo do tipo de atributo, os valores desta propriedade serão `builtIn`, `custom` ou `required`.</span><span class="sxs-lookup"><span data-stu-id="66917-148">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="66917-149">dataType</span><span class="sxs-lookup"><span data-stu-id="66917-149">dataType</span></span>|<span data-ttu-id="66917-150">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="66917-150">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="66917-151">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="66917-151">The data type of the user flow attribute.</span></span> <span data-ttu-id="66917-152">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="66917-152">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="66917-153">Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="66917-153">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66917-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66917-154">JSON representation</span></span>

<span data-ttu-id="66917-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66917-155">The following is a JSON representation of the resource.</span></span>

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
