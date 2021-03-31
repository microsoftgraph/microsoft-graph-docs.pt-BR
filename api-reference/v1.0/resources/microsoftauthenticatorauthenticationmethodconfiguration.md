---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0700a6811b35123709628abc66d8e4eb6b319a03
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469259"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="298b9-103">Tipo de recurso microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="298b9-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="298b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="298b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="298b9-105">Representa uma política de métodos de autenticação do Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="298b9-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="298b9-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="298b9-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="298b9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="298b9-107">Methods</span></span>
|<span data-ttu-id="298b9-108">Método</span><span class="sxs-lookup"><span data-stu-id="298b9-108">Method</span></span>|<span data-ttu-id="298b9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="298b9-109">Return type</span></span>|<span data-ttu-id="298b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="298b9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="298b9-111">Get</span><span class="sxs-lookup"><span data-stu-id="298b9-111">Get</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="298b9-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="298b9-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="298b9-113">Leia as propriedades e as relações de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="298b9-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="298b9-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="298b9-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="298b9-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="298b9-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="298b9-116">Atualize as propriedades de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="298b9-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="298b9-117">Delete</span><span class="sxs-lookup"><span data-stu-id="298b9-117">Delete</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="298b9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="298b9-118">None</span></span>|<span data-ttu-id="298b9-119">Reverte o objeto microsoftAuthenticatorAuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="298b9-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="298b9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="298b9-120">Properties</span></span>
|<span data-ttu-id="298b9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="298b9-121">Property</span></span>|<span data-ttu-id="298b9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="298b9-122">Type</span></span>|<span data-ttu-id="298b9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="298b9-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="298b9-124">id</span><span class="sxs-lookup"><span data-stu-id="298b9-124">id</span></span>|<span data-ttu-id="298b9-125">String</span><span class="sxs-lookup"><span data-stu-id="298b9-125">String</span></span>|<span data-ttu-id="298b9-126">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="298b9-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="298b9-127">state</span><span class="sxs-lookup"><span data-stu-id="298b9-127">state</span></span>|<span data-ttu-id="298b9-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="298b9-128">authenticationMethodState</span></span>|<span data-ttu-id="298b9-129">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="298b9-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="298b9-130">Relações</span><span class="sxs-lookup"><span data-stu-id="298b9-130">Relationships</span></span>
|<span data-ttu-id="298b9-131">Relação</span><span class="sxs-lookup"><span data-stu-id="298b9-131">Relationship</span></span>|<span data-ttu-id="298b9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="298b9-132">Type</span></span>|<span data-ttu-id="298b9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="298b9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="298b9-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="298b9-134">includeTargets</span></span>|<span data-ttu-id="298b9-135">[coleção microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="298b9-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="298b9-136">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="298b9-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="298b9-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="298b9-137">JSON representation</span></span>
<span data-ttu-id="298b9-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="298b9-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

