---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30e7a68f76c60fafff9fc2b035a65a60307f775d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981465"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="0775a-103">tipo de recurso iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0775a-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="0775a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0775a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0775a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0775a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0775a-106">Certificados de raiz confiável e PFX para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="0775a-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="0775a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0775a-107">Properties</span></span>
|<span data-ttu-id="0775a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0775a-108">Property</span></span>|<span data-ttu-id="0775a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0775a-109">Type</span></span>|<span data-ttu-id="0775a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0775a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0775a-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0775a-111">trustedRootCertificate</span></span>|<span data-ttu-id="0775a-112">Binária</span><span class="sxs-lookup"><span data-stu-id="0775a-112">Binary</span></span>|<span data-ttu-id="0775a-113">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="0775a-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="0775a-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="0775a-114">certFileName</span></span>|<span data-ttu-id="0775a-115">String</span><span class="sxs-lookup"><span data-stu-id="0775a-115">String</span></span>|<span data-ttu-id="0775a-116">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="0775a-116">File name to display in UI.</span></span>|
|<span data-ttu-id="0775a-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="0775a-117">certificationAuthority</span></span>|<span data-ttu-id="0775a-118">String</span><span class="sxs-lookup"><span data-stu-id="0775a-118">String</span></span>|<span data-ttu-id="0775a-119">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="0775a-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="0775a-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="0775a-120">certificationAuthorityName</span></span>|<span data-ttu-id="0775a-121">String</span><span class="sxs-lookup"><span data-stu-id="0775a-121">String</span></span>|<span data-ttu-id="0775a-122">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="0775a-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="0775a-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="0775a-123">certificateTemplateName</span></span>|<span data-ttu-id="0775a-124">String</span><span class="sxs-lookup"><span data-stu-id="0775a-124">String</span></span>|<span data-ttu-id="0775a-125">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="0775a-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="0775a-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0775a-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="0775a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0775a-127">Int32</span></span>|<span data-ttu-id="0775a-128">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="0775a-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0775a-129">Valores válidos de 1 a 99</span><span class="sxs-lookup"><span data-stu-id="0775a-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="0775a-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0775a-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0775a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0775a-131">Int32</span></span>|<span data-ttu-id="0775a-132">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0775a-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="0775a-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0775a-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0775a-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0775a-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0775a-135">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0775a-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0775a-136">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0775a-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0775a-137">Relações</span><span class="sxs-lookup"><span data-stu-id="0775a-137">Relationships</span></span>
<span data-ttu-id="0775a-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0775a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0775a-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0775a-139">JSON Representation</span></span>
<span data-ttu-id="0775a-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0775a-140">Here is a JSON representation of the resource.</span></span>
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





