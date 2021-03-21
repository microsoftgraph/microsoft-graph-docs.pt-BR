---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 375044feffd7ba22a2e2174808d639d2d2c3b6f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964612"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="8b536-103">Tipo de recurso microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b536-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="8b536-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b536-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b536-105">Representa uma política de métodos de autenticação do Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="8b536-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="8b536-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8b536-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="8b536-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b536-107">Methods</span></span>
|<span data-ttu-id="8b536-108">Método</span><span class="sxs-lookup"><span data-stu-id="8b536-108">Method</span></span>|<span data-ttu-id="8b536-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b536-109">Return type</span></span>|<span data-ttu-id="8b536-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b536-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b536-111">Get</span><span class="sxs-lookup"><span data-stu-id="8b536-111">Get</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="8b536-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b536-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="8b536-113">Leia as propriedades e as relações de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8b536-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="8b536-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="8b536-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="8b536-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b536-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="8b536-116">Atualize as propriedades de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8b536-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="8b536-117">Delete</span><span class="sxs-lookup"><span data-stu-id="8b536-117">Delete</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="8b536-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b536-118">None</span></span>|<span data-ttu-id="8b536-119">Reverte o objeto microsoftAuthenticatorAuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="8b536-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b536-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b536-120">Properties</span></span>
|<span data-ttu-id="8b536-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b536-121">Property</span></span>|<span data-ttu-id="8b536-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b536-122">Type</span></span>|<span data-ttu-id="8b536-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b536-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b536-124">id</span><span class="sxs-lookup"><span data-stu-id="8b536-124">id</span></span>|<span data-ttu-id="8b536-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b536-125">String</span></span>|<span data-ttu-id="8b536-126">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8b536-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="8b536-127">estado</span><span class="sxs-lookup"><span data-stu-id="8b536-127">state</span></span>|<span data-ttu-id="8b536-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="8b536-128">authenticationMethodState</span></span>|<span data-ttu-id="8b536-129">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="8b536-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b536-130">Relações</span><span class="sxs-lookup"><span data-stu-id="8b536-130">Relationships</span></span>
|<span data-ttu-id="8b536-131">Relação</span><span class="sxs-lookup"><span data-stu-id="8b536-131">Relationship</span></span>|<span data-ttu-id="8b536-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b536-132">Type</span></span>|<span data-ttu-id="8b536-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b536-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b536-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="8b536-134">includeTargets</span></span>|<span data-ttu-id="8b536-135">[coleção microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="8b536-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="8b536-136">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8b536-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b536-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b536-137">JSON representation</span></span>
<span data-ttu-id="8b536-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b536-138">The following is a JSON representation of the resource.</span></span>
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

