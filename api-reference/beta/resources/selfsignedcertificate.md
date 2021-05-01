---
title: Tipo de recurso selfSignedCertificate
description: Contém informações sobre a parte pública de um certificado de assinatura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 1dbb9bcb15a3e820b3676e336826a741ecbb5e9f
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118967"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="9a577-103">Tipo de recurso selfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="9a577-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="9a577-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a577-105">Contém a parte pública de um certificado de assinatura.</span><span class="sxs-lookup"><span data-stu-id="9a577-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="9a577-106">É o tipo de retorno da ação [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9a577-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="9a577-107">Os provedores de serviços usam a parte pública do certificado de assinatura para validar o emissor do token.</span><span class="sxs-lookup"><span data-stu-id="9a577-107">Service providers use the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="9a577-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a577-108">Properties</span></span>
<span data-ttu-id="9a577-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a577-109">Property</span></span>|<span data-ttu-id="9a577-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a577-110">Type</span></span>|<span data-ttu-id="9a577-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a577-111">Description</span></span>
----|--|---
|<span data-ttu-id="9a577-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="9a577-112">customKeyIdentifier</span></span>|<span data-ttu-id="9a577-113">Binário</span><span class="sxs-lookup"><span data-stu-id="9a577-113">Binary</span></span>| <span data-ttu-id="9a577-114">Identificador de chave personalizado.</span><span class="sxs-lookup"><span data-stu-id="9a577-114">Custom key identifier.</span></span> |
| <span data-ttu-id="9a577-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9a577-115">displayName</span></span> | <span data-ttu-id="9a577-116">String</span><span class="sxs-lookup"><span data-stu-id="9a577-116">String</span></span> | <span data-ttu-id="9a577-117">O nome amigável da chave.</span><span class="sxs-lookup"><span data-stu-id="9a577-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="9a577-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9a577-118">endDateTime</span></span>|<span data-ttu-id="9a577-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a577-119">DateTimeOffset</span></span>|<span data-ttu-id="9a577-120">A data e a hora em que a credencial expira.</span><span class="sxs-lookup"><span data-stu-id="9a577-120">The date and time at which the credential expires.</span></span> <span data-ttu-id="9a577-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9a577-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a577-122">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="9a577-122">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="9a577-123">keyId</span><span class="sxs-lookup"><span data-stu-id="9a577-123">keyId</span></span>|<span data-ttu-id="9a577-124">Guid</span><span class="sxs-lookup"><span data-stu-id="9a577-124">Guid</span></span>|<span data-ttu-id="9a577-125">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="9a577-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="9a577-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9a577-126">startDateTime</span></span>|<span data-ttu-id="9a577-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a577-127">DateTimeOffset</span></span>|<span data-ttu-id="9a577-128">A data e a hora em que a credencial se torna válida.</span><span class="sxs-lookup"><span data-stu-id="9a577-128">The date and time at which the credential becomes valid.</span></span> <span data-ttu-id="9a577-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9a577-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a577-130">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="9a577-130">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="9a577-131">tipo</span><span class="sxs-lookup"><span data-stu-id="9a577-131">type</span></span>|<span data-ttu-id="9a577-132">String</span><span class="sxs-lookup"><span data-stu-id="9a577-132">String</span></span>|<span data-ttu-id="9a577-133">O tipo de credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="9a577-133">The type of key credential.</span></span> <span data-ttu-id="9a577-134">"AsymmetricX509Cert".</span><span class="sxs-lookup"><span data-stu-id="9a577-134">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="9a577-135">usage</span><span class="sxs-lookup"><span data-stu-id="9a577-135">usage</span></span>|<span data-ttu-id="9a577-136">String</span><span class="sxs-lookup"><span data-stu-id="9a577-136">String</span></span>|<span data-ttu-id="9a577-137">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada.</span><span class="sxs-lookup"><span data-stu-id="9a577-137">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="9a577-138">Por exemplo, "Verificar".</span><span class="sxs-lookup"><span data-stu-id="9a577-138">For example, "Verify".</span></span>|
|<span data-ttu-id="9a577-139">chave</span><span class="sxs-lookup"><span data-stu-id="9a577-139">key</span></span>|<span data-ttu-id="9a577-140">Binário</span><span class="sxs-lookup"><span data-stu-id="9a577-140">Binary</span></span>| <span data-ttu-id="9a577-141">O valor da credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="9a577-141">The value for the key credential.</span></span> <span data-ttu-id="9a577-142">Deve ser um valor codificado de base-64.</span><span class="sxs-lookup"><span data-stu-id="9a577-142">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="9a577-143">thumbprint</span><span class="sxs-lookup"><span data-stu-id="9a577-143">thumbprint</span></span>| <span data-ttu-id="9a577-144">String</span><span class="sxs-lookup"><span data-stu-id="9a577-144">String</span></span> | <span data-ttu-id="9a577-145">O valor de impressão digital da chave.</span><span class="sxs-lookup"><span data-stu-id="9a577-145">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a577-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a577-146">JSON representation</span></span>

<span data-ttu-id="9a577-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9a577-147">Here is a JSON representation of the resource</span></span>

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

