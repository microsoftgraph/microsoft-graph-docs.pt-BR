---
title: tipo de recurso securityVendorInformation
description: " subfornecedor = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bb2b67892f5c1bffbc9844a7d30b9b16ea9cdf6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533755"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="f924d-103">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f924d-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="f924d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f924d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f924d-105">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="f924d-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="f924d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f924d-106">Properties</span></span>

| <span data-ttu-id="f924d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f924d-107">Property</span></span>   | <span data-ttu-id="f924d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f924d-108">Type</span></span>|<span data-ttu-id="f924d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f924d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f924d-110">provedor</span><span class="sxs-lookup"><span data-stu-id="f924d-110">provider</span></span> |<span data-ttu-id="f924d-111">String</span><span class="sxs-lookup"><span data-stu-id="f924d-111">String</span></span>|<span data-ttu-id="f924d-112">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="f924d-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="f924d-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="f924d-113">providerVersion</span></span>|<span data-ttu-id="f924d-114">String</span><span class="sxs-lookup"><span data-stu-id="f924d-114">String</span></span>|<span data-ttu-id="f924d-115">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="f924d-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="f924d-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="f924d-116">*Required*</span></span>|
|<span data-ttu-id="f924d-117">subprovedor</span><span class="sxs-lookup"><span data-stu-id="f924d-117">subProvider</span></span>|<span data-ttu-id="f924d-118">String</span><span class="sxs-lookup"><span data-stu-id="f924d-118">String</span></span>|<span data-ttu-id="f924d-119">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="f924d-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="f924d-120">fornecedor</span><span class="sxs-lookup"><span data-stu-id="f924d-120">vendor</span></span> |<span data-ttu-id="f924d-121">String</span><span class="sxs-lookup"><span data-stu-id="f924d-121">String</span></span>|<span data-ttu-id="f924d-122">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="f924d-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="f924d-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="f924d-123">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f924d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f924d-124">JSON representation</span></span>

<span data-ttu-id="f924d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f924d-125">The following is a JSON representation of the resource.</span></span>
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
