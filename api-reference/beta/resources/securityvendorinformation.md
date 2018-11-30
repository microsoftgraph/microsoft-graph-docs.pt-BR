---
title: tipo de recurso de securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 4016e274a82ad6a28101dbf5b053124b439a3cbf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038898"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="21fd4-104">tipo de recurso de securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="21fd4-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="21fd4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21fd4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21fd4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21fd4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21fd4-107">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="21fd4-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="21fd4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21fd4-108">Properties</span></span>

| <span data-ttu-id="21fd4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21fd4-109">Property</span></span>   | <span data-ttu-id="21fd4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="21fd4-110">Type</span></span>|<span data-ttu-id="21fd4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="21fd4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21fd4-112">provedor</span><span class="sxs-lookup"><span data-stu-id="21fd4-112">provider</span></span> |<span data-ttu-id="21fd4-113">String</span><span class="sxs-lookup"><span data-stu-id="21fd4-113">String</span></span>|<span data-ttu-id="21fd4-114">Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="21fd4-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="21fd4-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="21fd4-115">providerVersion</span></span>|<span data-ttu-id="21fd4-116">String</span><span class="sxs-lookup"><span data-stu-id="21fd4-116">String</span></span>|<span data-ttu-id="21fd4-117">Versão do provedor ou subprovider, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="21fd4-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="21fd4-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="21fd4-118">*Required*</span></span>|
|<span data-ttu-id="21fd4-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="21fd4-119">subProvider</span></span>|<span data-ttu-id="21fd4-120">String</span><span class="sxs-lookup"><span data-stu-id="21fd4-120">String</span></span>|<span data-ttu-id="21fd4-121">Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="21fd4-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="21fd4-122">fornecedor</span><span class="sxs-lookup"><span data-stu-id="21fd4-122">vendor</span></span> |<span data-ttu-id="21fd4-123">String</span><span class="sxs-lookup"><span data-stu-id="21fd4-123">String</span></span>|<span data-ttu-id="21fd4-124">Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="21fd4-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="21fd4-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="21fd4-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21fd4-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21fd4-126">JSON representation</span></span>

<span data-ttu-id="21fd4-127">A seguinte é uma representação de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21fd4-127">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
