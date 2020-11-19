---
title: tipo de recurso iosEduCertificateSettings
description: Certificados de raiz confiável e PFX para iOS EDU.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a4f62587c2a569896d69a4273d80eb5a92942b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273603"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="14b23-103">tipo de recurso iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="14b23-103">iosEduCertificateSettings resource type</span></span>

<span data-ttu-id="14b23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14b23-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14b23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14b23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14b23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14b23-107">Certificados de raiz confiável e PFX para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="14b23-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="14b23-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14b23-108">Properties</span></span>
|<span data-ttu-id="14b23-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14b23-109">Property</span></span>|<span data-ttu-id="14b23-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="14b23-110">Type</span></span>|<span data-ttu-id="14b23-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="14b23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b23-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="14b23-112">trustedRootCertificate</span></span>|<span data-ttu-id="14b23-113">Binária</span><span class="sxs-lookup"><span data-stu-id="14b23-113">Binary</span></span>|<span data-ttu-id="14b23-114">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="14b23-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="14b23-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="14b23-115">certFileName</span></span>|<span data-ttu-id="14b23-116">String</span><span class="sxs-lookup"><span data-stu-id="14b23-116">String</span></span>|<span data-ttu-id="14b23-117">Nome do arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="14b23-117">File name to display in UI.</span></span>|
|<span data-ttu-id="14b23-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="14b23-118">certificationAuthority</span></span>|<span data-ttu-id="14b23-119">String</span><span class="sxs-lookup"><span data-stu-id="14b23-119">String</span></span>|<span data-ttu-id="14b23-120">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="14b23-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="14b23-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="14b23-121">certificationAuthorityName</span></span>|<span data-ttu-id="14b23-122">String</span><span class="sxs-lookup"><span data-stu-id="14b23-122">String</span></span>|<span data-ttu-id="14b23-123">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="14b23-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="14b23-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="14b23-124">certificateTemplateName</span></span>|<span data-ttu-id="14b23-125">String</span><span class="sxs-lookup"><span data-stu-id="14b23-125">String</span></span>|<span data-ttu-id="14b23-126">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="14b23-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="14b23-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="14b23-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="14b23-128">Int32</span><span class="sxs-lookup"><span data-stu-id="14b23-128">Int32</span></span>|<span data-ttu-id="14b23-129">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="14b23-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="14b23-130">Valores válidos de 1 a 99</span><span class="sxs-lookup"><span data-stu-id="14b23-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="14b23-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="14b23-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="14b23-132">Int32</span><span class="sxs-lookup"><span data-stu-id="14b23-132">Int32</span></span>|<span data-ttu-id="14b23-133">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="14b23-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="14b23-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="14b23-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="14b23-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="14b23-135">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="14b23-136">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="14b23-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="14b23-137">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="14b23-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14b23-138">Relações</span><span class="sxs-lookup"><span data-stu-id="14b23-138">Relationships</span></span>
<span data-ttu-id="14b23-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14b23-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14b23-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14b23-140">JSON Representation</span></span>
<span data-ttu-id="14b23-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14b23-141">Here is a JSON representation of the resource.</span></span>
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




