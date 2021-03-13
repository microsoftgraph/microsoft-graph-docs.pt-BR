---
title: tipo de recurso temporaryAccessPassAuthenticationMethod
description: Representa um Passe de Acesso Temporário registrado para um usuário.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8c118978f9e7c8a7c3aa127ba12aba48f2cfe362
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760957"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a><span data-ttu-id="db795-103">tipo de recurso temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db795-103">temporaryAccessPassAuthenticationMethod resource type</span></span>

<span data-ttu-id="db795-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db795-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db795-105">Representa um Passe de Acesso Temporário registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="db795-105">Represents a Temporary Access Pass registered to a user.</span></span> <span data-ttu-id="db795-106">Um Passe de Acesso Temporário é uma senha limitada por tempo que serve como uma credencial forte e permite a integração de credenciais sem senha.</span><span class="sxs-lookup"><span data-stu-id="db795-106">A Temporary Access Pass is a time-limited passcode that serves as a strong credential and allows onboarding of passwordless credentials.</span></span>

## <a name="methods"></a><span data-ttu-id="db795-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="db795-107">Methods</span></span>
|<span data-ttu-id="db795-108">Método</span><span class="sxs-lookup"><span data-stu-id="db795-108">Method</span></span>|<span data-ttu-id="db795-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db795-109">Return type</span></span>|<span data-ttu-id="db795-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db795-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db795-111">List</span><span class="sxs-lookup"><span data-stu-id="db795-111">List</span></span>](../api/temporaryaccesspassauthenticationmethod-list.md)|<span data-ttu-id="db795-112">[coleção temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="db795-112">[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) collection</span></span>|<span data-ttu-id="db795-113">Recupere uma lista dos objetos **temporaryAccessPassAuthenticationMethod** de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="db795-113">Retrieve a list of a user's **temporaryAccessPassAuthenticationMethod** objects and their properties.</span></span> <span data-ttu-id="db795-114">Os usuários só podem ter um método de autenticação de Passagem de Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="db795-114">Users can only have one Temporary Access Pass authentication method.</span></span>|
|[<span data-ttu-id="db795-115">Create</span><span class="sxs-lookup"><span data-stu-id="db795-115">Create</span></span>](../api/temporaryaccesspassauthenticationmethod-post.md)|[<span data-ttu-id="db795-116">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db795-116">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="db795-117">Crie um objeto **temporaryAccessPassAuthenticationMethod de um** usuário.</span><span class="sxs-lookup"><span data-stu-id="db795-117">Create a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|
|[<span data-ttu-id="db795-118">Obter</span><span class="sxs-lookup"><span data-stu-id="db795-118">Get</span></span>](../api/temporaryaccesspassauthenticationmethod-get.md)|[<span data-ttu-id="db795-119">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db795-119">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="db795-120">Recupere as propriedades do objeto **temporaryAccessPassAuthenticationMethod do** usuário.</span><span class="sxs-lookup"><span data-stu-id="db795-120">Retrieve the properties of the user's **temporaryAccessPassAuthenticationMethod** object.</span></span>||
|[<span data-ttu-id="db795-121">Delete</span><span class="sxs-lookup"><span data-stu-id="db795-121">Delete</span></span>](../api/temporaryaccesspassauthenticationmethod-delete.md)|<span data-ttu-id="db795-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db795-122">None</span></span>|<span data-ttu-id="db795-123">Exclua o **objeto temporaryAccessPassAuthenticationMethod de um** usuário.</span><span class="sxs-lookup"><span data-stu-id="db795-123">Delete a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="db795-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db795-124">Properties</span></span>
|<span data-ttu-id="db795-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db795-125">Property</span></span>|<span data-ttu-id="db795-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="db795-126">Type</span></span>|<span data-ttu-id="db795-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="db795-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db795-128">id</span><span class="sxs-lookup"><span data-stu-id="db795-128">id</span></span>|<span data-ttu-id="db795-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db795-129">String</span></span>|<span data-ttu-id="db795-130">O identificador do Passe de Acesso Temporário registrado para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="db795-130">The identifier of the Temporary Access Pass registered to this user.</span></span>|
|<span data-ttu-id="db795-131">temporaryAccessPass</span><span class="sxs-lookup"><span data-stu-id="db795-131">temporaryAccessPass</span></span>|<span data-ttu-id="db795-132">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="db795-132">String</span></span>|<span data-ttu-id="db795-133">O temporaryAccessPass usado para autenticar.</span><span class="sxs-lookup"><span data-stu-id="db795-133">The temporaryAccessPass used to authenticate.</span></span> <span data-ttu-id="db795-134">Retornado somente na criação de um novo temporaryAccessPass; retornado como NULL com GET.</span><span class="sxs-lookup"><span data-stu-id="db795-134">Returned only on creation of a new temporaryAccessPass; returned as NULL with GET.</span></span>|
|<span data-ttu-id="db795-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db795-135">createdDateTime</span></span>|<span data-ttu-id="db795-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db795-136">DateTimeOffset</span></span>|<span data-ttu-id="db795-137">A data e a hora em que o temporaryAccessPass foi criado.</span><span class="sxs-lookup"><span data-stu-id="db795-137">The date and time when the temporaryAccessPass was created.</span></span>|
|<span data-ttu-id="db795-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="db795-138">startDateTime</span></span>|<span data-ttu-id="db795-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db795-139">DateTimeOffset</span></span>|<span data-ttu-id="db795-140">A data e a hora em que o temporaryAccessPass fica disponível para uso.</span><span class="sxs-lookup"><span data-stu-id="db795-140">The date and time when the temporaryAccessPass becomes available to use.</span></span>|
|<span data-ttu-id="db795-141">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="db795-141">lifetimeInMinutes</span></span>|<span data-ttu-id="db795-142">Int32</span><span class="sxs-lookup"><span data-stu-id="db795-142">Int32</span></span>|<span data-ttu-id="db795-143">O tempo de vida do temporaryAccessPass em minutos começando em startDateTime.</span><span class="sxs-lookup"><span data-stu-id="db795-143">The lifetime of the temporaryAccessPass in minutes starting at startDateTime.</span></span> <span data-ttu-id="db795-144">Mínimo 10, Máximo 43200 (equivalente a 30 dias).</span><span class="sxs-lookup"><span data-stu-id="db795-144">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>|
|<span data-ttu-id="db795-145">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="db795-145">isUsableOnce</span></span>|<span data-ttu-id="db795-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="db795-146">Boolean</span></span>|<span data-ttu-id="db795-147">Determina se a passagem está limitada a um uso único.</span><span class="sxs-lookup"><span data-stu-id="db795-147">Determines whether the pass is limited to a one time use.</span></span> <span data-ttu-id="db795-148">If , the pass can be used once; if , the pass can be `true` used multiple times within the `false` temporaryAccessPass lifetime.</span><span class="sxs-lookup"><span data-stu-id="db795-148">If `true`, the pass can be used once; if `false`, the pass can be used multiple times within the temporaryAccessPass lifetime.</span></span>|
|<span data-ttu-id="db795-149">isUsable</span><span class="sxs-lookup"><span data-stu-id="db795-149">isUsable</span></span>|<span data-ttu-id="db795-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="db795-150">Boolean</span></span>|<span data-ttu-id="db795-151">O estado do método de autenticação que indica se ele pode ser usado no momento pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="db795-151">The state of the authentication method that indicates whether it's currently usable by the user.</span></span>|
|<span data-ttu-id="db795-152">methodUsabilityReason</span><span class="sxs-lookup"><span data-stu-id="db795-152">methodUsabilityReason</span></span>|<span data-ttu-id="db795-153">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="db795-153">String</span></span>|<span data-ttu-id="db795-154">Detalhes sobre o estado de usabilidade (isUsable).</span><span class="sxs-lookup"><span data-stu-id="db795-154">Details about usability state (isUsable).</span></span> <span data-ttu-id="db795-155">Os motivos podem incluir: `enabledByPolicy` , , , , `disabledByPolicy` `expired` `notYetValid` `oneTimeUsed` .</span><span class="sxs-lookup"><span data-stu-id="db795-155">Reasons can include: `enabledByPolicy`, `disabledByPolicy`, `expired`, `notYetValid`, `oneTimeUsed`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="db795-156">Relações</span><span class="sxs-lookup"><span data-stu-id="db795-156">Relationships</span></span>
<span data-ttu-id="db795-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db795-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db795-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db795-158">JSON representation</span></span>
<span data-ttu-id="db795-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db795-159">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "String (identifier)",
  "temporaryAccessPass": "String",
  "createdDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "isUsable": "Boolean",
  "methodUsabilityReason": "String"
}
```
