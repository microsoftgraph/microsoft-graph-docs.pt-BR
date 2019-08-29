---
title: tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf88364ffd8f06783ef98ac32276d948fc6b1791
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667617"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="d66bb-103">tipo de recurso certificateAuthority</span><span class="sxs-lookup"><span data-stu-id="d66bb-103">certificateAuthority resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66bb-104">Representa uma autoridade de certificação.</span><span class="sxs-lookup"><span data-stu-id="d66bb-104">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="d66bb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d66bb-105">Properties</span></span>

| <span data-ttu-id="d66bb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d66bb-106">Property</span></span>     | <span data-ttu-id="d66bb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d66bb-107">Type</span></span>        | <span data-ttu-id="d66bb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d66bb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d66bb-109">certificado</span><span class="sxs-lookup"><span data-stu-id="d66bb-109">certificate</span></span>|<span data-ttu-id="d66bb-110">Binário</span><span class="sxs-lookup"><span data-stu-id="d66bb-110">Binary</span></span>|<span data-ttu-id="d66bb-111">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d66bb-111">Required.</span></span> <span data-ttu-id="d66bb-112">A cadeia de caracteres codificada em base64 que representa o certificado público.</span><span class="sxs-lookup"><span data-stu-id="d66bb-112">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="d66bb-113">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="d66bb-113">certificateRevocationListUrl</span></span>|<span data-ttu-id="d66bb-114">String</span><span class="sxs-lookup"><span data-stu-id="d66bb-114">String</span></span>|<span data-ttu-id="d66bb-115">A URL da lista de certificados revogados.</span><span class="sxs-lookup"><span data-stu-id="d66bb-115">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="d66bb-116">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="d66bb-116">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="d66bb-117">String</span><span class="sxs-lookup"><span data-stu-id="d66bb-117">String</span></span>|<span data-ttu-id="d66bb-118">A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de revocaton de certificados completo foi criada.</span><span class="sxs-lookup"><span data-stu-id="d66bb-118">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="d66bb-119">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="d66bb-119">isRootAuthority</span></span>|<span data-ttu-id="d66bb-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="d66bb-120">Boolean</span></span>|<span data-ttu-id="d66bb-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d66bb-121">Required.</span></span> <span data-ttu-id="d66bb-122">**true** se o certificado confiável é uma autoridade raiz, **false** se o certificado confiável é uma autoridade intermediária.</span><span class="sxs-lookup"><span data-stu-id="d66bb-122">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="d66bb-123">emissor</span><span class="sxs-lookup"><span data-stu-id="d66bb-123">issuer</span></span>|<span data-ttu-id="d66bb-124">String</span><span class="sxs-lookup"><span data-stu-id="d66bb-124">String</span></span>|<span data-ttu-id="d66bb-125">O emissor do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="d66bb-125">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="d66bb-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d66bb-126">Read-only.</span></span> |
|<span data-ttu-id="d66bb-127">issuerSki</span><span class="sxs-lookup"><span data-stu-id="d66bb-127">issuerSki</span></span>|<span data-ttu-id="d66bb-128">String</span><span class="sxs-lookup"><span data-stu-id="d66bb-128">String</span></span>|<span data-ttu-id="d66bb-129">O identificador de chave de entidade do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="d66bb-129">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="d66bb-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d66bb-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d66bb-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d66bb-131">JSON representation</span></span>

<span data-ttu-id="d66bb-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d66bb-132">The following is a JSON representation of the resource.</span></span>

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