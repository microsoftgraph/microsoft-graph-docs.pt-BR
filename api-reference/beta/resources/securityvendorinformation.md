---
title: tipo de recurso securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 517213e3e2266681eee0f6bdca53b0b9ce5a0bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520805"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="59f6c-104">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="59f6c-104">securityVendorInformation resource type</span></span>

<span data-ttu-id="59f6c-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59f6c-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59f6c-106">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subfornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="59f6c-106">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="59f6c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59f6c-107">Properties</span></span>

| <span data-ttu-id="59f6c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59f6c-108">Property</span></span>   | <span data-ttu-id="59f6c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f6c-109">Type</span></span>|<span data-ttu-id="59f6c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59f6c-111">provedor</span><span class="sxs-lookup"><span data-stu-id="59f6c-111">provider</span></span> |<span data-ttu-id="59f6c-112">String</span><span class="sxs-lookup"><span data-stu-id="59f6c-112">String</span></span>|<span data-ttu-id="59f6c-113">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="59f6c-113">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="59f6c-114">providerVersion</span><span class="sxs-lookup"><span data-stu-id="59f6c-114">providerVersion</span></span>|<span data-ttu-id="59f6c-115">String</span><span class="sxs-lookup"><span data-stu-id="59f6c-115">String</span></span>|<span data-ttu-id="59f6c-116">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="59f6c-116">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="59f6c-117">**Required**</span><span class="sxs-lookup"><span data-stu-id="59f6c-117">**Required**</span></span>|
|<span data-ttu-id="59f6c-118">subprovedor</span><span class="sxs-lookup"><span data-stu-id="59f6c-118">subProvider</span></span>|<span data-ttu-id="59f6c-119">String</span><span class="sxs-lookup"><span data-stu-id="59f6c-119">String</span></span>|<span data-ttu-id="59f6c-120">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="59f6c-120">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="59f6c-121">fornecedor</span><span class="sxs-lookup"><span data-stu-id="59f6c-121">vendor</span></span> |<span data-ttu-id="59f6c-122">String</span><span class="sxs-lookup"><span data-stu-id="59f6c-122">String</span></span>|<span data-ttu-id="59f6c-123">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="59f6c-123">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="59f6c-124">**Required**</span><span class="sxs-lookup"><span data-stu-id="59f6c-124">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59f6c-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59f6c-125">JSON representation</span></span>

<span data-ttu-id="59f6c-126">O folllowing é uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59f6c-126">The folllowing is a JSON representation of the resource.</span></span>
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
