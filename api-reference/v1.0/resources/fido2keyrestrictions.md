---
title: Tipo de recurso fido2KeyRestrictions
description: Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fd319b64d124fc2c80c7f851a2e062d3568c2d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964619"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="05941-103">Tipo de recurso fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="05941-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="05941-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05941-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05941-105">Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05941-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="05941-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05941-106">Properties</span></span>
|<span data-ttu-id="05941-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05941-107">Property</span></span>|<span data-ttu-id="05941-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="05941-108">Type</span></span>|<span data-ttu-id="05941-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05941-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05941-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="05941-110">aaGuids</span></span>|<span data-ttu-id="05941-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05941-111">String collection</span></span>|<span data-ttu-id="05941-112">Uma coleção de GUIDs de Atestado do Autenticador.</span><span class="sxs-lookup"><span data-stu-id="05941-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="05941-113">Os AADGUIDs definem os principais tipos e fabricantes.</span><span class="sxs-lookup"><span data-stu-id="05941-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="05941-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="05941-114">enforcementType</span></span>|<span data-ttu-id="05941-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="05941-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="05941-116">Tipo de imposição.</span><span class="sxs-lookup"><span data-stu-id="05941-116">Enforcement type.</span></span> <span data-ttu-id="05941-117">Os valores possíveis são: `allow` e `block`.</span><span class="sxs-lookup"><span data-stu-id="05941-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="05941-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="05941-118">isEnforced</span></span>|<span data-ttu-id="05941-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="05941-119">Boolean</span></span>|<span data-ttu-id="05941-120">Determina se a imposição de chave configurada está habilitada.</span><span class="sxs-lookup"><span data-stu-id="05941-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05941-121">Relações</span><span class="sxs-lookup"><span data-stu-id="05941-121">Relationships</span></span>
<span data-ttu-id="05941-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05941-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05941-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05941-123">JSON representation</span></span>
<span data-ttu-id="05941-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05941-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
