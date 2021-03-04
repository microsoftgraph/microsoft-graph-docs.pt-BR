---
title: Tipo de recurso emailAuthenticationMethod
description: Uma representação de um endereço de email registrado para um usuário. O email é um método de autenticação disponível apenas para redefinição de senha de autoatendados (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a24a67fdb4bcc054036de26ba235bf4bac0f2da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440364"
---
# <a name="emailauthenticationmethod-resource-type"></a><span data-ttu-id="578ad-104">Tipo de recurso emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="578ad-104">emailAuthenticationMethod resource type</span></span>

<span data-ttu-id="578ad-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="578ad-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="578ad-106">Uma representação de um endereço de email registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-106">A representation of an email address registered to a user.</span></span> <span data-ttu-id="578ad-107">O email é um método de autenticação disponível apenas para redefinição de senha de autoatendados (SSPR).</span><span class="sxs-lookup"><span data-stu-id="578ad-107">Email is an authentication method available only to self-service password reset (SSPR).</span></span> <span data-ttu-id="578ad-108">Os usuários podem ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="578ad-108">Users may only have one email authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="578ad-109">Methods</span><span class="sxs-lookup"><span data-stu-id="578ad-109">Methods</span></span>
|<span data-ttu-id="578ad-110">Método</span><span class="sxs-lookup"><span data-stu-id="578ad-110">Method</span></span>|<span data-ttu-id="578ad-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="578ad-111">Return type</span></span>|<span data-ttu-id="578ad-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="578ad-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="578ad-113">List</span><span class="sxs-lookup"><span data-stu-id="578ad-113">List</span></span>](../api/emailauthenticationmethod-list.md)|<span data-ttu-id="578ad-114">[Coleção emailAuthenticationMethod](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="578ad-114">[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection</span></span>|<span data-ttu-id="578ad-115">Recupere uma lista de emailsauthenticationMethods de um usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-115">Retrieve a list of a user's emailAuthenticationMethods.</span></span> <span data-ttu-id="578ad-116">Os usuários podem ter apenas um método de autenticação de email.</span><span class="sxs-lookup"><span data-stu-id="578ad-116">Users may only have one email authentication method.</span></span>|
|[<span data-ttu-id="578ad-117">Create</span><span class="sxs-lookup"><span data-stu-id="578ad-117">Create</span></span>](../api/emailauthenticationmethod-post.md)|[<span data-ttu-id="578ad-118">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="578ad-118">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="578ad-119">Criar o objeto emailMethods de um usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-119">Create a user's emailMethods object.</span></span>|
|[<span data-ttu-id="578ad-120">Get</span><span class="sxs-lookup"><span data-stu-id="578ad-120">Get</span></span>](../api/emailauthenticationmethod-get.md)|[<span data-ttu-id="578ad-121">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="578ad-121">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="578ad-122">Recupere as propriedades do objeto emailAuthenticationMethod do usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-122">Retrieve the properties  of the user's emailAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="578ad-123">Atualização</span><span class="sxs-lookup"><span data-stu-id="578ad-123">Update</span></span>](../api/emailauthenticationmethod-update.md)|[<span data-ttu-id="578ad-124">emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="578ad-124">emailAuthenticationMethod</span></span>](../resources/emailauthenticationmethod.md)|<span data-ttu-id="578ad-125">Atualize as propriedades do objeto emailMethods de um usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-125">Update the properties of a user's emailMethods object.</span></span>|
|[<span data-ttu-id="578ad-126">Delete</span><span class="sxs-lookup"><span data-stu-id="578ad-126">Delete</span></span>](../api/emailauthenticationmethod-delete.md)|<span data-ttu-id="578ad-127">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="578ad-127">None</span></span>|<span data-ttu-id="578ad-128">Exclua o objeto emailAuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-128">Delete a user's emailAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="578ad-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="578ad-129">Properties</span></span>
|<span data-ttu-id="578ad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="578ad-130">Property</span></span>|<span data-ttu-id="578ad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="578ad-131">Type</span></span>|<span data-ttu-id="578ad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="578ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="578ad-133">id</span><span class="sxs-lookup"><span data-stu-id="578ad-133">id</span></span>|<span data-ttu-id="578ad-134">String</span><span class="sxs-lookup"><span data-stu-id="578ad-134">String</span></span>|<span data-ttu-id="578ad-135">O identificador do endereço de email registrado para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-135">The identifier of the email address registered to this user.</span></span>|
|<span data-ttu-id="578ad-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="578ad-136">emailAddress</span></span>|<span data-ttu-id="578ad-137">String</span><span class="sxs-lookup"><span data-stu-id="578ad-137">String</span></span>|<span data-ttu-id="578ad-138">O endereço de email registrado para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="578ad-138">The email address registered to this user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="578ad-139">Relações</span><span class="sxs-lookup"><span data-stu-id="578ad-139">Relationships</span></span>
<span data-ttu-id="578ad-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="578ad-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="578ad-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="578ad-141">JSON representation</span></span>
<span data-ttu-id="578ad-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="578ad-142">The following is a JSON representation of the resource.</span></span>
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

