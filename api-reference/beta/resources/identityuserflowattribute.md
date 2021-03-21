---
title: tipo de recurso identityUserFlowAttribute
description: Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory e em um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 8262d8c77d31abbd25aaaae26018c651f0dcfbe5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957006"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="d8318-103">tipo de recurso identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="d8318-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="d8318-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8318-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8318-105">Representa os atributos de fluxo de usuário em um locatário do Azure Active Directory (Azure AD) e em um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="d8318-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="d8318-106">Configurar os atributos de fluxo de usuário no seu Azure AD ou no Azure AD B2C permite que você colete informações sobre um usuário durante a inscrição.</span><span class="sxs-lookup"><span data-stu-id="d8318-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="d8318-107">Você pode optar por coletar um conjunto de atributos interno. Por exemplo, o nome, o sobrenome, a cidade e o CEP.</span><span class="sxs-lookup"><span data-stu-id="d8318-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="d8318-108">Você também pode configurar atributos de fluxo de usuário personalizado para coletar informações de um usuário que não está integrado ao diretório.</span><span class="sxs-lookup"><span data-stu-id="d8318-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="d8318-109">Os atributos de fluxo de usuário personalizado são uma abstração das [extensões de esquema do Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="d8318-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="d8318-110">Methods</span><span class="sxs-lookup"><span data-stu-id="d8318-110">Methods</span></span>

| <span data-ttu-id="d8318-111">Método</span><span class="sxs-lookup"><span data-stu-id="d8318-111">Method</span></span>       | <span data-ttu-id="d8318-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8318-112">Return Type</span></span>  |<span data-ttu-id="d8318-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8318-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8318-114">List</span><span class="sxs-lookup"><span data-stu-id="d8318-114">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="d8318-115">coleção identityUserFlowAttributes </span><span class="sxs-lookup"><span data-stu-id="d8318-115">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="d8318-116">Recuperar todos os atributos internos de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="d8318-116">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="d8318-117">Create</span><span class="sxs-lookup"><span data-stu-id="d8318-117">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="d8318-118">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="d8318-118">identityUserFlowAttribute</span></span>|<span data-ttu-id="d8318-119">Criar um novo atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="d8318-119">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="d8318-120">Get</span><span class="sxs-lookup"><span data-stu-id="d8318-120">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="d8318-121">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="d8318-121">identityUserFlowAttribute</span></span>|<span data-ttu-id="d8318-122">Recuperar as propriedades de um atributo de fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="d8318-122">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="d8318-123">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d8318-123">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="d8318-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="d8318-124">None</span></span>|<span data-ttu-id="d8318-125">Atualizar um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="d8318-125">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="d8318-126">Delete</span><span class="sxs-lookup"><span data-stu-id="d8318-126">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="d8318-127">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="d8318-127">None</span></span>|<span data-ttu-id="d8318-128">Excluir um atributo de fluxo de usuário personalizado.</span><span class="sxs-lookup"><span data-stu-id="d8318-128">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8318-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8318-129">Properties</span></span>

|<span data-ttu-id="d8318-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8318-130">Property</span></span>|<span data-ttu-id="d8318-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8318-131">Type</span></span>|<span data-ttu-id="d8318-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8318-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8318-133">id</span><span class="sxs-lookup"><span data-stu-id="d8318-133">id</span></span>|<span data-ttu-id="d8318-134">String</span><span class="sxs-lookup"><span data-stu-id="d8318-134">String</span></span>|<span data-ttu-id="d8318-135">O identificador do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8318-135">The identifier of the user flow attribute.</span></span> <span data-ttu-id="d8318-136">Esse é um atributo somente leitura criado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d8318-136">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="d8318-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d8318-137">displayName</span></span>|<span data-ttu-id="d8318-138">String</span><span class="sxs-lookup"><span data-stu-id="d8318-138">String</span></span>|<span data-ttu-id="d8318-139">O nome de exibição do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8318-139">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="d8318-140">descrição</span><span class="sxs-lookup"><span data-stu-id="d8318-140">description</span></span>|<span data-ttu-id="d8318-141">String</span><span class="sxs-lookup"><span data-stu-id="d8318-141">String</span></span>|<span data-ttu-id="d8318-142">A descrição do atributo de fluxo de usuário exibido para o usuário no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="d8318-142">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="d8318-143">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="d8318-143">userFlowAttributeType</span></span>|<span data-ttu-id="d8318-144">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="d8318-144">identityUserFlowAttributeType</span></span>|<span data-ttu-id="d8318-145">O tipo do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8318-145">The type of the user flow attribute.</span></span> <span data-ttu-id="d8318-146">Esse é um atributo somente leitura que é definido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d8318-146">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="d8318-147">Dependendo do tipo de atributo, os valores desta propriedade serão `builtIn`, `custom` ou `required`.</span><span class="sxs-lookup"><span data-stu-id="d8318-147">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="d8318-148">dataType</span><span class="sxs-lookup"><span data-stu-id="d8318-148">dataType</span></span>|<span data-ttu-id="d8318-149">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="d8318-149">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="d8318-150">O tipo de dados do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8318-150">The data type of the user flow attribute.</span></span> <span data-ttu-id="d8318-151">Isso não pode ser modificado após o atributo de fluxo de usuário personalizado ser criado.</span><span class="sxs-lookup"><span data-stu-id="d8318-151">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="d8318-152">Os valores suportados para **dataType** são: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="d8318-152">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8318-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8318-153">JSON representation</span></span>

<span data-ttu-id="d8318-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8318-154">The following is a JSON representation of the resource.</span></span>

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
