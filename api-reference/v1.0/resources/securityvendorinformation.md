---
title: tipo de recurso de securityVendorInformation
description: " subProvider = AppLocker)."
localization_priority: Normal
ms.openlocfilehash: e9d8551c085c05007388bf0c6e33143994c6969b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820143"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="42091-103">tipo de recurso de securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="42091-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="42091-104">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="42091-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="42091-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42091-105">Properties</span></span>

| <span data-ttu-id="42091-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42091-106">Property</span></span>   | <span data-ttu-id="42091-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="42091-107">Type</span></span>|<span data-ttu-id="42091-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="42091-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42091-109">provedor</span><span class="sxs-lookup"><span data-stu-id="42091-109">provider</span></span> |<span data-ttu-id="42091-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42091-110">String</span></span>|<span data-ttu-id="42091-111">Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="42091-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="42091-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="42091-112">providerVersion</span></span>|<span data-ttu-id="42091-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42091-113">String</span></span>|<span data-ttu-id="42091-114">Versão do provedor ou subprovider, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="42091-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="42091-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="42091-115">*Required*</span></span>|
|<span data-ttu-id="42091-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="42091-116">subProvider</span></span>|<span data-ttu-id="42091-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42091-117">String</span></span>|<span data-ttu-id="42091-118">Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="42091-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="42091-119">fornecedor</span><span class="sxs-lookup"><span data-stu-id="42091-119">vendor</span></span> |<span data-ttu-id="42091-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42091-120">String</span></span>|<span data-ttu-id="42091-121">Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="42091-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="42091-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="42091-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="42091-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42091-123">JSON representation</span></span>

<span data-ttu-id="42091-124">A seguinte é uma representação de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42091-124">The folllowing is a JSON representation of the resource.</span></span>
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
