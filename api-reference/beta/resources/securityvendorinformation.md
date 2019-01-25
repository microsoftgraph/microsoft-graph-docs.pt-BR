---
title: tipo de recurso de securityVendorInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512175"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="8ded3-104">tipo de recurso de securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="8ded3-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ded3-105">Contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="8ded3-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="8ded3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ded3-106">Properties</span></span>

| <span data-ttu-id="8ded3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ded3-107">Property</span></span>   | <span data-ttu-id="8ded3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ded3-108">Type</span></span>|<span data-ttu-id="8ded3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ded3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ded3-110">Provider=</span><span class="sxs-lookup"><span data-stu-id="8ded3-110">provider</span></span> |<span data-ttu-id="8ded3-111">String</span><span class="sxs-lookup"><span data-stu-id="8ded3-111">String</span></span>|<span data-ttu-id="8ded3-112">Provedor específico (produto ou serviço - não a empresa de fornecedor); Por exemplo, WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="8ded3-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="8ded3-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="8ded3-113">providerVersion</span></span>|<span data-ttu-id="8ded3-114">String</span><span class="sxs-lookup"><span data-stu-id="8ded3-114">String</span></span>|<span data-ttu-id="8ded3-115">Versão do provedor ou subprovider, se ela existir, que gerou o alerta.</span><span class="sxs-lookup"><span data-stu-id="8ded3-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="8ded3-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="8ded3-116">*Required*</span></span>|
|<span data-ttu-id="8ded3-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="8ded3-117">subProvider</span></span>|<span data-ttu-id="8ded3-118">String</span><span class="sxs-lookup"><span data-stu-id="8ded3-118">String</span></span>|<span data-ttu-id="8ded3-119">Subprovider específico (abaixo de agregação de provedor;) Por exemplo, WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="8ded3-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="8ded3-120">fornecedor</span><span class="sxs-lookup"><span data-stu-id="8ded3-120">vendor</span></span> |<span data-ttu-id="8ded3-121">String</span><span class="sxs-lookup"><span data-stu-id="8ded3-121">String</span></span>|<span data-ttu-id="8ded3-122">Nome do alerta fornecedor (por exemplo, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="8ded3-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="8ded3-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="8ded3-123">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ded3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ded3-124">JSON representation</span></span>

<span data-ttu-id="8ded3-125">A seguinte é uma representação de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ded3-125">The folllowing is a JSON representation of the resource.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
