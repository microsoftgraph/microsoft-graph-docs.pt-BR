---
title: Tipo de recurso pkcs12CertificateInformation
description: Representa as informações públicas de um certificado de cliente Pkcs12.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ada0d5d56d9fc785f6056862324aebd69d7358b3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509366"
---
# <a name="pkcs12certificateinformation-resource-type"></a><span data-ttu-id="23ebb-103">Tipo de recurso pkcs12CertificateInformation</span><span class="sxs-lookup"><span data-stu-id="23ebb-103">pkcs12CertificateInformation resource type</span></span>

<span data-ttu-id="23ebb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ebb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ebb-105">Representa as informações públicas de um certificado Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="23ebb-105">Represents the public information of a Pkcs12 certificate.</span></span>

## <a name="properties"></a><span data-ttu-id="23ebb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23ebb-106">Properties</span></span>

|<span data-ttu-id="23ebb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23ebb-107">Property</span></span>|<span data-ttu-id="23ebb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="23ebb-108">Type</span></span>|<span data-ttu-id="23ebb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ebb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ebb-110">isActive</span><span class="sxs-lookup"><span data-stu-id="23ebb-110">isActive</span></span>|<span data-ttu-id="23ebb-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="23ebb-111">Boolean</span></span>|  <span data-ttu-id="23ebb-112">Representa se o certificado é o certificado ativo a ser usado para chamar o conector de API.</span><span class="sxs-lookup"><span data-stu-id="23ebb-112">Represents whether the certificate is the active certificate to be used for calling the API connector.</span></span> <span data-ttu-id="23ebb-113">O certificado ativo é o certificado carregado mais recentemente que ainda não expirou, mas cujo tempo de notBefore não está no passado.</span><span class="sxs-lookup"><span data-stu-id="23ebb-113">The active certificate is the most recently uploaded certificate which is not yet expired but whose notBefore time is in the past.</span></span>|
|<span data-ttu-id="23ebb-114">thumbprint</span><span class="sxs-lookup"><span data-stu-id="23ebb-114">thumbprint</span></span>|<span data-ttu-id="23ebb-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ebb-115">String</span></span>| <span data-ttu-id="23ebb-116">A impressão digital do certificado.</span><span class="sxs-lookup"><span data-stu-id="23ebb-116">The certificate thumbprint.</span></span> |
|<span data-ttu-id="23ebb-117">notAfter</span><span class="sxs-lookup"><span data-stu-id="23ebb-117">notAfter</span></span>|<span data-ttu-id="23ebb-118">Inteiro</span><span class="sxs-lookup"><span data-stu-id="23ebb-118">Integer</span></span>| <span data-ttu-id="23ebb-119">O certificado expirou.</span><span class="sxs-lookup"><span data-stu-id="23ebb-119">The certificate's expiry.</span></span> <span data-ttu-id="23ebb-120">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="23ebb-120">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|
|<span data-ttu-id="23ebb-121">notBefore</span><span class="sxs-lookup"><span data-stu-id="23ebb-121">notBefore</span></span>|<span data-ttu-id="23ebb-122">Inteiro</span><span class="sxs-lookup"><span data-stu-id="23ebb-122">Integer</span></span>| <span data-ttu-id="23ebb-123">O tempo de emissão do certificado (não antes).</span><span class="sxs-lookup"><span data-stu-id="23ebb-123">The certificate's issue time (not before).</span></span> <span data-ttu-id="23ebb-124">Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)</span><span class="sxs-lookup"><span data-stu-id="23ebb-124">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23ebb-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23ebb-125">JSON representation</span></span>

<span data-ttu-id="23ebb-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23ebb-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": true,
    "thumbprint": "string",
    "notAfter": 0000000000,
    "notBefore": 0000000000,
}
```
