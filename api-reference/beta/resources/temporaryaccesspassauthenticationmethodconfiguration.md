---
title: Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de Passagem de Acesso Temporário.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9edb4038180a96d6878fcaf6770728a1befbca19
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272587"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="21104-103">Tipo de recurso temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="21104-103">temporaryAccessPassAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="21104-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21104-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21104-105">Representa uma política de métodos de autenticação de Passagem de Acesso Temporário.</span><span class="sxs-lookup"><span data-stu-id="21104-105">Represents a Temporary Access Pass authentication methods policy.</span></span> <span data-ttu-id="21104-106">A política de métodos de autenticação define as definições de configuração e os usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="21104-106">The Authentication methods policy defines the configuration settings and users or groups who are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="21104-107">Methods</span><span class="sxs-lookup"><span data-stu-id="21104-107">Methods</span></span>
|<span data-ttu-id="21104-108">Método</span><span class="sxs-lookup"><span data-stu-id="21104-108">Method</span></span>|<span data-ttu-id="21104-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21104-109">Return type</span></span>|<span data-ttu-id="21104-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21104-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21104-111">Get</span><span class="sxs-lookup"><span data-stu-id="21104-111">Get</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="21104-112">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="21104-112">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="21104-113">Leia as propriedades e os relacionamentos de **um objeto temporaryaccesspassauthenticationmethodconfiguration.**</span><span class="sxs-lookup"><span data-stu-id="21104-113">Read the properties and relationships of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|[<span data-ttu-id="21104-114">Update</span><span class="sxs-lookup"><span data-stu-id="21104-114">Update</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="21104-115">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="21104-115">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="21104-116">Atualizar as propriedades de **um objeto temporaryaccesspassauthenticationmethodconfiguration.**</span><span class="sxs-lookup"><span data-stu-id="21104-116">Update the properties of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|[<span data-ttu-id="21104-117">Delete</span><span class="sxs-lookup"><span data-stu-id="21104-117">Delete</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="21104-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21104-118">None</span></span>|<span data-ttu-id="21104-119">Reverte o **objeto temporaryaccesspassauthenticationmethodconfiguration** para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="21104-119">Reverts the **temporaryaccesspassauthenticationmethodconfiguration** object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="21104-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21104-120">Properties</span></span>
|<span data-ttu-id="21104-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21104-121">Property</span></span>|<span data-ttu-id="21104-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="21104-122">Type</span></span>|<span data-ttu-id="21104-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="21104-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21104-124">id</span><span class="sxs-lookup"><span data-stu-id="21104-124">id</span></span>|<span data-ttu-id="21104-125">String</span><span class="sxs-lookup"><span data-stu-id="21104-125">String</span></span>|<span data-ttu-id="21104-126">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="21104-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="21104-127">minimumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="21104-127">minimumLifetimeInMinutes</span></span>|<span data-ttu-id="21104-128">Int</span><span class="sxs-lookup"><span data-stu-id="21104-128">Int</span></span>|<span data-ttu-id="21104-129">Tempo de vida mínimo em minutos para qualquer temporaryAccessPass criado no locatário.</span><span class="sxs-lookup"><span data-stu-id="21104-129">Minimum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="21104-130">O valor pode estar entre 10 e 43.200 minutos (equivalente a 30 dias).</span><span class="sxs-lookup"><span data-stu-id="21104-130">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="21104-131">maximumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="21104-131">maximumLifetimeInMinutes</span></span>|<span data-ttu-id="21104-132">Int</span><span class="sxs-lookup"><span data-stu-id="21104-132">Int</span></span>|<span data-ttu-id="21104-133">Tempo de vida máximo em minutos para qualquer temporaryAccessPass criado no locatário.</span><span class="sxs-lookup"><span data-stu-id="21104-133">Maximum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="21104-134">O valor pode estar entre 10 e 43.200 minutos (equivalente a 30 dias).</span><span class="sxs-lookup"><span data-stu-id="21104-134">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="21104-135">defaultLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="21104-135">defaultLifetimeInMinutes</span></span>|<span data-ttu-id="21104-136">int</span><span class="sxs-lookup"><span data-stu-id="21104-136">int</span></span>|<span data-ttu-id="21104-137">Tempo de vida padrão, em minutos, para um temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="21104-137">Default lifetime, in minutes, for a temporaryAccessPass.</span></span> <span data-ttu-id="21104-138">O valor pode estar entre minimumLifetimeInMinutes e maximumLifetimeInMinutes.</span><span class="sxs-lookup"><span data-stu-id="21104-138">Value can be between the minimumLifetimeInMinutes and maximumLifetimeInMinutes.</span></span>|
|<span data-ttu-id="21104-139">defaultLength</span><span class="sxs-lookup"><span data-stu-id="21104-139">defaultLength</span></span>|<span data-ttu-id="21104-140">int</span><span class="sxs-lookup"><span data-stu-id="21104-140">int</span></span>|<span data-ttu-id="21104-141">Comprimento padrão, em caracteres, de um temporaryAccessPass, entre 8 e 48 caracteres.</span><span class="sxs-lookup"><span data-stu-id="21104-141">Default length, in characters, of a temporaryAccessPass, between 8 and 48 characters.</span></span>|
|<span data-ttu-id="21104-142">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="21104-142">isUsableOnce</span></span>|<span data-ttu-id="21104-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="21104-143">Boolean</span></span>   |<span data-ttu-id="21104-144">Se `true` , todas as passagens no locatário serão restritas ao uso único.</span><span class="sxs-lookup"><span data-stu-id="21104-144">If `true`, all the passes in the tenant will be restricted to one-time use.</span></span> <span data-ttu-id="21104-145">Se , passa no locatário pode ser criado para ser uso único ou `false` uso de várias vezes.</span><span class="sxs-lookup"><span data-stu-id="21104-145">If `false`, passes in the tenant can be created to be either one-time use or multiple time use.</span></span>|
|<span data-ttu-id="21104-146">estado</span><span class="sxs-lookup"><span data-stu-id="21104-146">state</span></span>|<span data-ttu-id="21104-147">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="21104-147">authenticationMethodState</span></span>|<span data-ttu-id="21104-148">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="21104-148">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21104-149">Relações</span><span class="sxs-lookup"><span data-stu-id="21104-149">Relationships</span></span>
|<span data-ttu-id="21104-150">Relação</span><span class="sxs-lookup"><span data-stu-id="21104-150">Relationship</span></span>|<span data-ttu-id="21104-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="21104-151">Type</span></span>|<span data-ttu-id="21104-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="21104-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21104-153">includeTargets</span><span class="sxs-lookup"><span data-stu-id="21104-153">includeTargets</span></span>|<span data-ttu-id="21104-154">[Coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="21104-154">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="21104-155">Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="21104-155">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21104-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21104-156">JSON representation</span></span>
<span data-ttu-id="21104-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21104-157">The following is a JSON representation of the resource.</span></span>

``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
},
"includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
