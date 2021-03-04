---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration tipo de recurso
description: Representa uma política de autenticação de telefone sem senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 054a8c01e0a8ccb1523622fe5df20e8e60831f60
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444060"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a><span data-ttu-id="fe045-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration tipo de recurso (preterido)</span><span class="sxs-lookup"><span data-stu-id="fe045-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type (deprecated)</span></span>

<span data-ttu-id="fe045-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe045-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe045-105">Representa uma política de autenticação de telefone sem senha do Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="fe045-105">Represents a Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy.</span></span> <span data-ttu-id="fe045-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="fe045-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

> [!CAUTION]
> <span data-ttu-id="fe045-107">A API de política de autenticação do método de autenticação de telefone sem senha do Microsoft Authenticator é preterida e parou de retornar resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="fe045-107">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="fe045-108">Use a nova política de método de autenticação do [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe045-108">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fe045-109">Methods</span><span class="sxs-lookup"><span data-stu-id="fe045-109">Methods</span></span>
|<span data-ttu-id="fe045-110">Método</span><span class="sxs-lookup"><span data-stu-id="fe045-110">Method</span></span>|<span data-ttu-id="fe045-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fe045-111">Return type</span></span>|<span data-ttu-id="fe045-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe045-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe045-113">[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="fe045-113">[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (deprecated)</span></span>|[<span data-ttu-id="fe045-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe045-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="fe045-115">Leia as propriedades e as relações de um objetoMicrosoftAuthenticatorAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fe045-115">Read the properties and relationships of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="fe045-116">[Atualização](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (preterida)</span><span class="sxs-lookup"><span data-stu-id="fe045-116">[Update](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (deprecated)</span></span> |[<span data-ttu-id="fe045-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe045-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="fe045-118">Atualize as propriedades de um objetoMicrosoftAuthenticatorAuthenticationMethodConfiguration sem senha.</span><span class="sxs-lookup"><span data-stu-id="fe045-118">Update the properties of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="fe045-119">[Excluir](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (preterido)</span><span class="sxs-lookup"><span data-stu-id="fe045-119">[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (deprecated)</span></span>|<span data-ttu-id="fe045-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="fe045-120">None</span></span>|<span data-ttu-id="fe045-121">Reverte o objeto PasswordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="fe045-121">Reverts the passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="fe045-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe045-122">Properties</span></span>
|<span data-ttu-id="fe045-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe045-123">Property</span></span>|<span data-ttu-id="fe045-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe045-124">Type</span></span>|<span data-ttu-id="fe045-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe045-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe045-126">id</span><span class="sxs-lookup"><span data-stu-id="fe045-126">id</span></span>|<span data-ttu-id="fe045-127">String</span><span class="sxs-lookup"><span data-stu-id="fe045-127">String</span></span>|<span data-ttu-id="fe045-128">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="fe045-128">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="fe045-129">state</span><span class="sxs-lookup"><span data-stu-id="fe045-129">state</span></span>|<span data-ttu-id="fe045-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="fe045-130">authenticationMethodState</span></span>|<span data-ttu-id="fe045-131">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="fe045-131">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe045-132">Relações</span><span class="sxs-lookup"><span data-stu-id="fe045-132">Relationships</span></span>
|<span data-ttu-id="fe045-133">Relação</span><span class="sxs-lookup"><span data-stu-id="fe045-133">Relationship</span></span>|<span data-ttu-id="fe045-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe045-134">Type</span></span>|<span data-ttu-id="fe045-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe045-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe045-136">includeTargets</span><span class="sxs-lookup"><span data-stu-id="fe045-136">includeTargets</span></span>|<span data-ttu-id="fe045-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe045-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="fe045-138">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="fe045-138">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe045-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe045-139">JSON representation</span></span>
<span data-ttu-id="fe045-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe045-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
