---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd063ec70dd794ffb151036ea7bbbda090829343
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001248"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="ce2af-103">tipo de recurso iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="ce2af-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="ce2af-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce2af-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2af-106">Certificados de raiz confiável e PFX para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="ce2af-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="ce2af-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce2af-107">Properties</span></span>
|<span data-ttu-id="ce2af-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce2af-108">Property</span></span>|<span data-ttu-id="ce2af-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce2af-109">Type</span></span>|<span data-ttu-id="ce2af-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce2af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2af-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ce2af-111">trustedRootCertificate</span></span>|<span data-ttu-id="ce2af-112">Binária</span><span class="sxs-lookup"><span data-stu-id="ce2af-112">Binary</span></span>|<span data-ttu-id="ce2af-113">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="ce2af-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="ce2af-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="ce2af-114">certFileName</span></span>|<span data-ttu-id="ce2af-115">String</span><span class="sxs-lookup"><span data-stu-id="ce2af-115">String</span></span>|<span data-ttu-id="ce2af-116">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ce2af-116">File name to display in UI.</span></span>|
|<span data-ttu-id="ce2af-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="ce2af-117">certificationAuthority</span></span>|<span data-ttu-id="ce2af-118">String</span><span class="sxs-lookup"><span data-stu-id="ce2af-118">String</span></span>|<span data-ttu-id="ce2af-119">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="ce2af-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="ce2af-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="ce2af-120">certificationAuthorityName</span></span>|<span data-ttu-id="ce2af-121">String</span><span class="sxs-lookup"><span data-stu-id="ce2af-121">String</span></span>|<span data-ttu-id="ce2af-122">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="ce2af-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="ce2af-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="ce2af-123">certificateTemplateName</span></span>|<span data-ttu-id="ce2af-124">String</span><span class="sxs-lookup"><span data-stu-id="ce2af-124">String</span></span>|<span data-ttu-id="ce2af-125">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="ce2af-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="ce2af-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ce2af-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="ce2af-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ce2af-127">Int32</span></span>|<span data-ttu-id="ce2af-128">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="ce2af-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ce2af-129">Valores válidos de 1 a 99</span><span class="sxs-lookup"><span data-stu-id="ce2af-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="ce2af-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ce2af-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ce2af-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ce2af-131">Int32</span></span>|<span data-ttu-id="ce2af-132">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ce2af-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="ce2af-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce2af-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ce2af-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce2af-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ce2af-135">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ce2af-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ce2af-136">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ce2af-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce2af-137">Relações</span><span class="sxs-lookup"><span data-stu-id="ce2af-137">Relationships</span></span>
<span data-ttu-id="ce2af-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce2af-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce2af-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce2af-139">JSON Representation</span></span>
<span data-ttu-id="ce2af-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce2af-140">Here is a JSON representation of the resource.</span></span>
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





