---
title: tipo de recurso securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d543bf16617ed28d50d2e7082372ff2014cd24c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343290"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="c9a8c-104">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="c9a8c-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9a8c-105">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subFornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="c9a8c-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="c9a8c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9a8c-106">Properties</span></span>

| <span data-ttu-id="c9a8c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9a8c-107">Property</span></span>   | <span data-ttu-id="c9a8c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9a8c-108">Type</span></span>|<span data-ttu-id="c9a8c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9a8c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9a8c-110">provedor</span><span class="sxs-lookup"><span data-stu-id="c9a8c-110">provider</span></span> |<span data-ttu-id="c9a8c-111">String</span><span class="sxs-lookup"><span data-stu-id="c9a8c-111">String</span></span>|<span data-ttu-id="c9a8c-112">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="c9a8c-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="c9a8c-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="c9a8c-113">providerVersion</span></span>|<span data-ttu-id="c9a8c-114">String</span><span class="sxs-lookup"><span data-stu-id="c9a8c-114">String</span></span>|<span data-ttu-id="c9a8c-115">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="c9a8c-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="c9a8c-116">**Required**</span><span class="sxs-lookup"><span data-stu-id="c9a8c-116">**Required**</span></span>|
|<span data-ttu-id="c9a8c-117">subprovedor</span><span class="sxs-lookup"><span data-stu-id="c9a8c-117">subProvider</span></span>|<span data-ttu-id="c9a8c-118">String</span><span class="sxs-lookup"><span data-stu-id="c9a8c-118">String</span></span>|<span data-ttu-id="c9a8c-119">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="c9a8c-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="c9a8c-120">fornecedor</span><span class="sxs-lookup"><span data-stu-id="c9a8c-120">vendor</span></span> |<span data-ttu-id="c9a8c-121">String</span><span class="sxs-lookup"><span data-stu-id="c9a8c-121">String</span></span>|<span data-ttu-id="c9a8c-122">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="c9a8c-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="c9a8c-123">**Required**</span><span class="sxs-lookup"><span data-stu-id="c9a8c-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9a8c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9a8c-124">JSON representation</span></span>

<span data-ttu-id="c9a8c-125">O folllowing é uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9a8c-125">The folllowing is a JSON representation of the resource.</span></span>
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
