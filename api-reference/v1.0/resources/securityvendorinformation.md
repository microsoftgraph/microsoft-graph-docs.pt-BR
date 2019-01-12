---
title: tipo de recurso de securityVendorInformation
description: " subProvider = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945934"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="f5ae6-103">tipo de recurso de securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f5ae6-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="f5ae6-104">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="f5ae6-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="f5ae6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5ae6-105">Properties</span></span>

| <span data-ttu-id="f5ae6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5ae6-106">Property</span></span>   | <span data-ttu-id="f5ae6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5ae6-107">Type</span></span>|<span data-ttu-id="f5ae6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ae6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5ae6-109">provedor</span><span class="sxs-lookup"><span data-stu-id="f5ae6-109">provider</span></span> |<span data-ttu-id="f5ae6-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5ae6-110">String</span></span>|<span data-ttu-id="f5ae6-111">Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="f5ae6-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="f5ae6-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="f5ae6-112">providerVersion</span></span>|<span data-ttu-id="f5ae6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5ae6-113">String</span></span>|<span data-ttu-id="f5ae6-114">Versão do provedor ou subprovider, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="f5ae6-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="f5ae6-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="f5ae6-115">*Required*</span></span>|
|<span data-ttu-id="f5ae6-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="f5ae6-116">subProvider</span></span>|<span data-ttu-id="f5ae6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5ae6-117">String</span></span>|<span data-ttu-id="f5ae6-118">Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="f5ae6-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="f5ae6-119">fornecedor</span><span class="sxs-lookup"><span data-stu-id="f5ae6-119">vendor</span></span> |<span data-ttu-id="f5ae6-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5ae6-120">String</span></span>|<span data-ttu-id="f5ae6-121">Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="f5ae6-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="f5ae6-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="f5ae6-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f5ae6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5ae6-123">JSON representation</span></span>

<span data-ttu-id="f5ae6-124">A seguinte é uma representação de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5ae6-124">The folllowing is a JSON representation of the resource.</span></span>
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
