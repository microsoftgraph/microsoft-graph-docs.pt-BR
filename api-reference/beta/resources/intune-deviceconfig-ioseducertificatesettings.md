---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d9060c28744bae52d4690bf75487e298d58d2a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571713"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="d2468-103">tipo de recurso iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="d2468-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="d2468-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2468-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2468-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2468-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2468-106">Certificados de raiz confiável e PFX para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="d2468-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="d2468-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2468-107">Properties</span></span>
|<span data-ttu-id="d2468-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2468-108">Property</span></span>|<span data-ttu-id="d2468-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2468-109">Type</span></span>|<span data-ttu-id="d2468-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2468-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2468-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d2468-111">trustedRootCertificate</span></span>|<span data-ttu-id="d2468-112">Binário</span><span class="sxs-lookup"><span data-stu-id="d2468-112">Binary</span></span>|<span data-ttu-id="d2468-113">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="d2468-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="d2468-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="d2468-114">certFileName</span></span>|<span data-ttu-id="d2468-115">String</span><span class="sxs-lookup"><span data-stu-id="d2468-115">String</span></span>|<span data-ttu-id="d2468-116">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2468-116">File name to display in UI.</span></span>|
|<span data-ttu-id="d2468-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="d2468-117">certificationAuthority</span></span>|<span data-ttu-id="d2468-118">String</span><span class="sxs-lookup"><span data-stu-id="d2468-118">String</span></span>|<span data-ttu-id="d2468-119">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="d2468-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="d2468-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="d2468-120">certificationAuthorityName</span></span>|<span data-ttu-id="d2468-121">String</span><span class="sxs-lookup"><span data-stu-id="d2468-121">String</span></span>|<span data-ttu-id="d2468-122">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="d2468-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="d2468-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="d2468-123">certificateTemplateName</span></span>|<span data-ttu-id="d2468-124">String</span><span class="sxs-lookup"><span data-stu-id="d2468-124">String</span></span>|<span data-ttu-id="d2468-125">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="d2468-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="d2468-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d2468-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="d2468-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d2468-127">Int32</span></span>|<span data-ttu-id="d2468-128">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="d2468-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d2468-129">Valores válidos de 1 a 99</span><span class="sxs-lookup"><span data-stu-id="d2468-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="d2468-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d2468-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d2468-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d2468-131">Int32</span></span>|<span data-ttu-id="d2468-132">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d2468-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="d2468-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d2468-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d2468-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d2468-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d2468-135">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d2468-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d2468-136">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d2468-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2468-137">Relações</span><span class="sxs-lookup"><span data-stu-id="d2468-137">Relationships</span></span>
<span data-ttu-id="d2468-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2468-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2468-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2468-139">JSON Representation</span></span>
<span data-ttu-id="d2468-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2468-140">Here is a JSON representation of the resource.</span></span>
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





