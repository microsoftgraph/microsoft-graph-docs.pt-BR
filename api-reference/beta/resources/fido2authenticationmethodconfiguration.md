---
title: tipo de recurso fido2AuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação FIDO2
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b5d823caefba62a66fc9b2a7236c063cfaeee69b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440315"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="4190e-103">tipo de recurso fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4190e-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="4190e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4190e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4190e-105">Representa uma política de métodos de autenticação FIDO2.</span><span class="sxs-lookup"><span data-stu-id="4190e-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="4190e-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4190e-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="4190e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="4190e-107">Methods</span></span>
|<span data-ttu-id="4190e-108">Método</span><span class="sxs-lookup"><span data-stu-id="4190e-108">Method</span></span>|<span data-ttu-id="4190e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4190e-109">Return type</span></span>|<span data-ttu-id="4190e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4190e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4190e-111">Get</span><span class="sxs-lookup"><span data-stu-id="4190e-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="4190e-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4190e-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="4190e-113">Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4190e-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="4190e-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="4190e-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="4190e-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4190e-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="4190e-116">Atualize as propriedades de um objeto fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4190e-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="4190e-117">Delete</span><span class="sxs-lookup"><span data-stu-id="4190e-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="4190e-118">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="4190e-118">None</span></span>|<span data-ttu-id="4190e-119">Reverte o objeto fido2AuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="4190e-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="4190e-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4190e-120">Properties</span></span>
|<span data-ttu-id="4190e-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4190e-121">Property</span></span>|<span data-ttu-id="4190e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="4190e-122">Type</span></span>|<span data-ttu-id="4190e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4190e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4190e-124">id</span><span class="sxs-lookup"><span data-stu-id="4190e-124">id</span></span>|<span data-ttu-id="4190e-125">String</span><span class="sxs-lookup"><span data-stu-id="4190e-125">String</span></span>|<span data-ttu-id="4190e-126">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4190e-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="4190e-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="4190e-127">isAttestationEnforced</span></span>|<span data-ttu-id="4190e-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="4190e-128">Boolean</span></span>|<span data-ttu-id="4190e-129">Determina se o atestado deve ser imposto para o registro da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="4190e-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="4190e-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="4190e-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="4190e-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="4190e-131">Boolean</span></span>|<span data-ttu-id="4190e-132">Determina se os usuários podem registrar novas chaves de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="4190e-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="4190e-133">keyRestrictions</span><span class="sxs-lookup"><span data-stu-id="4190e-133">keyRestrictions</span></span>|[<span data-ttu-id="4190e-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="4190e-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="4190e-135">Controla se as restrições de chave são impostas às teclas de segurança FIDO2, permitindo ou desproteção de determinados tipos de chave, conforme definido pelo AAGUID (Authenticator Attestation GUID), um identificador que indica o tipo (por exemplo, make e model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="4190e-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="4190e-136">state</span><span class="sxs-lookup"><span data-stu-id="4190e-136">state</span></span>|<span data-ttu-id="4190e-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="4190e-137">authenticationMethodState</span></span>|<span data-ttu-id="4190e-138">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4190e-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4190e-139">Relações</span><span class="sxs-lookup"><span data-stu-id="4190e-139">Relationships</span></span>
|<span data-ttu-id="4190e-140">Relação</span><span class="sxs-lookup"><span data-stu-id="4190e-140">Relationship</span></span>|<span data-ttu-id="4190e-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="4190e-141">Type</span></span>|<span data-ttu-id="4190e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="4190e-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4190e-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="4190e-143">includeTargets</span></span>|<span data-ttu-id="4190e-144">[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="4190e-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="4190e-145">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4190e-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4190e-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4190e-146">JSON representation</span></span>
<span data-ttu-id="4190e-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4190e-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  },
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
