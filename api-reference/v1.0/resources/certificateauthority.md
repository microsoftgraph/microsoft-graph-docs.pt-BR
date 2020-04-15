---
title: tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4c8d97f6cbbb789e99ad177c8c90f308a90d6381
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451632"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="b2bca-103">tipo de recurso certificateAuthority</span><span class="sxs-lookup"><span data-stu-id="b2bca-103">certificateAuthority resource type</span></span>

<span data-ttu-id="b2bca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2bca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2bca-105">Representa uma autoridade de certificação.</span><span class="sxs-lookup"><span data-stu-id="b2bca-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="b2bca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2bca-106">Properties</span></span>

| <span data-ttu-id="b2bca-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2bca-107">Property</span></span>     | <span data-ttu-id="b2bca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2bca-108">Type</span></span>        | <span data-ttu-id="b2bca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2bca-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2bca-110">certificado</span><span class="sxs-lookup"><span data-stu-id="b2bca-110">certificate</span></span>|<span data-ttu-id="b2bca-111">Binário</span><span class="sxs-lookup"><span data-stu-id="b2bca-111">Binary</span></span>|<span data-ttu-id="b2bca-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2bca-112">Required.</span></span> <span data-ttu-id="b2bca-113">A cadeia de caracteres codificada em base64 que representa o certificado público.</span><span class="sxs-lookup"><span data-stu-id="b2bca-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="b2bca-114">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="b2bca-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="b2bca-115">String</span><span class="sxs-lookup"><span data-stu-id="b2bca-115">String</span></span>|<span data-ttu-id="b2bca-116">A URL da lista de certificados revogados.</span><span class="sxs-lookup"><span data-stu-id="b2bca-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="b2bca-117">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="b2bca-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="b2bca-118">String</span><span class="sxs-lookup"><span data-stu-id="b2bca-118">String</span></span>|<span data-ttu-id="b2bca-119">A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de revocaton de certificados completo foi criada.</span><span class="sxs-lookup"><span data-stu-id="b2bca-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="b2bca-120">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="b2bca-120">isRootAuthority</span></span>|<span data-ttu-id="b2bca-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2bca-121">Boolean</span></span>|<span data-ttu-id="b2bca-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2bca-122">Required.</span></span> <span data-ttu-id="b2bca-123">**true** se o certificado confiável é uma autoridade raiz, **false** se o certificado confiável é uma autoridade intermediária.</span><span class="sxs-lookup"><span data-stu-id="b2bca-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="b2bca-124">emissor</span><span class="sxs-lookup"><span data-stu-id="b2bca-124">issuer</span></span>|<span data-ttu-id="b2bca-125">String</span><span class="sxs-lookup"><span data-stu-id="b2bca-125">String</span></span>|<span data-ttu-id="b2bca-126">O emissor do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="b2bca-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="b2bca-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2bca-127">Read-only.</span></span> |
|<span data-ttu-id="b2bca-128">issuerSki</span><span class="sxs-lookup"><span data-stu-id="b2bca-128">issuerSki</span></span>|<span data-ttu-id="b2bca-129">String</span><span class="sxs-lookup"><span data-stu-id="b2bca-129">String</span></span>|<span data-ttu-id="b2bca-130">O identificador de chave de entidade do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="b2bca-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="b2bca-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2bca-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2bca-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2bca-132">JSON representation</span></span>

<span data-ttu-id="b2bca-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2bca-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->