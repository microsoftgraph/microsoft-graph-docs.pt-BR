---
title: tipo de recurso de iosEduCertificateSettings
description: Certificados raiz e PFX confiáveis para iOS EDU.
author: tfitzmac
ms.openlocfilehash: 8e373a7c878dd06870b13a32c428f837d741964c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332323"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="2e26c-103">tipo de recurso de iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="2e26c-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="2e26c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2e26c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e26c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2e26c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e26c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2e26c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e26c-107">Certificados raiz e PFX confiáveis para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="2e26c-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="2e26c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e26c-108">Properties</span></span>
|<span data-ttu-id="2e26c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e26c-109">Property</span></span>|<span data-ttu-id="2e26c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e26c-110">Type</span></span>|<span data-ttu-id="2e26c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e26c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e26c-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2e26c-112">trustedRootCertificate</span></span>|<span data-ttu-id="2e26c-113">Binária</span><span class="sxs-lookup"><span data-stu-id="2e26c-113">Binary</span></span>|<span data-ttu-id="2e26c-114">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="2e26c-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="2e26c-115">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="2e26c-115">certFileName</span></span>|<span data-ttu-id="2e26c-116">String</span><span class="sxs-lookup"><span data-stu-id="2e26c-116">String</span></span>|<span data-ttu-id="2e26c-117">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e26c-117">File name to display in UI.</span></span>|
|<span data-ttu-id="2e26c-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="2e26c-118">certificationAuthority</span></span>|<span data-ttu-id="2e26c-119">String</span><span class="sxs-lookup"><span data-stu-id="2e26c-119">String</span></span>|<span data-ttu-id="2e26c-120">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="2e26c-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="2e26c-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="2e26c-121">certificationAuthorityName</span></span>|<span data-ttu-id="2e26c-122">String</span><span class="sxs-lookup"><span data-stu-id="2e26c-122">String</span></span>|<span data-ttu-id="2e26c-123">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="2e26c-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="2e26c-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="2e26c-124">certificateTemplateName</span></span>|<span data-ttu-id="2e26c-125">String</span><span class="sxs-lookup"><span data-stu-id="2e26c-125">String</span></span>|<span data-ttu-id="2e26c-126">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="2e26c-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="2e26c-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="2e26c-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="2e26c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2e26c-128">Int32</span></span>|<span data-ttu-id="2e26c-129">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="2e26c-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="2e26c-130">Valores válidos 1 a 99</span><span class="sxs-lookup"><span data-stu-id="2e26c-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="2e26c-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="2e26c-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="2e26c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="2e26c-132">Int32</span></span>|<span data-ttu-id="2e26c-133">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="2e26c-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="2e26c-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2e26c-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="2e26c-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2e26c-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2e26c-136">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="2e26c-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="2e26c-137">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="2e26c-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e26c-138">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="2e26c-138">Relationships</span></span>
<span data-ttu-id="2e26c-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e26c-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e26c-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e26c-140">JSON Representation</span></span>
<span data-ttu-id="2e26c-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e26c-141">Here is a JSON representation of the resource.</span></span>
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





