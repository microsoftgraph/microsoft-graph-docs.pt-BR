---
title: tipo de recurso securityVendorInformation
description: " subfornecedor = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 536ed37cfe8ba190a22ef86e190af2b171d352ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983981"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="0a574-103">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="0a574-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="0a574-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a574-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a574-105">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="0a574-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="0a574-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a574-106">Properties</span></span>

| <span data-ttu-id="0a574-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a574-107">Property</span></span>   | <span data-ttu-id="0a574-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a574-108">Type</span></span>|<span data-ttu-id="0a574-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a574-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a574-110">provedor</span><span class="sxs-lookup"><span data-stu-id="0a574-110">provider</span></span> |<span data-ttu-id="0a574-111">String</span><span class="sxs-lookup"><span data-stu-id="0a574-111">String</span></span>|<span data-ttu-id="0a574-112">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="0a574-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="0a574-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="0a574-113">providerVersion</span></span>|<span data-ttu-id="0a574-114">String</span><span class="sxs-lookup"><span data-stu-id="0a574-114">String</span></span>|<span data-ttu-id="0a574-115">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="0a574-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="0a574-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="0a574-116">*Required*</span></span>|
|<span data-ttu-id="0a574-117">subprovedor</span><span class="sxs-lookup"><span data-stu-id="0a574-117">subProvider</span></span>|<span data-ttu-id="0a574-118">String</span><span class="sxs-lookup"><span data-stu-id="0a574-118">String</span></span>|<span data-ttu-id="0a574-119">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="0a574-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="0a574-120">fornecedor</span><span class="sxs-lookup"><span data-stu-id="0a574-120">vendor</span></span> |<span data-ttu-id="0a574-121">String</span><span class="sxs-lookup"><span data-stu-id="0a574-121">String</span></span>|<span data-ttu-id="0a574-122">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="0a574-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="0a574-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="0a574-123">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0a574-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a574-124">JSON representation</span></span>

<span data-ttu-id="0a574-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a574-125">The following is a JSON representation of the resource.</span></span>
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

