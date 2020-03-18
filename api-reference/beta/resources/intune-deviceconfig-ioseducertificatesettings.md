---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f772ee8f484b2b8bc42a6ed48298dc5a17016afc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791615"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="5d993-103">tipo de recurso iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="5d993-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="5d993-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d993-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d993-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d993-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d993-106">Certificados de raiz confiável e PFX para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="5d993-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="5d993-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d993-107">Properties</span></span>
|<span data-ttu-id="5d993-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d993-108">Property</span></span>|<span data-ttu-id="5d993-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d993-109">Type</span></span>|<span data-ttu-id="5d993-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d993-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d993-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5d993-111">trustedRootCertificate</span></span>|<span data-ttu-id="5d993-112">Binária</span><span class="sxs-lookup"><span data-stu-id="5d993-112">Binary</span></span>|<span data-ttu-id="5d993-113">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="5d993-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="5d993-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="5d993-114">certFileName</span></span>|<span data-ttu-id="5d993-115">String</span><span class="sxs-lookup"><span data-stu-id="5d993-115">String</span></span>|<span data-ttu-id="5d993-116">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d993-116">File name to display in UI.</span></span>|
|<span data-ttu-id="5d993-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="5d993-117">certificationAuthority</span></span>|<span data-ttu-id="5d993-118">String</span><span class="sxs-lookup"><span data-stu-id="5d993-118">String</span></span>|<span data-ttu-id="5d993-119">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="5d993-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="5d993-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="5d993-120">certificationAuthorityName</span></span>|<span data-ttu-id="5d993-121">String</span><span class="sxs-lookup"><span data-stu-id="5d993-121">String</span></span>|<span data-ttu-id="5d993-122">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="5d993-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="5d993-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="5d993-123">certificateTemplateName</span></span>|<span data-ttu-id="5d993-124">String</span><span class="sxs-lookup"><span data-stu-id="5d993-124">String</span></span>|<span data-ttu-id="5d993-125">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="5d993-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="5d993-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5d993-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="5d993-127">Int32</span><span class="sxs-lookup"><span data-stu-id="5d993-127">Int32</span></span>|<span data-ttu-id="5d993-128">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="5d993-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5d993-129">Valores válidos de 1 a 99</span><span class="sxs-lookup"><span data-stu-id="5d993-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="5d993-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5d993-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5d993-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5d993-131">Int32</span></span>|<span data-ttu-id="5d993-132">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5d993-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="5d993-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5d993-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5d993-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5d993-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5d993-135">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5d993-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5d993-136">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5d993-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d993-137">Relações</span><span class="sxs-lookup"><span data-stu-id="5d993-137">Relationships</span></span>
<span data-ttu-id="5d993-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d993-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d993-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d993-139">JSON Representation</span></span>
<span data-ttu-id="5d993-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d993-140">Here is a JSON representation of the resource.</span></span>
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



