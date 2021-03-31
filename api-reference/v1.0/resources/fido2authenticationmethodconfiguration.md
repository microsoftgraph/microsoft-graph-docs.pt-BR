---
title: tipo de recurso fido2AuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação FIDO2
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 00137618daf327793d7d60d8dadbe8ad89abc840
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468622"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="3e9f9-103">tipo de recurso fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e9f9-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="3e9f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e9f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e9f9-105">Representa uma política de métodos de autenticação FIDO2.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="3e9f9-106">As políticas de métodos de autenticação definem configurações e usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="3e9f9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3e9f9-107">Methods</span></span>
|<span data-ttu-id="3e9f9-108">Método</span><span class="sxs-lookup"><span data-stu-id="3e9f9-108">Method</span></span>|<span data-ttu-id="3e9f9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e9f9-109">Return type</span></span>|<span data-ttu-id="3e9f9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e9f9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e9f9-111">Get</span><span class="sxs-lookup"><span data-stu-id="3e9f9-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="3e9f9-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e9f9-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="3e9f9-113">Leia as propriedades e as relações de um objeto fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="3e9f9-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="3e9f9-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="3e9f9-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e9f9-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="3e9f9-116">Atualize as propriedades de um objeto fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="3e9f9-117">Delete</span><span class="sxs-lookup"><span data-stu-id="3e9f9-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="3e9f9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e9f9-118">None</span></span>|<span data-ttu-id="3e9f9-119">Reverte o objeto fido2AuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="3e9f9-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e9f9-120">Properties</span></span>
|<span data-ttu-id="3e9f9-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e9f9-121">Property</span></span>|<span data-ttu-id="3e9f9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e9f9-122">Type</span></span>|<span data-ttu-id="3e9f9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e9f9-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e9f9-124">id</span><span class="sxs-lookup"><span data-stu-id="3e9f9-124">id</span></span>|<span data-ttu-id="3e9f9-125">String</span><span class="sxs-lookup"><span data-stu-id="3e9f9-125">String</span></span>|<span data-ttu-id="3e9f9-126">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="3e9f9-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="3e9f9-127">isAttestationEnforced</span></span>|<span data-ttu-id="3e9f9-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e9f9-128">Boolean</span></span>|<span data-ttu-id="3e9f9-129">Determina se o atestado deve ser imposto para o registro da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="3e9f9-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="3e9f9-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="3e9f9-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e9f9-131">Boolean</span></span>|<span data-ttu-id="3e9f9-132">Determina se os usuários podem registrar novas chaves de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="3e9f9-133">keyRestrictions</span><span class="sxs-lookup"><span data-stu-id="3e9f9-133">keyRestrictions</span></span>|[<span data-ttu-id="3e9f9-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="3e9f9-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="3e9f9-135">Controla se as restrições de chave são impostas às teclas de segurança FIDO2, permitindo ou desproteção de determinados tipos de chave, conforme definido pelo AAGUID (Authenticator Attestation GUID), um identificador que indica o tipo (por exemplo, make e model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="3e9f9-136">state</span><span class="sxs-lookup"><span data-stu-id="3e9f9-136">state</span></span>|<span data-ttu-id="3e9f9-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="3e9f9-137">authenticationMethodState</span></span>|<span data-ttu-id="3e9f9-138">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e9f9-139">Relações</span><span class="sxs-lookup"><span data-stu-id="3e9f9-139">Relationships</span></span>
|<span data-ttu-id="3e9f9-140">Relação</span><span class="sxs-lookup"><span data-stu-id="3e9f9-140">Relationship</span></span>|<span data-ttu-id="3e9f9-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e9f9-141">Type</span></span>|<span data-ttu-id="3e9f9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e9f9-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e9f9-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="3e9f9-143">includeTargets</span></span>|<span data-ttu-id="3e9f9-144">[coleção authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="3e9f9-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="3e9f9-145">Uma coleção de usuários ou grupos habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e9f9-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e9f9-146">JSON representation</span></span>
<span data-ttu-id="3e9f9-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e9f9-147">The following is a JSON representation of the resource.</span></span>
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
