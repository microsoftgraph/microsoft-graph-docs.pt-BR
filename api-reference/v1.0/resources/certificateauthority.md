---
title: tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50555ff47d81d96def360fe55fe8684f6ff07994
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531949"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="6fe8d-103">tipo de recurso certificateAuthority</span><span class="sxs-lookup"><span data-stu-id="6fe8d-103">certificateAuthority resource type</span></span>

<span data-ttu-id="6fe8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fe8d-105">Representa uma autoridade de certificação.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="6fe8d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fe8d-106">Properties</span></span>

| <span data-ttu-id="6fe8d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fe8d-107">Property</span></span>     | <span data-ttu-id="6fe8d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fe8d-108">Type</span></span>        | <span data-ttu-id="6fe8d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fe8d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fe8d-110">certificado</span><span class="sxs-lookup"><span data-stu-id="6fe8d-110">certificate</span></span>|<span data-ttu-id="6fe8d-111">Binário</span><span class="sxs-lookup"><span data-stu-id="6fe8d-111">Binary</span></span>|<span data-ttu-id="6fe8d-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-112">Required.</span></span> <span data-ttu-id="6fe8d-113">A cadeia de caracteres codificada em base64 que representa o certificado público.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="6fe8d-114">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="6fe8d-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="6fe8d-115">String</span><span class="sxs-lookup"><span data-stu-id="6fe8d-115">String</span></span>|<span data-ttu-id="6fe8d-116">A URL da lista de certificados revogados.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="6fe8d-117">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="6fe8d-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="6fe8d-118">String</span><span class="sxs-lookup"><span data-stu-id="6fe8d-118">String</span></span>|<span data-ttu-id="6fe8d-119">A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de revocaton de certificados completo foi criada.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="6fe8d-120">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="6fe8d-120">isRootAuthority</span></span>|<span data-ttu-id="6fe8d-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="6fe8d-121">Boolean</span></span>|<span data-ttu-id="6fe8d-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-122">Required.</span></span> <span data-ttu-id="6fe8d-123">**true** se o certificado confiável é uma autoridade raiz, **false** se o certificado confiável é uma autoridade intermediária.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="6fe8d-124">emissor</span><span class="sxs-lookup"><span data-stu-id="6fe8d-124">issuer</span></span>|<span data-ttu-id="6fe8d-125">String</span><span class="sxs-lookup"><span data-stu-id="6fe8d-125">String</span></span>|<span data-ttu-id="6fe8d-126">O emissor do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="6fe8d-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="6fe8d-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-127">Read-only.</span></span> |
|<span data-ttu-id="6fe8d-128">issuerSki</span><span class="sxs-lookup"><span data-stu-id="6fe8d-128">issuerSki</span></span>|<span data-ttu-id="6fe8d-129">String</span><span class="sxs-lookup"><span data-stu-id="6fe8d-129">String</span></span>|<span data-ttu-id="6fe8d-130">O identificador de chave de entidade do certificado, calculado com base no valor do **certificado** .</span><span class="sxs-lookup"><span data-stu-id="6fe8d-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="6fe8d-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fe8d-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fe8d-132">JSON representation</span></span>

<span data-ttu-id="6fe8d-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-133">The following is a JSON representation of the resource.</span></span>

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