---
title: tipo de recurso de iosEduCertificateSettings
description: Certificados raiz e PFX confiáveis para iOS EDU.
ms.openlocfilehash: 348b8231ed87c46180c54eb5ebfe24d671c9015b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034927"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="ebbcf-103">tipo de recurso de iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="ebbcf-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="ebbcf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebbcf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebbcf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebbcf-107">Certificados raiz e PFX confiáveis para iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="ebbcf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebbcf-108">Properties</span></span>
|<span data-ttu-id="ebbcf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebbcf-109">Property</span></span>|<span data-ttu-id="ebbcf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebbcf-110">Type</span></span>|<span data-ttu-id="ebbcf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebbcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbcf-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ebbcf-112">trustedRootCertificate</span></span>|<span data-ttu-id="ebbcf-113">Binário</span><span class="sxs-lookup"><span data-stu-id="ebbcf-113">Binary</span></span>|<span data-ttu-id="ebbcf-114">Certificado raiz confiável.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="ebbcf-115">Nome_arquivo_cert</span><span class="sxs-lookup"><span data-stu-id="ebbcf-115">certFileName</span></span>|<span data-ttu-id="ebbcf-116">String</span><span class="sxs-lookup"><span data-stu-id="ebbcf-116">String</span></span>|<span data-ttu-id="ebbcf-117">Nome de arquivo a ser exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-117">File name to display in UI.</span></span>|
|<span data-ttu-id="ebbcf-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="ebbcf-118">certificationAuthority</span></span>|<span data-ttu-id="ebbcf-119">String</span><span class="sxs-lookup"><span data-stu-id="ebbcf-119">String</span></span>|<span data-ttu-id="ebbcf-120">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="ebbcf-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="ebbcf-121">certificationAuthorityName</span></span>|<span data-ttu-id="ebbcf-122">String</span><span class="sxs-lookup"><span data-stu-id="ebbcf-122">String</span></span>|<span data-ttu-id="ebbcf-123">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="ebbcf-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="ebbcf-124">certificateTemplateName</span></span>|<span data-ttu-id="ebbcf-125">String</span><span class="sxs-lookup"><span data-stu-id="ebbcf-125">String</span></span>|<span data-ttu-id="ebbcf-126">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="ebbcf-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ebbcf-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="ebbcf-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ebbcf-128">Int32</span></span>|<span data-ttu-id="ebbcf-129">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ebbcf-130">Valores válidos 1 a 99</span><span class="sxs-lookup"><span data-stu-id="ebbcf-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="ebbcf-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ebbcf-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ebbcf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ebbcf-132">Int32</span></span>|<span data-ttu-id="ebbcf-133">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="ebbcf-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ebbcf-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ebbcf-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ebbcf-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ebbcf-136">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ebbcf-137">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebbcf-138">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ebbcf-138">Relationships</span></span>
<span data-ttu-id="ebbcf-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebbcf-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebbcf-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebbcf-140">JSON Representation</span></span>
<span data-ttu-id="ebbcf-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebbcf-141">Here is a JSON representation of the resource.</span></span>
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





