---
title: Tipo de recurso clientCertificateAuthentication
description: Representa a configuração para recuperar um clientCertificateAuthentication.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69870b1160078495d3b9440260aab1f231041eef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882393"
---
# <a name="clientcertificateauthentication-resource-type"></a><span data-ttu-id="71fef-103">Tipo de recurso clientCertificateAuthentication</span><span class="sxs-lookup"><span data-stu-id="71fef-103">clientCertificateAuthentication resource type</span></span>

<span data-ttu-id="71fef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71fef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71fef-105">Um tipo derivado de apiAuthenticationConfigurationBase usado para representar uma autenticação de certificado cliente baseada em Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="71fef-105">A type derived from apiAuthenticationConfigurationBase that is used to represent a Pkcs12-based client certificate authentication.</span></span> <span data-ttu-id="71fef-106">Isso é usado para recuperar as propriedades públicas de certificados carregados.</span><span class="sxs-lookup"><span data-stu-id="71fef-106">This is used to retrieve the public properties of uploaded certificates.</span></span>

<span data-ttu-id="71fef-107">Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="71fef-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="71fef-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71fef-108">Properties</span></span>

|<span data-ttu-id="71fef-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71fef-109">Property</span></span>|<span data-ttu-id="71fef-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="71fef-110">Type</span></span>|<span data-ttu-id="71fef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71fef-112">certificateList</span><span class="sxs-lookup"><span data-stu-id="71fef-112">certificateList</span></span>| <span data-ttu-id="71fef-113">[Coleção pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md)</span><span class="sxs-lookup"><span data-stu-id="71fef-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) collection</span></span>| <span data-ttu-id="71fef-114">A lista de certificados carregados para este conector de API.</span><span class="sxs-lookup"><span data-stu-id="71fef-114">The list of certificates uploaded for this API connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71fef-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71fef-115">JSON representation</span></span>

<span data-ttu-id="71fef-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71fef-116">The following is a JSON representation of the resource.</span></span>
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
