---
title: tipo de recurso de securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 0137abd7a9df0df94f73e18d7efa201008031ff6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939921"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="18bff-104">tipo de recurso de securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="18bff-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="18bff-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18bff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18bff-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18bff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18bff-107">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="18bff-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="18bff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18bff-108">Properties</span></span>

| <span data-ttu-id="18bff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18bff-109">Property</span></span>   | <span data-ttu-id="18bff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18bff-110">Type</span></span>|<span data-ttu-id="18bff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18bff-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18bff-112">provedor</span><span class="sxs-lookup"><span data-stu-id="18bff-112">provider</span></span> |<span data-ttu-id="18bff-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bff-113">String</span></span>|<span data-ttu-id="18bff-114">Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="18bff-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="18bff-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="18bff-115">providerVersion</span></span>|<span data-ttu-id="18bff-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bff-116">String</span></span>|<span data-ttu-id="18bff-117">Versão do provedor ou subprovider, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="18bff-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="18bff-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="18bff-118">*Required*</span></span>|
|<span data-ttu-id="18bff-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="18bff-119">subProvider</span></span>|<span data-ttu-id="18bff-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bff-120">String</span></span>|<span data-ttu-id="18bff-121">Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="18bff-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="18bff-122">fornecedor</span><span class="sxs-lookup"><span data-stu-id="18bff-122">vendor</span></span> |<span data-ttu-id="18bff-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18bff-123">String</span></span>|<span data-ttu-id="18bff-124">Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="18bff-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="18bff-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="18bff-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18bff-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18bff-126">JSON representation</span></span>

<span data-ttu-id="18bff-127">A seguinte é uma representação de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18bff-127">The folllowing is a JSON representation of the resource.</span></span>
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
