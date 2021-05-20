---
title: Tipo de recurso authenticationContextClassReference
description: Representa uma Azure Active Directory de classe de contexto de autenticação.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1397545d7b102d05b8c71957cea88f9c131f0e09
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547351"
---
# <a name="authenticationcontextclassreference-resource-type"></a><span data-ttu-id="3f81d-103">Tipo de recurso authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-103">authenticationContextClassReference resource type</span></span>

<span data-ttu-id="3f81d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f81d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f81d-105">Representa uma Azure Active Directory de classe de contexto de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3f81d-105">Represents an Azure Active Directory authentication context class reference.</span></span> <span data-ttu-id="3f81d-106">Referências de classe de contexto de autenticação são valores personalizados que definem um requisito de autenticação de Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="3f81d-106">Authentication context class references are custom values that define a Conditional Access authentication requirement.</span></span>

## <a name="methods"></a><span data-ttu-id="3f81d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3f81d-107">Methods</span></span>

| <span data-ttu-id="3f81d-108">Método</span><span class="sxs-lookup"><span data-stu-id="3f81d-108">Method</span></span>       | <span data-ttu-id="3f81d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3f81d-109">Return Type</span></span> | <span data-ttu-id="3f81d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f81d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3f81d-111">Listar authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-111">List authenticationContextClassReference</span></span>](../api/conditionalaccessroot-list-authenticationcontextclassreferences.md) | <span data-ttu-id="3f81d-112">[Coleção authenticationContextClassReference](authenticationContextClassReference.md)</span><span class="sxs-lookup"><span data-stu-id="3f81d-112">[authenticationContextClassReference](authenticationContextClassReference.md) collection</span></span> | <span data-ttu-id="3f81d-113">Obter todos os objetos authenticationContextClassReference na organização.</span><span class="sxs-lookup"><span data-stu-id="3f81d-113">Get all of the authenticationContextClassReference objects in the organization.</span></span> |
| [<span data-ttu-id="3f81d-114">Criar authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-114">Create authenticationContextClassReference</span></span>](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md) | [<span data-ttu-id="3f81d-115">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-115">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="3f81d-116">Crie um novo objeto authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="3f81d-116">Create a new authenticationContextClassReference object.</span></span> |
| [<span data-ttu-id="3f81d-117">Obter authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-117">Get authenticationContextClassReference</span></span>](../api/authenticationcontextclassreference-get.md) | [<span data-ttu-id="3f81d-118">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-118">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="3f81d-119">Ler propriedades e relações de um objeto authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="3f81d-119">Read properties and relationships of a authenticationContextClassReference object.</span></span> |
| [<span data-ttu-id="3f81d-120">Atualizar authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-120">Update authenticationContextClassReference</span></span>](../api/authenticationcontextclassreference-update.md) | [<span data-ttu-id="3f81d-121">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="3f81d-121">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="3f81d-122">Atualize um objeto authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="3f81d-122">Update a authenticationContextClassReference object.</span></span> |


## <a name="properties"></a><span data-ttu-id="3f81d-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f81d-123">Properties</span></span>

| <span data-ttu-id="3f81d-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f81d-124">Property</span></span>     | <span data-ttu-id="3f81d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f81d-125">Type</span></span>        | <span data-ttu-id="3f81d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f81d-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3f81d-127">id</span><span class="sxs-lookup"><span data-stu-id="3f81d-127">id</span></span>|<span data-ttu-id="3f81d-128">String</span><span class="sxs-lookup"><span data-stu-id="3f81d-128">String</span></span>| <span data-ttu-id="3f81d-129">Identificador usado para fazer referência à classe de contexto de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3f81d-129">Identifier used to reference the authentication context class.</span></span> <span data-ttu-id="3f81d-130">A id é usada para disparar a autenticação de etapa para os requisitos de autenticação referenciados e é o valor que será emitido na declaração do acrs.</span><span class="sxs-lookup"><span data-stu-id="3f81d-130">The id is used to trigger step-up authentication for the referenced authentication requirements and is the value that will be issued in the acrs claim.</span></span> <span data-ttu-id="3f81d-131">Esse valor na declaração é usado para verificar se o contexto de autenticação necessário foi satisfeito.</span><span class="sxs-lookup"><span data-stu-id="3f81d-131">This value in the claim is used to verify the required authentication context has been satisfied.</span></span> <span data-ttu-id="3f81d-132">Os valores de id permitidos são "c1" até "c25".</span><span class="sxs-lookup"><span data-stu-id="3f81d-132">The allowed id values are "c1" through "c25".</span></span> |
|<span data-ttu-id="3f81d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3f81d-133">displayName</span></span>|<span data-ttu-id="3f81d-134">String</span><span class="sxs-lookup"><span data-stu-id="3f81d-134">String</span></span>| <span data-ttu-id="3f81d-135">O nome para exibição é o nome amigável da authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="3f81d-135">The display name is the friendly name of the authenticationContextClassReference.</span></span> <span data-ttu-id="3f81d-136">Esse valor deve ser usado para identificar a referência de classe de contexto de autenticação ao criar experiências de administrador voltadas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3f81d-136">This value should be used to identify the authentication context class reference when building user facing admin experiences.</span></span> <span data-ttu-id="3f81d-137">Por exemplo, UX de seleção.</span><span class="sxs-lookup"><span data-stu-id="3f81d-137">For example, selection UX.</span></span> |
|<span data-ttu-id="3f81d-138">descrição</span><span class="sxs-lookup"><span data-stu-id="3f81d-138">description</span></span>|<span data-ttu-id="3f81d-139">String</span><span class="sxs-lookup"><span data-stu-id="3f81d-139">String</span></span>| <span data-ttu-id="3f81d-140">Uma breve explicação das políticas impostas pela authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="3f81d-140">A short explanation of the policies that are enforced by authenticationContextClassReference.</span></span> <span data-ttu-id="3f81d-141">Esse valor deve ser usado para fornecer texto secundário para descrever a referência de classe de contexto de autenticação ao criar experiências de administrador voltadas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3f81d-141">This value should be used to provide secondary text to describe the authentication context class reference when building user facing admin experiences.</span></span> <span data-ttu-id="3f81d-142">Por exemplo, UX de seleção.</span><span class="sxs-lookup"><span data-stu-id="3f81d-142">For example, selection UX.</span></span>|
|<span data-ttu-id="3f81d-143">isAvailable</span><span class="sxs-lookup"><span data-stu-id="3f81d-143">isAvailable</span></span>|<span data-ttu-id="3f81d-144">booliano</span><span class="sxs-lookup"><span data-stu-id="3f81d-144">boolean</span></span>| <span data-ttu-id="3f81d-145">Indica se a authenticationContextClassReference foi publicada pelo administrador de segurança e está pronta para uso pelos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3f81d-145">Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps.</span></span> <span data-ttu-id="3f81d-146">Quando estiver definido para ele, não deverá ser mostrado nas experiências de UX do administrador, pois o valor não está disponível no momento `false` para seleção.</span><span class="sxs-lookup"><span data-stu-id="3f81d-146">When it is set to `false` it should not be shown in admin UX experiences because the value is not currently available for selection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f81d-147">Relações</span><span class="sxs-lookup"><span data-stu-id="3f81d-147">Relationships</span></span>

<span data-ttu-id="3f81d-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f81d-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f81d-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f81d-149">JSON representation</span></span>

<span data-ttu-id="3f81d-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f81d-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
    {
      "id": "String",
      "displayName": "String",
      "description": "String",
      "isAvailable": "boolean",
    }

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationContextClassReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
