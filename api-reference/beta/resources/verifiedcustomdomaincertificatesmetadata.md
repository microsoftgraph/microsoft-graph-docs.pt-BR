---
title: tipo de recurso verifiedCustomDomainCertificatesMetadata
description: Representa os metadados de criar certificado personalizados para um aplicativo local publicado por meio do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4268c7d9faba8e744f7a6bd6a674ff680cb24346
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556374"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="57d49-103">tipo de recurso verifiedCustomDomainCertificatesMetadata</span><span class="sxs-lookup"><span data-stu-id="57d49-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="57d49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57d49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57d49-105">Representa os metadados do certificado de domínio personalizado para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o proxy de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57d49-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="57d49-106">Usar um domínio personalizado permite que você use seu próprio nome de domínio em vez do domínio padrão, msappproxy.net, para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57d49-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="57d49-107">Para saber mais, confira [domínios personalizados no proxy de aplicativo do Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span><span class="sxs-lookup"><span data-stu-id="57d49-107">To learn more see, [Custom domains in Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="57d49-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57d49-108">Properties</span></span>

| <span data-ttu-id="57d49-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57d49-109">Property</span></span>     | <span data-ttu-id="57d49-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="57d49-110">Type</span></span>        | <span data-ttu-id="57d49-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57d49-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57d49-112">expiryDate</span><span class="sxs-lookup"><span data-stu-id="57d49-112">expiryDate</span></span>|<span data-ttu-id="57d49-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d49-113">DateTimeOffset</span></span>| <span data-ttu-id="57d49-114">A data de expiração do certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="57d49-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="57d49-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="57d49-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="57d49-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="57d49-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="57d49-117">Emitido</span><span class="sxs-lookup"><span data-stu-id="57d49-117">issueDate</span></span>|<span data-ttu-id="57d49-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d49-118">DateTimeOffset</span></span>| <span data-ttu-id="57d49-119">A data de emissão do domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="57d49-119">The issue date of the custom domain.</span></span> <span data-ttu-id="57d49-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="57d49-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="57d49-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="57d49-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="57d49-122">issuerName</span><span class="sxs-lookup"><span data-stu-id="57d49-122">issuerName</span></span>|<span data-ttu-id="57d49-123">String</span><span class="sxs-lookup"><span data-stu-id="57d49-123">String</span></span>| <span data-ttu-id="57d49-124">O nome do emissor do certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="57d49-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="57d49-125">SubjectName</span><span class="sxs-lookup"><span data-stu-id="57d49-125">subjectName</span></span>|<span data-ttu-id="57d49-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57d49-126">String</span></span>| <span data-ttu-id="57d49-127">O nome da entidade do certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="57d49-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="57d49-128">identificação</span><span class="sxs-lookup"><span data-stu-id="57d49-128">thumbprint</span></span>|<span data-ttu-id="57d49-129">String</span><span class="sxs-lookup"><span data-stu-id="57d49-129">String</span></span>| <span data-ttu-id="57d49-130">A impressão digital associada ao certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="57d49-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57d49-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57d49-131">JSON representation</span></span>

<span data-ttu-id="57d49-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57d49-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "baseType": null
}-->

```json
{
  "expiryDate": "String (timestamp)",
  "issueDate": "String (timestamp)",
  "issuerName": "String",
  "subjectName": "String",
  "thumbprint": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedCustomDomainCertificatesMetadata resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->