---
title: tipo de recurso securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: f0c0142333237c1c4700353b01f75b9867b85ad7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988825"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="33821-104">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="33821-104">securityVendorInformation resource type</span></span>

<span data-ttu-id="33821-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33821-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33821-106">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="33821-106">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="33821-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33821-107">Properties</span></span>

| <span data-ttu-id="33821-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33821-108">Property</span></span>   | <span data-ttu-id="33821-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="33821-109">Type</span></span>|<span data-ttu-id="33821-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33821-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33821-111">provedor</span><span class="sxs-lookup"><span data-stu-id="33821-111">provider</span></span> |<span data-ttu-id="33821-112">String</span><span class="sxs-lookup"><span data-stu-id="33821-112">String</span></span>|<span data-ttu-id="33821-113">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="33821-113">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="33821-114">providerVersion</span><span class="sxs-lookup"><span data-stu-id="33821-114">providerVersion</span></span>|<span data-ttu-id="33821-115">String</span><span class="sxs-lookup"><span data-stu-id="33821-115">String</span></span>|<span data-ttu-id="33821-116">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="33821-116">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="33821-117">**Required**</span><span class="sxs-lookup"><span data-stu-id="33821-117">**Required**</span></span>|
|<span data-ttu-id="33821-118">subprovedor</span><span class="sxs-lookup"><span data-stu-id="33821-118">subProvider</span></span>|<span data-ttu-id="33821-119">String</span><span class="sxs-lookup"><span data-stu-id="33821-119">String</span></span>|<span data-ttu-id="33821-120">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="33821-120">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="33821-121">fornecedor</span><span class="sxs-lookup"><span data-stu-id="33821-121">vendor</span></span> |<span data-ttu-id="33821-122">String</span><span class="sxs-lookup"><span data-stu-id="33821-122">String</span></span>|<span data-ttu-id="33821-123">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="33821-123">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="33821-124">**Required**</span><span class="sxs-lookup"><span data-stu-id="33821-124">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33821-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33821-125">JSON representation</span></span>

<span data-ttu-id="33821-126">O folllowing é uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33821-126">The folllowing is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


