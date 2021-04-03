---
title: Tipo de recurso clientCertificateAuthentication
description: Representa a configuração para buscar um clientCertificateAuthentication em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e88a1de011fb975afae49d53b8707b95e16157c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509376"
---
# <a name="clientcertificateauthentication-resource-type"></a><span data-ttu-id="9f0d2-103">Tipo de recurso clientCertificateAuthentication</span><span class="sxs-lookup"><span data-stu-id="9f0d2-103">clientCertificateAuthentication resource type</span></span>

<span data-ttu-id="9f0d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f0d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f0d2-105">Um tipo derivado de apiAuthenticationConfigurationBase que é usado para representar a autenticação de certificado de cliente baseada em Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="9f0d2-105">A type derived from apiAuthenticationConfigurationBase which is used to represent Pkcs12 based client certificate authentication.</span></span> <span data-ttu-id="9f0d2-106">Isso é usado para recuperar as propriedades públicas de certificados carregados.</span><span class="sxs-lookup"><span data-stu-id="9f0d2-106">This is used to retrieve the public properties of uploaded certificates.</span></span>

<span data-ttu-id="9f0d2-107">Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="9f0d2-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9f0d2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f0d2-108">Properties</span></span>

|<span data-ttu-id="9f0d2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f0d2-109">Property</span></span>|<span data-ttu-id="9f0d2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f0d2-110">Type</span></span>|<span data-ttu-id="9f0d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f0d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f0d2-112">certificateList</span><span class="sxs-lookup"><span data-stu-id="9f0d2-112">certificateList</span></span>| <span data-ttu-id="9f0d2-113">[Coleção pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md)</span><span class="sxs-lookup"><span data-stu-id="9f0d2-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) collection</span></span>| <span data-ttu-id="9f0d2-114">A lista de certificados carregados para este conector de API.</span><span class="sxs-lookup"><span data-stu-id="9f0d2-114">The list of certificates uploaded for this API connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f0d2-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f0d2-115">JSON representation</span></span>

<span data-ttu-id="9f0d2-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f0d2-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.clientCertificateAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
  "certificateList": "Collection(microsoft.graph.pkcs12CertificateInformation)",
}
```
