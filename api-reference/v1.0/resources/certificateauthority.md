---
title: tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 030e0fbe8fcae0408f51c20882d49e50d825cdb8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539292"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="0b846-103">tipo de recurso certificateAuthority</span><span class="sxs-lookup"><span data-stu-id="0b846-103">certificateAuthority resource type</span></span>

<span data-ttu-id="0b846-104">Representa uma autoridade de certificação.</span><span class="sxs-lookup"><span data-stu-id="0b846-104">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="0b846-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b846-105">Properties</span></span>

| <span data-ttu-id="0b846-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b846-106">Property</span></span>     | <span data-ttu-id="0b846-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b846-107">Type</span></span>        | <span data-ttu-id="0b846-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b846-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b846-109">certificado</span><span class="sxs-lookup"><span data-stu-id="0b846-109">certificate</span></span>|<span data-ttu-id="0b846-110">Binário</span><span class="sxs-lookup"><span data-stu-id="0b846-110">Binary</span></span>|<span data-ttu-id="0b846-111">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b846-111">Required.</span></span> <span data-ttu-id="0b846-112">A cadeia de caracteres codificada em base64 que representa o certificado público.</span><span class="sxs-lookup"><span data-stu-id="0b846-112">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="0b846-113">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="0b846-113">certificateRevocationListUrl</span></span>|<span data-ttu-id="0b846-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b846-114">String</span></span>|<span data-ttu-id="0b846-115">A URL da lista de certificados revogados.</span><span class="sxs-lookup"><span data-stu-id="0b846-115">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="0b846-116">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="0b846-116">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="0b846-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b846-117">String</span></span>|<span data-ttu-id="0b846-118">A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de revocaton de certificados completo foi criada.</span><span class="sxs-lookup"><span data-stu-id="0b846-118">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="0b846-119">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="0b846-119">isRootAuthority</span></span>|<span data-ttu-id="0b846-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b846-120">Boolean</span></span>|<span data-ttu-id="0b846-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b846-121">Required.</span></span> <span data-ttu-id="0b846-122">**true** se o certificado confiável é uma autoridade raiz, **false** se o certificado confiável é uma autoridade intermediária.</span><span class="sxs-lookup"><span data-stu-id="0b846-122">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="0b846-123">emissor</span><span class="sxs-lookup"><span data-stu-id="0b846-123">issuer</span></span>|<span data-ttu-id="0b846-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b846-124">String</span></span>|<span data-ttu-id="0b846-125">O emissor do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="0b846-125">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="0b846-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b846-126">Read-only.</span></span> |
|<span data-ttu-id="0b846-127">issuerSki</span><span class="sxs-lookup"><span data-stu-id="0b846-127">issuerSki</span></span>|<span data-ttu-id="0b846-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b846-128">String</span></span>|<span data-ttu-id="0b846-129">O identificador de chave de entidade do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="0b846-129">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="0b846-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b846-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b846-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b846-131">JSON representation</span></span>

<span data-ttu-id="0b846-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b846-132">The following is a JSON representation of the resource.</span></span>

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