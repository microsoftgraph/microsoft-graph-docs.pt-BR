---
title: Tipo de recurso emailAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação OTP de email
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: bcc1a355db78dc697df892cd2f6129ef3caa3bac
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469063"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="ada7b-103">Tipo de recurso emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada7b-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="ada7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ada7b-105">Representa a política de métodos de autenticação OTP de email desse locatário.</span><span class="sxs-lookup"><span data-stu-id="ada7b-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="ada7b-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ada7b-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="ada7b-107">O OTP de email pode ser usado pelos usuários nativos da nuvem do locatário para redefinição de senha de autoatendida ou por usuários externos para autenticação em algumas circunstâncias.</span><span class="sxs-lookup"><span data-stu-id="ada7b-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication in some circumstances.</span></span>

## <a name="methods"></a><span data-ttu-id="ada7b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ada7b-108">Methods</span></span>

|<span data-ttu-id="ada7b-109">Método</span><span class="sxs-lookup"><span data-stu-id="ada7b-109">Method</span></span>|<span data-ttu-id="ada7b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ada7b-110">Return type</span></span>|<span data-ttu-id="ada7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ada7b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ada7b-112">Obter emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada7b-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="ada7b-113">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada7b-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="ada7b-114">Leia as propriedades e as relações de um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ada7b-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ada7b-115">Atualizar emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada7b-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="ada7b-116">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada7b-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="ada7b-117">Atualize as propriedades de um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ada7b-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ada7b-118">Excluir emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada7b-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="ada7b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ada7b-119">None</span></span>|<span data-ttu-id="ada7b-120">Exclui um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ada7b-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ada7b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ada7b-121">Properties</span></span>

|<span data-ttu-id="ada7b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ada7b-122">Property</span></span>|<span data-ttu-id="ada7b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ada7b-123">Type</span></span>|<span data-ttu-id="ada7b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ada7b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada7b-125">id</span><span class="sxs-lookup"><span data-stu-id="ada7b-125">id</span></span>|<span data-ttu-id="ada7b-126">String</span><span class="sxs-lookup"><span data-stu-id="ada7b-126">String</span></span>|<span data-ttu-id="ada7b-127">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ada7b-127">The authentication method policy identifier.</span></span> <span data-ttu-id="ada7b-128">Herdado [da autenticaçãoMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada7b-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="ada7b-129">state</span><span class="sxs-lookup"><span data-stu-id="ada7b-129">state</span></span>|<span data-ttu-id="ada7b-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="ada7b-130">authenticationMethodState</span></span>|<span data-ttu-id="ada7b-131">Indica se esse método de autenticação está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="ada7b-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="ada7b-132">Os valores possíveis são: `enabled` e `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ada7b-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ada7b-133">allowExternalIdToUseEmailOtp</span><span class="sxs-lookup"><span data-stu-id="ada7b-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="ada7b-134">externalEmailOtpState</span><span class="sxs-lookup"><span data-stu-id="ada7b-134">externalEmailOtpState</span></span>|<span data-ttu-id="ada7b-135">Determina se o OTP de email pode ser usuável por usuários externos para autenticação.</span><span class="sxs-lookup"><span data-stu-id="ada7b-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="ada7b-136">Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ada7b-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="ada7b-137">Os locatários no estado que não utilizaram a visualização pública terão automaticamente o OTP de email habilitado a partir de março de `default` 2021.</span><span class="sxs-lookup"><span data-stu-id="ada7b-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in March 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ada7b-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ada7b-138">Relationships</span></span>

|<span data-ttu-id="ada7b-139">Relação</span><span class="sxs-lookup"><span data-stu-id="ada7b-139">Relationship</span></span>|<span data-ttu-id="ada7b-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="ada7b-140">Type</span></span>|<span data-ttu-id="ada7b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="ada7b-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada7b-142">includeTargets</span><span class="sxs-lookup"><span data-stu-id="ada7b-142">includeTargets</span></span>|<span data-ttu-id="ada7b-143">[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="ada7b-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="ada7b-144">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ada7b-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ada7b-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ada7b-145">JSON representation</span></span>

<span data-ttu-id="ada7b-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ada7b-146">The following is a JSON representation of the resource.</span></span>
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
