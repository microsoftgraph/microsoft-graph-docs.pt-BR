---
title: Tipo de recurso pkcs12CertificateInformation
description: Representa as informações públicas de um certificado de cliente Pkcs12.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c649021d8fe66530edb794a859eecd8ed08def3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882781"
---
# <a name="pkcs12certificateinformation-resource-type"></a><span data-ttu-id="1efc1-103">Tipo de recurso pkcs12CertificateInformation</span><span class="sxs-lookup"><span data-stu-id="1efc1-103">pkcs12CertificateInformation resource type</span></span>

<span data-ttu-id="1efc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1efc1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1efc1-105">Representa as informações públicas de um certificado Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="1efc1-105">Represents the public information of a Pkcs12 certificate.</span></span>

## <a name="properties"></a><span data-ttu-id="1efc1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1efc1-106">Properties</span></span>

|<span data-ttu-id="1efc1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1efc1-107">Property</span></span>|<span data-ttu-id="1efc1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1efc1-108">Type</span></span>|<span data-ttu-id="1efc1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1efc1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efc1-110">isActive</span><span class="sxs-lookup"><span data-stu-id="1efc1-110">isActive</span></span>|<span data-ttu-id="1efc1-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="1efc1-111">Boolean</span></span>|  <span data-ttu-id="1efc1-112">Representa se o certificado é o certificado ativo a ser usado para chamar o conector de API.</span><span class="sxs-lookup"><span data-stu-id="1efc1-112">Represents whether the certificate is the active certificate to be used for calling the API connector.</span></span> <span data-ttu-id="1efc1-113">O certificado ativo é o certificado carregado mais recentemente que ainda não expirou, mas cujo tempo de notBefore não está no passado.</span><span class="sxs-lookup"><span data-stu-id="1efc1-113">The active certificate is the most recently uploaded certificate which is not yet expired but whose notBefore time is in the past.</span></span>|
|<span data-ttu-id="1efc1-114">thumbprint</span><span class="sxs-lookup"><span data-stu-id="1efc1-114">thumbprint</span></span>|<span data-ttu-id="1efc1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1efc1-115">String</span></span>| <span data-ttu-id="1efc1-116">A impressão digital do certificado.</span><span class="sxs-lookup"><span data-stu-id="1efc1-116">The certificate thumbprint.</span></span> |
|<span data-ttu-id="1efc1-117">notAfter</span><span class="sxs-lookup"><span data-stu-id="1efc1-117">notAfter</span></span>|<span data-ttu-id="1efc1-118">Inteiro</span><span class="sxs-lookup"><span data-stu-id="1efc1-118">Integer</span></span>| <span data-ttu-id="1efc1-119">O certificado expirou.</span><span class="sxs-lookup"><span data-stu-id="1efc1-119">The certificate's expiry.</span></span> <span data-ttu-id="1efc1-120">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="1efc1-120">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|
|<span data-ttu-id="1efc1-121">notBefore</span><span class="sxs-lookup"><span data-stu-id="1efc1-121">notBefore</span></span>|<span data-ttu-id="1efc1-122">Inteiro</span><span class="sxs-lookup"><span data-stu-id="1efc1-122">Integer</span></span>| <span data-ttu-id="1efc1-123">O tempo de emissão do certificado (não antes).</span><span class="sxs-lookup"><span data-stu-id="1efc1-123">The certificate's issue time (not before).</span></span> <span data-ttu-id="1efc1-124">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="1efc1-124">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1efc1-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1efc1-125">JSON representation</span></span>

<span data-ttu-id="1efc1-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1efc1-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": "Boolean",
    "thumbprint": "String",
    "notAfter": "DateTime",
    "notBefore": "DateTime"
}
```
