---
title: tipo de recurso emailAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação OTP de email
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e3e18973759d7f120dd0bd8e984c98568054960
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617107"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="7553a-103">tipo de recurso emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7553a-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="7553a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7553a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7553a-105">Representa a política dos métodos de autenticação OTP de email do locatário.</span><span class="sxs-lookup"><span data-stu-id="7553a-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="7553a-106">Métodos de autenticação as políticas definem definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="7553a-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="7553a-107">A OTP de email pode ser usada pelos usuários de nuvem nativa do locatário para redefinição de senha de autoatendimento ou por usuários externos para autenticação em algumas circunstâncias.</span><span class="sxs-lookup"><span data-stu-id="7553a-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication in some circumstances.</span></span>

## <a name="methods"></a><span data-ttu-id="7553a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7553a-108">Methods</span></span>

|<span data-ttu-id="7553a-109">Método</span><span class="sxs-lookup"><span data-stu-id="7553a-109">Method</span></span>|<span data-ttu-id="7553a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7553a-110">Return type</span></span>|<span data-ttu-id="7553a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7553a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7553a-112">Obter emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7553a-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="7553a-113">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7553a-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="7553a-114">Leia as propriedades e os relacionamentos de um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7553a-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="7553a-115">Atualizar emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7553a-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="7553a-116">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7553a-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="7553a-117">Atualiza as propriedades de um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7553a-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="7553a-118">Excluir emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7553a-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="7553a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7553a-119">None</span></span>|<span data-ttu-id="7553a-120">Exclui um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7553a-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7553a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7553a-121">Properties</span></span>

|<span data-ttu-id="7553a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7553a-122">Property</span></span>|<span data-ttu-id="7553a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7553a-123">Type</span></span>|<span data-ttu-id="7553a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7553a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7553a-125">id</span><span class="sxs-lookup"><span data-stu-id="7553a-125">id</span></span>|<span data-ttu-id="7553a-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7553a-126">String</span></span>|<span data-ttu-id="7553a-127">O identificador de política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="7553a-127">The authentication method policy identifier.</span></span> <span data-ttu-id="7553a-128">Herdado de [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7553a-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="7553a-129">state</span><span class="sxs-lookup"><span data-stu-id="7553a-129">state</span></span>|<span data-ttu-id="7553a-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="7553a-130">authenticationMethodState</span></span>|<span data-ttu-id="7553a-131">Indica se este método de autenticação está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="7553a-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="7553a-132">Os valores possíveis são: `enabled` e `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7553a-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7553a-133">allowExternalIdToUseEmailOtp</span><span class="sxs-lookup"><span data-stu-id="7553a-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="7553a-134">externalEmailOtpState</span><span class="sxs-lookup"><span data-stu-id="7553a-134">externalEmailOtpState</span></span>|<span data-ttu-id="7553a-135">Determina se a OTP de email pode ser usada por usuários externos para autenticação.</span><span class="sxs-lookup"><span data-stu-id="7553a-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="7553a-136">Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7553a-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="7553a-137">Os locatários no `default` estado que não usaram a visualização pública serão automaticamente habilitados para a OTP de email a partir de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="7553a-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in March 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7553a-138">Relações</span><span class="sxs-lookup"><span data-stu-id="7553a-138">Relationships</span></span>

|<span data-ttu-id="7553a-139">Relação</span><span class="sxs-lookup"><span data-stu-id="7553a-139">Relationship</span></span>|<span data-ttu-id="7553a-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="7553a-140">Type</span></span>|<span data-ttu-id="7553a-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="7553a-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7553a-142">includeTargets</span><span class="sxs-lookup"><span data-stu-id="7553a-142">includeTargets</span></span>|<span data-ttu-id="7553a-143">coleção [authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="7553a-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="7553a-144">Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="7553a-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7553a-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7553a-145">JSON representation</span></span>

<span data-ttu-id="7553a-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7553a-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
