---
title: tipo de recurso fido2KeyRestrictions
description: Representa as restrições de chave que são impostas como parte da política de métodos de autenticação de chaves de segurança do FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c606b1d7bdbf604bd5109379bffb2c1a20f60730
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418166"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="9acdb-103">tipo de recurso fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="9acdb-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="9acdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9acdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9acdb-105">Representa as restrições de chave que são impostas como parte da [política de métodos de autenticação de chaves de segurança do FIDO2](../resources/fido2authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9acdb-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9acdb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9acdb-106">Properties</span></span>
|<span data-ttu-id="9acdb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9acdb-107">Property</span></span>|<span data-ttu-id="9acdb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9acdb-108">Type</span></span>|<span data-ttu-id="9acdb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9acdb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acdb-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="9acdb-110">aaGuids</span></span>|<span data-ttu-id="9acdb-111">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9acdb-111">String collection</span></span>|<span data-ttu-id="9acdb-112">Uma coleção de GUIDs de atestado de autenticador.</span><span class="sxs-lookup"><span data-stu-id="9acdb-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="9acdb-113">AADGUIDs definir tipos de chave e fabricantes.</span><span class="sxs-lookup"><span data-stu-id="9acdb-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="9acdb-114">imposiçãotype</span><span class="sxs-lookup"><span data-stu-id="9acdb-114">enforcementType</span></span>|<span data-ttu-id="9acdb-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="9acdb-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="9acdb-116">Tipo de imposição.</span><span class="sxs-lookup"><span data-stu-id="9acdb-116">Enforcement type.</span></span> <span data-ttu-id="9acdb-117">Os valores possíveis são: `allow` e `block`.</span><span class="sxs-lookup"><span data-stu-id="9acdb-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="9acdb-118">isforced</span><span class="sxs-lookup"><span data-stu-id="9acdb-118">isEnforced</span></span>|<span data-ttu-id="9acdb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9acdb-119">Boolean</span></span>|<span data-ttu-id="9acdb-120">Determina se a imposição de chave configurada está habilitada.</span><span class="sxs-lookup"><span data-stu-id="9acdb-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9acdb-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9acdb-121">Relationships</span></span>
<span data-ttu-id="9acdb-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9acdb-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9acdb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9acdb-123">JSON representation</span></span>
<span data-ttu-id="9acdb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9acdb-124">The following is a JSON representation of the resource.</span></span>
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
