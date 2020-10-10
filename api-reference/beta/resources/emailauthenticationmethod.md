---
title: tipo de recurso emailAuthenticationMethod
description: Uma representação de um endereço de email registrado para um usuário. O email é um método de autenticação disponível somente para redefinição de senha de autoatendimento (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6dde3c9a859f2527241b66c0172d6b5dd877aac4
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418193"
---
# <a name="emailauthenticationmethod-resource-type"></a><span data-ttu-id="32aee-104">tipo de recurso emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="32aee-104">emailAuthenticationMethod resource type</span></span>

<span data-ttu-id="32aee-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32aee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32aee-106">Uma representação de um endereço de email registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-106">A representation of an email address registered to a user.</span></span> <span data-ttu-id="32aee-107">O email é um método de autenticação disponível somente para redefinição de senha de autoatendimento (SSPR).</span><span class="sxs-lookup"><span data-stu-id="32aee-107">Email is an authentication method available only to self-service password reset (SSPR).</span></span> <span data-ttu-id="32aee-108">Os usuários podem ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="32aee-108">Users may only have one email authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="32aee-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="32aee-109">Methods</span></span>
|<span data-ttu-id="32aee-110">Método</span><span class="sxs-lookup"><span data-stu-id="32aee-110">Method</span></span>|<span data-ttu-id="32aee-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="32aee-111">Return type</span></span>|<span data-ttu-id="32aee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="32aee-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32aee-113">List</span><span class="sxs-lookup"><span data-stu-id="32aee-113">List</span></span>](../api/emailauthenticationmethod-list.md)|<span data-ttu-id="32aee-114">coleção [emailAuthenticationMethod](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="32aee-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span></span>|<span data-ttu-id="32aee-115">Recupere uma lista de emailAuthenticationMethods de um usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-115">Retrieve a list of a user's emailAuthenticationMethods.</span></span> <span data-ttu-id="32aee-116">Os usuários podem ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="32aee-116">Users may only have one email authentication method.</span></span>|
|[<span data-ttu-id="32aee-117">Criar</span><span class="sxs-lookup"><span data-stu-id="32aee-117">Create</span></span>](../api/emailauthenticationmethod-post.md)|[<span data-ttu-id="32aee-118">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="32aee-118">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="32aee-119">Criar um objeto emailMethods de um usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-119">Create a user's emailMethods object.</span></span>|
|[<span data-ttu-id="32aee-120">Obter</span><span class="sxs-lookup"><span data-stu-id="32aee-120">Get</span></span>](../api/emailauthenticationmethod-get.md)|[<span data-ttu-id="32aee-121">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="32aee-121">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="32aee-122">Recupere as propriedades do objeto emailAuthenticationMethod do usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-122">Retrieve the properties  of the user's emailAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="32aee-123">Atualizar</span><span class="sxs-lookup"><span data-stu-id="32aee-123">Update</span></span>](../api/emailauthenticationmethod-update.md)|[<span data-ttu-id="32aee-124">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="32aee-124">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="32aee-125">Atualiza as propriedades do objeto emailMethods de um usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-125">Update the properties of a user's emailMethods object.</span></span>|
|[<span data-ttu-id="32aee-126">Excluir</span><span class="sxs-lookup"><span data-stu-id="32aee-126">Delete</span></span>](../api/emailauthenticationmethod-delete.md)|<span data-ttu-id="32aee-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32aee-127">None</span></span>|<span data-ttu-id="32aee-128">Exclua o objeto emailAuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-128">Delete a user's emailAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="32aee-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32aee-129">Properties</span></span>
|<span data-ttu-id="32aee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32aee-130">Property</span></span>|<span data-ttu-id="32aee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32aee-131">Type</span></span>|<span data-ttu-id="32aee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32aee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32aee-133">id</span><span class="sxs-lookup"><span data-stu-id="32aee-133">id</span></span>|<span data-ttu-id="32aee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32aee-134">String</span></span>|<span data-ttu-id="32aee-135">O identificador do endereço de email registrado para este usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-135">The identifier of the email address registered to this user.</span></span>|
|<span data-ttu-id="32aee-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="32aee-136">emailAddress</span></span>|<span data-ttu-id="32aee-137">String</span><span class="sxs-lookup"><span data-stu-id="32aee-137">String</span></span>|<span data-ttu-id="32aee-138">O endereço de email registrado para este usuário.</span><span class="sxs-lookup"><span data-stu-id="32aee-138">The email address registered to this user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32aee-139">Relações</span><span class="sxs-lookup"><span data-stu-id="32aee-139">Relationships</span></span>
<span data-ttu-id="32aee-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32aee-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32aee-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32aee-141">JSON representation</span></span>
<span data-ttu-id="32aee-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32aee-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

