---
title: tipo de recurso vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f421da54543d74009cb921ec429e3795e31d8572
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375391"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="12132-103">tipo de recurso vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="12132-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="12132-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12132-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12132-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12132-106">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="12132-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="12132-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12132-107">Properties</span></span>
|<span data-ttu-id="12132-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12132-108">Property</span></span>|<span data-ttu-id="12132-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12132-109">Type</span></span>|<span data-ttu-id="12132-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12132-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12132-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="12132-111">vppTokenId</span></span>|<span data-ttu-id="12132-112">String</span><span class="sxs-lookup"><span data-stu-id="12132-112">String</span></span>|<span data-ttu-id="12132-113">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="12132-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="12132-114">appleId</span><span class="sxs-lookup"><span data-stu-id="12132-114">appleId</span></span>|<span data-ttu-id="12132-115">String</span><span class="sxs-lookup"><span data-stu-id="12132-115">String</span></span>|<span data-ttu-id="12132-116">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="12132-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="12132-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="12132-117">organizationName</span></span>|<span data-ttu-id="12132-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12132-118">String</span></span>|<span data-ttu-id="12132-119">A organização associada ao token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="12132-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="12132-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="12132-120">availableLicenseCount</span></span>|<span data-ttu-id="12132-121">Int32</span><span class="sxs-lookup"><span data-stu-id="12132-121">Int32</span></span>|<span data-ttu-id="12132-122">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="12132-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="12132-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="12132-123">usedLicenseCount</span></span>|<span data-ttu-id="12132-124">Int32</span><span class="sxs-lookup"><span data-stu-id="12132-124">Int32</span></span>|<span data-ttu-id="12132-125">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="12132-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12132-126">Relações</span><span class="sxs-lookup"><span data-stu-id="12132-126">Relationships</span></span>
<span data-ttu-id="12132-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12132-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12132-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12132-128">JSON Representation</span></span>
<span data-ttu-id="12132-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12132-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```



