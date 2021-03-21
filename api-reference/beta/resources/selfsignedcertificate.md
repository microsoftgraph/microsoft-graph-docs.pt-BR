---
title: Tipo de recurso selfSignedCertificate
description: Contém informações sobre a parte pública de um certificado de assinatura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: luleonpla
ms.openlocfilehash: f73cb515ce400762771c7553f6f668c295645b90
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965067"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="b1cc5-103">Tipo de recurso selfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="b1cc5-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="b1cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1cc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1cc5-105">Contém a parte pública de um certificado de assinatura.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="b1cc5-106">É o tipo de retorno da ação [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b1cc5-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="b1cc5-107">Os provedores de serviços usam a parte pública do certificado de assinatura para validar o emissor do token.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-107">Service providers use the the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="b1cc5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1cc5-108">Properties</span></span>
<span data-ttu-id="b1cc5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1cc5-109">Property</span></span>|<span data-ttu-id="b1cc5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1cc5-110">Type</span></span>|<span data-ttu-id="b1cc5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1cc5-111">Description</span></span>
----|--|---
|<span data-ttu-id="b1cc5-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1cc5-112">customKeyIdentifier</span></span>|<span data-ttu-id="b1cc5-113">Binária</span><span class="sxs-lookup"><span data-stu-id="b1cc5-113">Binary</span></span>| <span data-ttu-id="b1cc5-114">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="b1cc5-114">Custom key identifier</span></span> |
| <span data-ttu-id="b1cc5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="b1cc5-115">displayName</span></span> | <span data-ttu-id="b1cc5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1cc5-116">String</span></span> | <span data-ttu-id="b1cc5-117">O nome amigável da chave.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="b1cc5-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b1cc5-118">endDateTime</span></span>|<span data-ttu-id="b1cc5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1cc5-119">DateTimeOffset</span></span>|<span data-ttu-id="b1cc5-120">A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1cc5-121">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="b1cc5-121">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="b1cc5-122">keyId</span><span class="sxs-lookup"><span data-stu-id="b1cc5-122">keyId</span></span>|<span data-ttu-id="b1cc5-123">Guid</span><span class="sxs-lookup"><span data-stu-id="b1cc5-123">Guid</span></span>|<span data-ttu-id="b1cc5-124">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="b1cc5-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b1cc5-125">startDateTime</span></span>|<span data-ttu-id="b1cc5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1cc5-126">DateTimeOffset</span></span>|<span data-ttu-id="b1cc5-127">A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1cc5-128">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="b1cc5-128">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="b1cc5-129">tipo</span><span class="sxs-lookup"><span data-stu-id="b1cc5-129">type</span></span>|<span data-ttu-id="b1cc5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1cc5-130">String</span></span>|<span data-ttu-id="b1cc5-131">O tipo de credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-131">The type of key credential.</span></span> <span data-ttu-id="b1cc5-132">"AsymmetricX509Cert".</span><span class="sxs-lookup"><span data-stu-id="b1cc5-132">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="b1cc5-133">usage</span><span class="sxs-lookup"><span data-stu-id="b1cc5-133">usage</span></span>|<span data-ttu-id="b1cc5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1cc5-134">String</span></span>|<span data-ttu-id="b1cc5-135">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-135">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="b1cc5-136">Por exemplo, "Verificar".</span><span class="sxs-lookup"><span data-stu-id="b1cc5-136">For example, "Verify".</span></span>|
|<span data-ttu-id="b1cc5-137">chave</span><span class="sxs-lookup"><span data-stu-id="b1cc5-137">key</span></span>|<span data-ttu-id="b1cc5-138">Binário</span><span class="sxs-lookup"><span data-stu-id="b1cc5-138">Binary</span></span>| <span data-ttu-id="b1cc5-139">O valor da credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-139">The value for the key credential.</span></span> <span data-ttu-id="b1cc5-140">Deve ser um valor codificado de base-64.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-140">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="b1cc5-141">thumbprint</span><span class="sxs-lookup"><span data-stu-id="b1cc5-141">thumbprint</span></span>| <span data-ttu-id="b1cc5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1cc5-142">String</span></span> | <span data-ttu-id="b1cc5-143">O valor de impressão digital da chave.</span><span class="sxs-lookup"><span data-stu-id="b1cc5-143">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1cc5-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1cc5-144">JSON representation</span></span>

<span data-ttu-id="b1cc5-145">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b1cc5-145">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "binary",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "binary",
    "keyId": "guid",
    "startDateTime": "String (timestamp)",
    "type": "string",
    "thumbprint":"string",
    "usage": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

