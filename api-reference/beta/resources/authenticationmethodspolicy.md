---
title: tipo de recurso authenticationMethodsPolicy
description: Define os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA).
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fdf86929b4098d9fb62f1426883b55d95c669f32
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682864"
---
# <a name="authenticationmethodspolicy-resource-type"></a><span data-ttu-id="6e66f-103">tipo de recurso authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="6e66f-103">authenticationMethodsPolicy resource type</span></span>

<span data-ttu-id="6e66f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e66f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e66f-105">Define os métodos de autenticação e os usuários que têm permissão para usá-los para entrar e executar a autenticação multifato (MFA) no Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6e66f-105">Defines authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="6e66f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e66f-106">Methods</span></span>
|<span data-ttu-id="6e66f-107">Método</span><span class="sxs-lookup"><span data-stu-id="6e66f-107">Method</span></span>|<span data-ttu-id="6e66f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e66f-108">Return type</span></span>|<span data-ttu-id="6e66f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e66f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e66f-110">Obter authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="6e66f-110">Get authenticationMethodsPolicy</span></span>](../api/authenticationmethodspolicy-get.md)|[<span data-ttu-id="6e66f-111">authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="6e66f-111">authenticationMethodsPolicy</span></span>](../resources/authenticationmethodspolicy.md)|<span data-ttu-id="6e66f-112">Leia as propriedades e as relações de um [objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e66f-112">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>|
|[<span data-ttu-id="6e66f-113">Atualizar autenticaçãoMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="6e66f-113">Update authenticationMethodsPolicy</span></span>](../api/authenticationmethodspolicy-update.md)|[<span data-ttu-id="6e66f-114">authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="6e66f-114">authenticationMethodsPolicy</span></span>](../resources/authenticationmethodspolicy.md)|<span data-ttu-id="6e66f-115">Atualize as propriedades de [um objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e66f-115">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e66f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e66f-116">Properties</span></span>
|<span data-ttu-id="6e66f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e66f-117">Property</span></span>|<span data-ttu-id="6e66f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e66f-118">Type</span></span>|<span data-ttu-id="6e66f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e66f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e66f-120">description</span><span class="sxs-lookup"><span data-stu-id="6e66f-120">description</span></span>|<span data-ttu-id="6e66f-121">String</span><span class="sxs-lookup"><span data-stu-id="6e66f-121">String</span></span>|<span data-ttu-id="6e66f-122">Uma descrição da política.</span><span class="sxs-lookup"><span data-stu-id="6e66f-122">A description of the policy.</span></span>|
|<span data-ttu-id="6e66f-123">displayName</span><span class="sxs-lookup"><span data-stu-id="6e66f-123">displayName</span></span>|<span data-ttu-id="6e66f-124">String</span><span class="sxs-lookup"><span data-stu-id="6e66f-124">String</span></span>|<span data-ttu-id="6e66f-125">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="6e66f-125">The name of the policy.</span></span>|
|<span data-ttu-id="6e66f-126">id</span><span class="sxs-lookup"><span data-stu-id="6e66f-126">id</span></span>|<span data-ttu-id="6e66f-127">String</span><span class="sxs-lookup"><span data-stu-id="6e66f-127">String</span></span>|<span data-ttu-id="6e66f-128">O identificador da política.</span><span class="sxs-lookup"><span data-stu-id="6e66f-128">The identifier of the policy.</span></span> <span data-ttu-id="6e66f-129">Herdado da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="6e66f-129">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="6e66f-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e66f-130">lastModifiedDateTime</span></span>|<span data-ttu-id="6e66f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e66f-131">DateTimeOffset</span></span>|<span data-ttu-id="6e66f-132">A data e a hora da última atualização para a política.</span><span class="sxs-lookup"><span data-stu-id="6e66f-132">The date and time of the last update to the policy.</span></span>|
|<span data-ttu-id="6e66f-133">policyVersion</span><span class="sxs-lookup"><span data-stu-id="6e66f-133">policyVersion</span></span>|<span data-ttu-id="6e66f-134">String</span><span class="sxs-lookup"><span data-stu-id="6e66f-134">String</span></span>|<span data-ttu-id="6e66f-135">A versão da política em uso.</span><span class="sxs-lookup"><span data-stu-id="6e66f-135">The version of the policy in use.</span></span>|
|<span data-ttu-id="6e66f-136">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="6e66f-136">registrationEnforcement</span></span>|[<span data-ttu-id="6e66f-137">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="6e66f-137">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="6e66f-138">Impor o registro no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="6e66f-138">Enforce registration at sign-in time.</span></span> <span data-ttu-id="6e66f-139">Essa propriedade pode ser usada para lembrar os usuários de configurar métodos de autenticação direcionados.</span><span class="sxs-lookup"><span data-stu-id="6e66f-139">This property can be used to remind users to set up targeted authentication methods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e66f-140">Relações</span><span class="sxs-lookup"><span data-stu-id="6e66f-140">Relationships</span></span>
|<span data-ttu-id="6e66f-141">Relação</span><span class="sxs-lookup"><span data-stu-id="6e66f-141">Relationship</span></span>|<span data-ttu-id="6e66f-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e66f-142">Type</span></span>|<span data-ttu-id="6e66f-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e66f-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e66f-144">authenticationMethodConfigurations</span><span class="sxs-lookup"><span data-stu-id="6e66f-144">authenticationMethodConfigurations</span></span>|<span data-ttu-id="6e66f-145">[coleção authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e66f-145">[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) collection</span></span>|<span data-ttu-id="6e66f-146">Representa as configurações de cada método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="6e66f-146">Represents the settings for each authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e66f-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e66f-147">JSON representation</span></span>
<span data-ttu-id="6e66f-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e66f-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  } 
}
```
