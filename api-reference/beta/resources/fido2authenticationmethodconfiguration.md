---
title: tipo de recurso fido2AuthenticationMethodConfiguration
description: Representa uma política de métodos de autenticação do FIDO2
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62aa22fa22b70235f5221bc820cee5178b55b51b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418171"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="6c43c-103">tipo de recurso fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c43c-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="6c43c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c43c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c43c-105">Representa uma política de métodos de autenticação do FIDO2.</span><span class="sxs-lookup"><span data-stu-id="6c43c-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="6c43c-106">Métodos de autenticação as políticas definem definições de configuração e usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="6c43c-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="6c43c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c43c-107">Methods</span></span>
|<span data-ttu-id="6c43c-108">Método</span><span class="sxs-lookup"><span data-stu-id="6c43c-108">Method</span></span>|<span data-ttu-id="6c43c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c43c-109">Return type</span></span>|<span data-ttu-id="6c43c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c43c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c43c-111">Get</span><span class="sxs-lookup"><span data-stu-id="6c43c-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="6c43c-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c43c-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="6c43c-113">Leia as propriedades e os relacionamentos de um objeto fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c43c-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="6c43c-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6c43c-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="6c43c-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c43c-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="6c43c-116">Atualiza as propriedades de um objeto fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c43c-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="6c43c-117">Excluir</span><span class="sxs-lookup"><span data-stu-id="6c43c-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="6c43c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c43c-118">None</span></span>|<span data-ttu-id="6c43c-119">Reverte o objeto fido2AuthenticationMethodConfiguration para sua configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="6c43c-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="6c43c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c43c-120">Properties</span></span>
|<span data-ttu-id="6c43c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c43c-121">Property</span></span>|<span data-ttu-id="6c43c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c43c-122">Type</span></span>|<span data-ttu-id="6c43c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c43c-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c43c-124">id</span><span class="sxs-lookup"><span data-stu-id="6c43c-124">id</span></span>|<span data-ttu-id="6c43c-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c43c-125">String</span></span>|<span data-ttu-id="6c43c-126">O identificador de política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="6c43c-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="6c43c-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="6c43c-127">isAttestationEnforced</span></span>|<span data-ttu-id="6c43c-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c43c-128">Boolean</span></span>|<span data-ttu-id="6c43c-129">Determina se o atestado deve ser aplicado para o registro da chave de segurança do FIDO2.</span><span class="sxs-lookup"><span data-stu-id="6c43c-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="6c43c-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="6c43c-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="6c43c-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c43c-131">Boolean</span></span>|<span data-ttu-id="6c43c-132">Determina se os usuários podem registrar novas chaves de segurança do FIDO2.</span><span class="sxs-lookup"><span data-stu-id="6c43c-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="6c43c-133">restrições de</span><span class="sxs-lookup"><span data-stu-id="6c43c-133">keyRestrictions</span></span>|[<span data-ttu-id="6c43c-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="6c43c-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="6c43c-135">Controla se as restrições de chave são impostas nas chaves de segurança do FIDO2, permitindo ou não a permissão de certos tipos de chave, conforme definido pelo GUID de atestado de autenticador (AAGUID), um identificador que indica o tipo (por exemplo, Make e Model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="6c43c-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="6c43c-136">estado</span><span class="sxs-lookup"><span data-stu-id="6c43c-136">state</span></span>|<span data-ttu-id="6c43c-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="6c43c-137">authenticationMethodState</span></span>|<span data-ttu-id="6c43c-138">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6c43c-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c43c-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6c43c-139">Relationships</span></span>
|<span data-ttu-id="6c43c-140">Relação</span><span class="sxs-lookup"><span data-stu-id="6c43c-140">Relationship</span></span>|<span data-ttu-id="6c43c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c43c-141">Type</span></span>|<span data-ttu-id="6c43c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c43c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c43c-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="6c43c-143">includeTargets</span></span>|<span data-ttu-id="6c43c-144">coleção [authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="6c43c-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="6c43c-145">Uma coleção de usuários ou grupos que estão habilitados para usar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="6c43c-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c43c-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c43c-146">JSON representation</span></span>
<span data-ttu-id="6c43c-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c43c-147">The following is a JSON representation of the resource.</span></span>
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
