---
title: tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf6a66abbf745a769a44cf323ebb245c31ecf60
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418205"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="284f9-103">tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="284f9-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="284f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="284f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="284f9-105">Representa uma política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="284f9-105">Represents a Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy.</span></span> <span data-ttu-id="284f9-106">Métodos de autenticação as políticas definem definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="284f9-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

> [!NOTE]
> <span data-ttu-id="284f9-107">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="284f9-107">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="284f9-108">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="284f9-108">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="methods"></a><span data-ttu-id="284f9-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="284f9-109">Methods</span></span>
|<span data-ttu-id="284f9-110">Método</span><span class="sxs-lookup"><span data-stu-id="284f9-110">Method</span></span>|<span data-ttu-id="284f9-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="284f9-111">Return type</span></span>|<span data-ttu-id="284f9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="284f9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="284f9-113">Get</span><span class="sxs-lookup"><span data-stu-id="284f9-113">Get</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="284f9-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="284f9-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="284f9-115">Leia as propriedades e os relacionamentos de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="284f9-115">Read the properties and relationships of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="284f9-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="284f9-116">Update</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="284f9-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="284f9-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="284f9-118">Atualiza as propriedades de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="284f9-118">Update the properties of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="284f9-119">Excluir</span><span class="sxs-lookup"><span data-stu-id="284f9-119">Delete</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="284f9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="284f9-120">None</span></span>|<span data-ttu-id="284f9-121">Reverte o objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="284f9-121">Reverts the passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="284f9-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="284f9-122">Properties</span></span>
|<span data-ttu-id="284f9-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="284f9-123">Property</span></span>|<span data-ttu-id="284f9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="284f9-124">Type</span></span>|<span data-ttu-id="284f9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="284f9-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="284f9-126">id</span><span class="sxs-lookup"><span data-stu-id="284f9-126">id</span></span>|<span data-ttu-id="284f9-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="284f9-127">String</span></span>|<span data-ttu-id="284f9-128">O identificador de política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="284f9-128">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="284f9-129">estado</span><span class="sxs-lookup"><span data-stu-id="284f9-129">state</span></span>|<span data-ttu-id="284f9-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="284f9-130">authenticationMethodState</span></span>|<span data-ttu-id="284f9-131">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="284f9-131">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="284f9-132">Relações</span><span class="sxs-lookup"><span data-stu-id="284f9-132">Relationships</span></span>
|<span data-ttu-id="284f9-133">Relação</span><span class="sxs-lookup"><span data-stu-id="284f9-133">Relationship</span></span>|<span data-ttu-id="284f9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="284f9-134">Type</span></span>|<span data-ttu-id="284f9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="284f9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="284f9-136">includeTargets</span><span class="sxs-lookup"><span data-stu-id="284f9-136">includeTargets</span></span>|<span data-ttu-id="284f9-137">coleção [passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="284f9-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="284f9-138">Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="284f9-138">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="284f9-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="284f9-139">JSON representation</span></span>
<span data-ttu-id="284f9-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="284f9-140">The following is a JSON representation of the resource.</span></span>
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
