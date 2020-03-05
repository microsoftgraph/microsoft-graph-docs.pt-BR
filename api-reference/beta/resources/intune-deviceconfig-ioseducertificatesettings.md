---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 503d2b1d0f4fa94e95d20882b10a0c30d968680e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529931"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="7079c-103">tipo de recurso iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="7079c-103">iosEduCertificateSettings resource type</span></span>

<span data-ttu-id="7079c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7079c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7079c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7079c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7079c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7079c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7079c-107">Certificados de raiz confiável e PFX para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="7079c-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="7079c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7079c-108">Properties</span></span>
|<span data-ttu-id="7079c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7079c-109">Property</span></span>|<span data-ttu-id="7079c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7079c-110">Type</span></span>|<span data-ttu-id="7079c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7079c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7079c-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="7079c-112">trustedRootCertificate</span></span>|<span data-ttu-id="7079c-113">Binária</span><span class="sxs-lookup"><span data-stu-id="7079c-113">Binary</span></span>|<span data-ttu-id="7079c-114">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="7079c-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="7079c-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="7079c-115">certFileName</span></span>|<span data-ttu-id="7079c-116">String</span><span class="sxs-lookup"><span data-stu-id="7079c-116">String</span></span>|<span data-ttu-id="7079c-117">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7079c-117">File name to display in UI.</span></span>|
|<span data-ttu-id="7079c-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="7079c-118">certificationAuthority</span></span>|<span data-ttu-id="7079c-119">String</span><span class="sxs-lookup"><span data-stu-id="7079c-119">String</span></span>|<span data-ttu-id="7079c-120">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="7079c-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="7079c-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="7079c-121">certificationAuthorityName</span></span>|<span data-ttu-id="7079c-122">String</span><span class="sxs-lookup"><span data-stu-id="7079c-122">String</span></span>|<span data-ttu-id="7079c-123">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="7079c-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="7079c-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="7079c-124">certificateTemplateName</span></span>|<span data-ttu-id="7079c-125">String</span><span class="sxs-lookup"><span data-stu-id="7079c-125">String</span></span>|<span data-ttu-id="7079c-126">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="7079c-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="7079c-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="7079c-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="7079c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7079c-128">Int32</span></span>|<span data-ttu-id="7079c-129">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="7079c-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7079c-130">Valores válidos de 1 a 99</span><span class="sxs-lookup"><span data-stu-id="7079c-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="7079c-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7079c-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7079c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7079c-132">Int32</span></span>|<span data-ttu-id="7079c-133">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="7079c-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="7079c-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7079c-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7079c-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7079c-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7079c-136">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="7079c-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7079c-137">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7079c-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7079c-138">Relações</span><span class="sxs-lookup"><span data-stu-id="7079c-138">Relationships</span></span>
<span data-ttu-id="7079c-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7079c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7079c-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7079c-140">JSON Representation</span></span>
<span data-ttu-id="7079c-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7079c-141">Here is a JSON representation of the resource.</span></span>
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



