---
title: Tipo de recurso emailAuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação OTP de email
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1f85db08d4502df6cc3a928d2d56761b33dcc6d8
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232043"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="959e4-103">Tipo de recurso emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="959e4-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="959e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="959e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="959e4-105">Representa a política de métodos de autenticação OTP de email desse locatário.</span><span class="sxs-lookup"><span data-stu-id="959e4-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="959e4-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="959e4-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="959e4-107">O OTP de email pode ser usado pelos usuários nativos da nuvem do locatário para redefinição de senha de autoatendados ou por usuários externos para autenticação durante o resgate de convites e a inscrição de autoatendida para aplicativos específicos em fluxos de usuário.</span><span class="sxs-lookup"><span data-stu-id="959e4-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication during invitation redemption and self-service sign-up for specific apps in user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="959e4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="959e4-108">Methods</span></span>

|<span data-ttu-id="959e4-109">Método</span><span class="sxs-lookup"><span data-stu-id="959e4-109">Method</span></span>|<span data-ttu-id="959e4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="959e4-110">Return type</span></span>|<span data-ttu-id="959e4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="959e4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="959e4-112">Obter emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="959e4-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="959e4-113">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="959e4-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="959e4-114">Leia as propriedades e as relações de um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="959e4-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="959e4-115">Atualizar emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="959e4-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="959e4-116">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="959e4-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="959e4-117">Atualize as propriedades de um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="959e4-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="959e4-118">Excluir emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="959e4-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="959e4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="959e4-119">None</span></span>|<span data-ttu-id="959e4-120">Exclui um objeto emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="959e4-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="959e4-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="959e4-121">Properties</span></span>

|<span data-ttu-id="959e4-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="959e4-122">Property</span></span>|<span data-ttu-id="959e4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="959e4-123">Type</span></span>|<span data-ttu-id="959e4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="959e4-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959e4-125">id</span><span class="sxs-lookup"><span data-stu-id="959e4-125">id</span></span>|<span data-ttu-id="959e4-126">String</span><span class="sxs-lookup"><span data-stu-id="959e4-126">String</span></span>|<span data-ttu-id="959e4-127">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="959e4-127">The authentication method policy identifier.</span></span> <span data-ttu-id="959e4-128">Herdado [da autenticaçãoMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="959e4-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="959e4-129">state</span><span class="sxs-lookup"><span data-stu-id="959e4-129">state</span></span>|<span data-ttu-id="959e4-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="959e4-130">authenticationMethodState</span></span>|<span data-ttu-id="959e4-131">Indica se esse método de autenticação está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="959e4-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="959e4-132">Os valores possíveis são: `enabled` e `disabled`.</span><span class="sxs-lookup"><span data-stu-id="959e4-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="959e4-133">allowExternalIdToUseEmailOtp</span><span class="sxs-lookup"><span data-stu-id="959e4-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="959e4-134">externalEmailOtpState</span><span class="sxs-lookup"><span data-stu-id="959e4-134">externalEmailOtpState</span></span>|<span data-ttu-id="959e4-135">Determina se o OTP de email pode ser usuável por usuários externos para autenticação.</span><span class="sxs-lookup"><span data-stu-id="959e4-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="959e4-136">Os valores possíveis são: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="959e4-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="959e4-137">Os locatários no estado que não utilizaram a visualização pública terão automaticamente o OTP de email habilitado a partir `default` de outubro de 2021.</span><span class="sxs-lookup"><span data-stu-id="959e4-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in October 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="959e4-138">Relações</span><span class="sxs-lookup"><span data-stu-id="959e4-138">Relationships</span></span>

|<span data-ttu-id="959e4-139">Relação</span><span class="sxs-lookup"><span data-stu-id="959e4-139">Relationship</span></span>|<span data-ttu-id="959e4-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="959e4-140">Type</span></span>|<span data-ttu-id="959e4-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="959e4-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959e4-142">includeTargets</span><span class="sxs-lookup"><span data-stu-id="959e4-142">includeTargets</span></span>|<span data-ttu-id="959e4-143">[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="959e4-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="959e4-144">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="959e4-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="959e4-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="959e4-145">JSON representation</span></span>

<span data-ttu-id="959e4-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="959e4-146">The following is a JSON representation of the resource.</span></span>
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
