---
title: tipo de recurso verifiedCustomDomainCertificatesMetadata
description: Representa os metadados cerificados personalizados para um aplicativo local publicado por meio do Proxy de Aplicativo.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: eab6823bdd3ed6a822cbeabdebf0aedfb654b769
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721429"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="b6a89-103">tipo de recurso verifiedCustomDomainCertificatesMetadata</span><span class="sxs-lookup"><span data-stu-id="b6a89-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="b6a89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a89-105">Representa os metadados de certificado de domínio personalizados para o [recurso onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com Proxy de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6a89-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="b6a89-106">Usar um domínio personalizado permite que você use seu próprio nome de domínio em vez do domínio padrão, msappproxy.net, para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6a89-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="b6a89-107">Para saber mais, confira [Domínios personalizados no Proxy de Aplicativo do Azure AD.](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)</span><span class="sxs-lookup"><span data-stu-id="b6a89-107">To learn more see, [Custom domains in Azure AD Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="b6a89-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6a89-108">Properties</span></span>

| <span data-ttu-id="b6a89-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6a89-109">Property</span></span>     | <span data-ttu-id="b6a89-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6a89-110">Type</span></span>        | <span data-ttu-id="b6a89-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a89-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6a89-112">expiryDate</span><span class="sxs-lookup"><span data-stu-id="b6a89-112">expiryDate</span></span>|<span data-ttu-id="b6a89-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6a89-113">DateTimeOffset</span></span>| <span data-ttu-id="b6a89-114">A data de expiração do certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="b6a89-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="b6a89-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b6a89-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6a89-116">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b6a89-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
|<span data-ttu-id="b6a89-117">issueDate</span><span class="sxs-lookup"><span data-stu-id="b6a89-117">issueDate</span></span>|<span data-ttu-id="b6a89-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6a89-118">DateTimeOffset</span></span>| <span data-ttu-id="b6a89-119">A data de emissão do domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="b6a89-119">The issue date of the custom domain.</span></span> <span data-ttu-id="b6a89-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b6a89-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6a89-121">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b6a89-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
|<span data-ttu-id="b6a89-122">issuerName</span><span class="sxs-lookup"><span data-stu-id="b6a89-122">issuerName</span></span>|<span data-ttu-id="b6a89-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6a89-123">String</span></span>| <span data-ttu-id="b6a89-124">O nome do emissor do certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="b6a89-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="b6a89-125">SubjectName</span><span class="sxs-lookup"><span data-stu-id="b6a89-125">subjectName</span></span>|<span data-ttu-id="b6a89-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6a89-126">String</span></span>| <span data-ttu-id="b6a89-127">O nome do assunto do certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="b6a89-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="b6a89-128">thumbprint</span><span class="sxs-lookup"><span data-stu-id="b6a89-128">thumbprint</span></span>|<span data-ttu-id="b6a89-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6a89-129">String</span></span>| <span data-ttu-id="b6a89-130">A impressão digital associada ao certificado de domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="b6a89-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6a89-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6a89-131">JSON representation</span></span>

<span data-ttu-id="b6a89-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6a89-132">The following is a JSON representation of the resource.</span></span>

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
