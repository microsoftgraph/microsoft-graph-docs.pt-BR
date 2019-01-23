---
title: tipo de recurso de iosEduCertificateSettings
description: Certificados raiz e PFX confiáveis para iOS EDU.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d23b379dea7a75e4ae79029845cd6e9f956503c0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423549"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="9d672-103">tipo de recurso de iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="9d672-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="9d672-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d672-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9d672-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d672-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d672-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9d672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d672-107">Certificados raiz e PFX confiáveis para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="9d672-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="9d672-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d672-108">Properties</span></span>
|<span data-ttu-id="9d672-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d672-109">Property</span></span>|<span data-ttu-id="9d672-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d672-110">Type</span></span>|<span data-ttu-id="9d672-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d672-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d672-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9d672-112">trustedRootCertificate</span></span>|<span data-ttu-id="9d672-113">Binária</span><span class="sxs-lookup"><span data-stu-id="9d672-113">Binary</span></span>|<span data-ttu-id="9d672-114">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="9d672-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="9d672-115">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="9d672-115">certFileName</span></span>|<span data-ttu-id="9d672-116">String</span><span class="sxs-lookup"><span data-stu-id="9d672-116">String</span></span>|<span data-ttu-id="9d672-117">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="9d672-117">File name to display in UI.</span></span>|
|<span data-ttu-id="9d672-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="9d672-118">certificationAuthority</span></span>|<span data-ttu-id="9d672-119">String</span><span class="sxs-lookup"><span data-stu-id="9d672-119">String</span></span>|<span data-ttu-id="9d672-120">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="9d672-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="9d672-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="9d672-121">certificationAuthorityName</span></span>|<span data-ttu-id="9d672-122">String</span><span class="sxs-lookup"><span data-stu-id="9d672-122">String</span></span>|<span data-ttu-id="9d672-123">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="9d672-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="9d672-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="9d672-124">certificateTemplateName</span></span>|<span data-ttu-id="9d672-125">String</span><span class="sxs-lookup"><span data-stu-id="9d672-125">String</span></span>|<span data-ttu-id="9d672-126">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="9d672-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="9d672-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9d672-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="9d672-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9d672-128">Int32</span></span>|<span data-ttu-id="9d672-129">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="9d672-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9d672-130">Valores válidos 1 a 99</span><span class="sxs-lookup"><span data-stu-id="9d672-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="9d672-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9d672-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9d672-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9d672-132">Int32</span></span>|<span data-ttu-id="9d672-133">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="9d672-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="9d672-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9d672-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9d672-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9d672-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9d672-136">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="9d672-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9d672-137">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="9d672-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d672-138">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9d672-138">Relationships</span></span>
<span data-ttu-id="9d672-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d672-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d672-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d672-140">JSON Representation</span></span>
<span data-ttu-id="9d672-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d672-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```




