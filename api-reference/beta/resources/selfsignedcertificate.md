---
title: Tipo de recurso selfSignedCertificate
description: Contém informações sobre a parte pública de um certificado de assinatura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: a32720520c804d13048babe8a779132780abc782
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266861"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="75387-103">Tipo de recurso selfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="75387-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="75387-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75387-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75387-105">Contém a parte pública de um certificado de assinatura.</span><span class="sxs-lookup"><span data-stu-id="75387-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="75387-106">É o tipo de retorno da ação [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="75387-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="75387-107">Os provedores de serviços usam a parte pública do certificado de assinatura para validar o emissor do token.</span><span class="sxs-lookup"><span data-stu-id="75387-107">Service providers use the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="75387-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75387-108">Properties</span></span>
<span data-ttu-id="75387-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75387-109">Property</span></span>|<span data-ttu-id="75387-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75387-110">Type</span></span>|<span data-ttu-id="75387-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75387-111">Description</span></span>
----|--|---
|<span data-ttu-id="75387-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="75387-112">customKeyIdentifier</span></span>|<span data-ttu-id="75387-113">Binário</span><span class="sxs-lookup"><span data-stu-id="75387-113">Binary</span></span>| <span data-ttu-id="75387-114">Identificador de chave personalizado.</span><span class="sxs-lookup"><span data-stu-id="75387-114">Custom key identifier.</span></span> |
| <span data-ttu-id="75387-115">displayName</span><span class="sxs-lookup"><span data-stu-id="75387-115">displayName</span></span> | <span data-ttu-id="75387-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75387-116">String</span></span> | <span data-ttu-id="75387-117">O nome amigável da chave.</span><span class="sxs-lookup"><span data-stu-id="75387-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="75387-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="75387-118">endDateTime</span></span>|<span data-ttu-id="75387-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75387-119">DateTimeOffset</span></span>|<span data-ttu-id="75387-120">A data e a hora em que a credencial expira.</span><span class="sxs-lookup"><span data-stu-id="75387-120">The date and time at which the credential expires.</span></span> <span data-ttu-id="75387-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="75387-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75387-122">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="75387-122">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="75387-123">keyId</span><span class="sxs-lookup"><span data-stu-id="75387-123">keyId</span></span>|<span data-ttu-id="75387-124">Guid</span><span class="sxs-lookup"><span data-stu-id="75387-124">Guid</span></span>|<span data-ttu-id="75387-125">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="75387-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="75387-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="75387-126">startDateTime</span></span>|<span data-ttu-id="75387-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75387-127">DateTimeOffset</span></span>|<span data-ttu-id="75387-128">A data e a hora em que a credencial se torna válida.</span><span class="sxs-lookup"><span data-stu-id="75387-128">The date and time at which the credential becomes valid.</span></span> <span data-ttu-id="75387-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="75387-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75387-130">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="75387-130">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="75387-131">tipo</span><span class="sxs-lookup"><span data-stu-id="75387-131">type</span></span>|<span data-ttu-id="75387-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75387-132">String</span></span>|<span data-ttu-id="75387-133">O tipo de credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="75387-133">The type of key credential.</span></span> <span data-ttu-id="75387-134">"AsymmetricX509Cert".</span><span class="sxs-lookup"><span data-stu-id="75387-134">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="75387-135">usage</span><span class="sxs-lookup"><span data-stu-id="75387-135">usage</span></span>|<span data-ttu-id="75387-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75387-136">String</span></span>|<span data-ttu-id="75387-137">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada.</span><span class="sxs-lookup"><span data-stu-id="75387-137">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="75387-138">Por exemplo, "Verificar".</span><span class="sxs-lookup"><span data-stu-id="75387-138">For example, "Verify".</span></span>|
|<span data-ttu-id="75387-139">chave</span><span class="sxs-lookup"><span data-stu-id="75387-139">key</span></span>|<span data-ttu-id="75387-140">Binário</span><span class="sxs-lookup"><span data-stu-id="75387-140">Binary</span></span>| <span data-ttu-id="75387-141">O valor da credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="75387-141">The value for the key credential.</span></span> <span data-ttu-id="75387-142">Deve ser um valor codificado de base-64.</span><span class="sxs-lookup"><span data-stu-id="75387-142">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="75387-143">thumbprint</span><span class="sxs-lookup"><span data-stu-id="75387-143">thumbprint</span></span>| <span data-ttu-id="75387-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75387-144">String</span></span> | <span data-ttu-id="75387-145">O valor de impressão digital da chave.</span><span class="sxs-lookup"><span data-stu-id="75387-145">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75387-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75387-146">JSON representation</span></span>

<span data-ttu-id="75387-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="75387-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "string (binary)",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "string (binary)",
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

