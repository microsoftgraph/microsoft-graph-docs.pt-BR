---
title: Tipo de recurso apiAuthenticationConfigurationBase
description: Representa o tipo base de configuração de autenticação usado para chamar uma API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 915e1c0c26cee173991d75bc46a1a0230844d2ec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507963"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a><span data-ttu-id="63a8b-103">Tipo de recurso apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="63a8b-103">apiAuthenticationConfigurationBase resource type</span></span>

<span data-ttu-id="63a8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63a8b-105">O tipo base para manter informações de autenticação para chamar uma API.</span><span class="sxs-lookup"><span data-stu-id="63a8b-105">The base type to hold authentication information for calling an API.</span></span>

<span data-ttu-id="63a8b-106">Os tipos derivados incluem:</span><span class="sxs-lookup"><span data-stu-id="63a8b-106">Derived types include:</span></span>
- <span data-ttu-id="63a8b-107">[basicAuthentication para](basicauthentication.md) autenticação básica HTTP</span><span class="sxs-lookup"><span data-stu-id="63a8b-107">[basicAuthentication](basicauthentication.md) for HTTP basic authentication</span></span>
- <span data-ttu-id="63a8b-108">[pkcs12certificate para autenticação](pkcs12certificate.md) de certificado do cliente (usado para criar ou carregar conectores de API)</span><span class="sxs-lookup"><span data-stu-id="63a8b-108">[pkcs12certificate](pkcs12certificate.md) for client certificate authentication (used for API connector create or upload)</span></span>
- <span data-ttu-id="63a8b-109">[clientCertificateAuthentication para](pkcs12certificate.md) autenticação de certificado de cliente (usado para buscar os certificados do cliente de um conector de API)</span><span class="sxs-lookup"><span data-stu-id="63a8b-109">[clientCertificateAuthentication](pkcs12certificate.md) for client certificate authentication (used for fetching the client certificates of an API connector)</span></span>

## <a name="properties"></a><span data-ttu-id="63a8b-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63a8b-110">Properties</span></span>

|<span data-ttu-id="63a8b-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63a8b-111">Property</span></span>|<span data-ttu-id="63a8b-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="63a8b-112">Type</span></span>|<span data-ttu-id="63a8b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="63a8b-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="63a8b-114">Relações</span><span class="sxs-lookup"><span data-stu-id="63a8b-114">Relationships</span></span>

<span data-ttu-id="63a8b-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63a8b-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63a8b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63a8b-116">JSON representation</span></span>

<span data-ttu-id="63a8b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63a8b-117">The following is a JSON representation of the resource.</span></span>
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
