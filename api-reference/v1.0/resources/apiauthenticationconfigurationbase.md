---
title: Tipo de recurso apiAuthenticationConfigurationBase
description: Representa o tipo base de configuração de autenticação usado para chamar uma API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a9e48d38e7ad69d6790b3b9dddb85960c964ad91
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882802"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a><span data-ttu-id="86282-103">Tipo de recurso apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="86282-103">apiAuthenticationConfigurationBase resource type</span></span>

<span data-ttu-id="86282-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86282-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86282-105">O tipo base para manter informações de autenticação para chamar uma API.</span><span class="sxs-lookup"><span data-stu-id="86282-105">The base type to hold authentication information for calling an API.</span></span>

<span data-ttu-id="86282-106">Os tipos derivados incluem:</span><span class="sxs-lookup"><span data-stu-id="86282-106">Derived types include:</span></span>
- <span data-ttu-id="86282-107">[basicAuthentication para](basicauthentication.md) autenticação básica HTTP</span><span class="sxs-lookup"><span data-stu-id="86282-107">[basicAuthentication](basicauthentication.md) for HTTP basic authentication</span></span>
- <span data-ttu-id="86282-108">[pkcs12certificate para autenticação](pkcs12certificate.md) de certificado do cliente (usado para criar ou carregar conectores de API)</span><span class="sxs-lookup"><span data-stu-id="86282-108">[pkcs12certificate](pkcs12certificate.md) for client certificate authentication (used for API connector create or upload)</span></span>
- <span data-ttu-id="86282-109">[clientCertificateAuthentication para](pkcs12certificate.md) autenticação de certificado de cliente (usado para buscar os certificados do cliente de um conector de API)</span><span class="sxs-lookup"><span data-stu-id="86282-109">[clientCertificateAuthentication](pkcs12certificate.md) for client certificate authentication (used for fetching the client certificates of an API connector)</span></span>

## <a name="properties"></a><span data-ttu-id="86282-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86282-110">Properties</span></span>

|<span data-ttu-id="86282-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86282-111">Property</span></span>|<span data-ttu-id="86282-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="86282-112">Type</span></span>|<span data-ttu-id="86282-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="86282-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="86282-114">Relações</span><span class="sxs-lookup"><span data-stu-id="86282-114">Relationships</span></span>

<span data-ttu-id="86282-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86282-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86282-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86282-116">JSON representation</span></span>

<span data-ttu-id="86282-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86282-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
