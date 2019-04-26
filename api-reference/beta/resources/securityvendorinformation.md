---
title: tipo de recurso securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7f48c27ba94d8419ce244143a48cf6ab04dd080e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583233"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="01ce5-104">tipo de recurso securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="01ce5-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01ce5-105">Contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subfornecedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subFornecedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="01ce5-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="01ce5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01ce5-106">Properties</span></span>

| <span data-ttu-id="01ce5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01ce5-107">Property</span></span>   | <span data-ttu-id="01ce5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="01ce5-108">Type</span></span>|<span data-ttu-id="01ce5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="01ce5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01ce5-110">provedor</span><span class="sxs-lookup"><span data-stu-id="01ce5-110">provider</span></span> |<span data-ttu-id="01ce5-111">String</span><span class="sxs-lookup"><span data-stu-id="01ce5-111">String</span></span>|<span data-ttu-id="01ce5-112">Provedor específico (produto/serviço – empresa de fornecedor); por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="01ce5-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="01ce5-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="01ce5-113">providerVersion</span></span>|<span data-ttu-id="01ce5-114">String</span><span class="sxs-lookup"><span data-stu-id="01ce5-114">String</span></span>|<span data-ttu-id="01ce5-115">Versão do provedor ou do subfornecedor, se existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="01ce5-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="01ce5-116">**Required**</span><span class="sxs-lookup"><span data-stu-id="01ce5-116">**Required**</span></span>|
|<span data-ttu-id="01ce5-117">subprovedor</span><span class="sxs-lookup"><span data-stu-id="01ce5-117">subProvider</span></span>|<span data-ttu-id="01ce5-118">String</span><span class="sxs-lookup"><span data-stu-id="01ce5-118">String</span></span>|<span data-ttu-id="01ce5-119">Subfornecedor específico (em provedor de agregação); por exemplo, WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="01ce5-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="01ce5-120">fornecedor</span><span class="sxs-lookup"><span data-stu-id="01ce5-120">vendor</span></span> |<span data-ttu-id="01ce5-121">String</span><span class="sxs-lookup"><span data-stu-id="01ce5-121">String</span></span>|<span data-ttu-id="01ce5-122">Nome do fornecedor do alerta (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="01ce5-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="01ce5-123">**Required**</span><span class="sxs-lookup"><span data-stu-id="01ce5-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01ce5-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01ce5-124">JSON representation</span></span>

<span data-ttu-id="01ce5-125">O folllowing é uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01ce5-125">The folllowing is a JSON representation of the resource.</span></span>
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
