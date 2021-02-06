---
title: Tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64461015136129de452227cb0a8de5c7180cfb32
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135091"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="29600-103">Tipo de recurso certificateAuthority</span><span class="sxs-lookup"><span data-stu-id="29600-103">certificateAuthority resource type</span></span>

<span data-ttu-id="29600-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29600-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29600-105">Representa uma autoridade de certificação.</span><span class="sxs-lookup"><span data-stu-id="29600-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="29600-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29600-106">Properties</span></span>

| <span data-ttu-id="29600-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29600-107">Property</span></span>     | <span data-ttu-id="29600-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="29600-108">Type</span></span>        | <span data-ttu-id="29600-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29600-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29600-110">certificado</span><span class="sxs-lookup"><span data-stu-id="29600-110">certificate</span></span>|<span data-ttu-id="29600-111">Binário</span><span class="sxs-lookup"><span data-stu-id="29600-111">Binary</span></span>|<span data-ttu-id="29600-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29600-112">Required.</span></span> <span data-ttu-id="29600-113">A cadeia de caracteres codificada em base64 que representa o certificado público.</span><span class="sxs-lookup"><span data-stu-id="29600-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="29600-114">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="29600-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="29600-115">String</span><span class="sxs-lookup"><span data-stu-id="29600-115">String</span></span>|<span data-ttu-id="29600-116">A URL da lista de certificados revogados.</span><span class="sxs-lookup"><span data-stu-id="29600-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="29600-117">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="29600-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="29600-118">String</span><span class="sxs-lookup"><span data-stu-id="29600-118">String</span></span>|<span data-ttu-id="29600-119">A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de certificados revogados completos foi criada.</span><span class="sxs-lookup"><span data-stu-id="29600-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="29600-120">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="29600-120">isRootAuthority</span></span>|<span data-ttu-id="29600-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="29600-121">Boolean</span></span>|<span data-ttu-id="29600-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29600-122">Required.</span></span> <span data-ttu-id="29600-123">**true** se o certificado confiável for uma autoridade raiz, **false** se o certificado confiável for uma autoridade intermediária.</span><span class="sxs-lookup"><span data-stu-id="29600-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="29600-124">emissor</span><span class="sxs-lookup"><span data-stu-id="29600-124">issuer</span></span>|<span data-ttu-id="29600-125">String</span><span class="sxs-lookup"><span data-stu-id="29600-125">String</span></span>|<span data-ttu-id="29600-126">O emissor do certificado, calculado a partir do valor **do** certificado.</span><span class="sxs-lookup"><span data-stu-id="29600-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="29600-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29600-127">Read-only.</span></span> |
|<span data-ttu-id="29600-128">issuerSki</span><span class="sxs-lookup"><span data-stu-id="29600-128">issuerSki</span></span>|<span data-ttu-id="29600-129">String</span><span class="sxs-lookup"><span data-stu-id="29600-129">String</span></span>|<span data-ttu-id="29600-130">O identificador da chave de assunto do certificado, calculado a partir do valor **do** certificado.</span><span class="sxs-lookup"><span data-stu-id="29600-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="29600-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29600-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29600-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29600-132">JSON representation</span></span>

<span data-ttu-id="29600-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29600-133">The following is a JSON representation of the resource.</span></span>

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

