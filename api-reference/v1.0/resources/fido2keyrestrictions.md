---
title: Tipo de recurso fido2KeyRestrictions
description: Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1781e39952bb3bf7cfb307d06ca3167ff58a2a6
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469448"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="343fe-103">Tipo de recurso fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="343fe-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="343fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="343fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="343fe-105">Representa as principais restrições impostas como parte da política de métodos de autenticação de chaves de segurança [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="343fe-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="343fe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="343fe-106">Properties</span></span>
|<span data-ttu-id="343fe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="343fe-107">Property</span></span>|<span data-ttu-id="343fe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="343fe-108">Type</span></span>|<span data-ttu-id="343fe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="343fe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="343fe-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="343fe-110">aaGuids</span></span>|<span data-ttu-id="343fe-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="343fe-111">String collection</span></span>|<span data-ttu-id="343fe-112">Uma coleção de GUIDs de Atestado do Autenticador.</span><span class="sxs-lookup"><span data-stu-id="343fe-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="343fe-113">Os AADGUIDs definem os principais tipos e fabricantes.</span><span class="sxs-lookup"><span data-stu-id="343fe-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="343fe-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="343fe-114">enforcementType</span></span>|<span data-ttu-id="343fe-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="343fe-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="343fe-116">Tipo de imposição.</span><span class="sxs-lookup"><span data-stu-id="343fe-116">Enforcement type.</span></span> <span data-ttu-id="343fe-117">Os valores possíveis são: `allow` e `block`.</span><span class="sxs-lookup"><span data-stu-id="343fe-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="343fe-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="343fe-118">isEnforced</span></span>|<span data-ttu-id="343fe-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="343fe-119">Boolean</span></span>|<span data-ttu-id="343fe-120">Determina se a imposição de chave configurada está habilitada.</span><span class="sxs-lookup"><span data-stu-id="343fe-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="343fe-121">Relações</span><span class="sxs-lookup"><span data-stu-id="343fe-121">Relationships</span></span>
<span data-ttu-id="343fe-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="343fe-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="343fe-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="343fe-123">JSON representation</span></span>
<span data-ttu-id="343fe-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="343fe-124">The following is a JSON representation of the resource.</span></span>
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
