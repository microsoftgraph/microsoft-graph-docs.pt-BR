---
title: tipo de recurso securityVendorInformation
description: " subfornecedor = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3fb959da2d6af10632f9113a33eb942492b679ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034423"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="b2ed1-103">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="b2ed1-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="b2ed1-104">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="b2ed1-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="b2ed1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2ed1-105">Properties</span></span>

| <span data-ttu-id="b2ed1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2ed1-106">Property</span></span>   | <span data-ttu-id="b2ed1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2ed1-107">Type</span></span>|<span data-ttu-id="b2ed1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2ed1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2ed1-109">provedor</span><span class="sxs-lookup"><span data-stu-id="b2ed1-109">provider</span></span> |<span data-ttu-id="b2ed1-110">String</span><span class="sxs-lookup"><span data-stu-id="b2ed1-110">String</span></span>|<span data-ttu-id="b2ed1-111">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="b2ed1-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="b2ed1-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="b2ed1-112">providerVersion</span></span>|<span data-ttu-id="b2ed1-113">String</span><span class="sxs-lookup"><span data-stu-id="b2ed1-113">String</span></span>|<span data-ttu-id="b2ed1-114">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="b2ed1-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="b2ed1-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="b2ed1-115">*Required*</span></span>|
|<span data-ttu-id="b2ed1-116">subprovedor</span><span class="sxs-lookup"><span data-stu-id="b2ed1-116">subProvider</span></span>|<span data-ttu-id="b2ed1-117">String</span><span class="sxs-lookup"><span data-stu-id="b2ed1-117">String</span></span>|<span data-ttu-id="b2ed1-118">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="b2ed1-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="b2ed1-119">fornecedor</span><span class="sxs-lookup"><span data-stu-id="b2ed1-119">vendor</span></span> |<span data-ttu-id="b2ed1-120">String</span><span class="sxs-lookup"><span data-stu-id="b2ed1-120">String</span></span>|<span data-ttu-id="b2ed1-121">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="b2ed1-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="b2ed1-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="b2ed1-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b2ed1-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2ed1-123">JSON representation</span></span>

<span data-ttu-id="b2ed1-124">O folllowing é uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2ed1-124">The folllowing is a JSON representation of the resource.</span></span>
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
