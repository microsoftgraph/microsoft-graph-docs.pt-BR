---
title: tipo de recurso securityVendorInformation
description: " subfornecedor = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7af6e0903e3d178bacdd7c86b4a2cab04285171
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536094"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="bb5ac-103">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="bb5ac-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="bb5ac-104">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="bb5ac-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="bb5ac-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb5ac-105">Properties</span></span>

| <span data-ttu-id="bb5ac-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb5ac-106">Property</span></span>   | <span data-ttu-id="bb5ac-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb5ac-107">Type</span></span>|<span data-ttu-id="bb5ac-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb5ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb5ac-109">provedor</span><span class="sxs-lookup"><span data-stu-id="bb5ac-109">provider</span></span> |<span data-ttu-id="bb5ac-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-110">String</span></span>|<span data-ttu-id="bb5ac-111">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="bb5ac-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="bb5ac-112">providerVersion</span></span>|<span data-ttu-id="bb5ac-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-113">String</span></span>|<span data-ttu-id="bb5ac-114">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="bb5ac-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="bb5ac-115">*Required*</span></span>|
|<span data-ttu-id="bb5ac-116">subprovedor</span><span class="sxs-lookup"><span data-stu-id="bb5ac-116">subProvider</span></span>|<span data-ttu-id="bb5ac-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-117">String</span></span>|<span data-ttu-id="bb5ac-118">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="bb5ac-119">fornecedor</span><span class="sxs-lookup"><span data-stu-id="bb5ac-119">vendor</span></span> |<span data-ttu-id="bb5ac-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-120">String</span></span>|<span data-ttu-id="bb5ac-121">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="bb5ac-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="bb5ac-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="bb5ac-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bb5ac-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb5ac-123">JSON representation</span></span>

<span data-ttu-id="bb5ac-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-124">The following is a JSON representation of the resource.</span></span>
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
