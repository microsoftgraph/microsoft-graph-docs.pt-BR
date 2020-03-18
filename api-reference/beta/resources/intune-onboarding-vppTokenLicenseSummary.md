---
title: tipo de recurso vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20d7c24c887ca97f3a5a9890f5089b745130055e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777872"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="b8142-103">tipo de recurso vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="b8142-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="b8142-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8142-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8142-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8142-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8142-106">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="b8142-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="b8142-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8142-107">Properties</span></span>
|<span data-ttu-id="b8142-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8142-108">Property</span></span>|<span data-ttu-id="b8142-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8142-109">Type</span></span>|<span data-ttu-id="b8142-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8142-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8142-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b8142-111">vppTokenId</span></span>|<span data-ttu-id="b8142-112">String</span><span class="sxs-lookup"><span data-stu-id="b8142-112">String</span></span>|<span data-ttu-id="b8142-113">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="b8142-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="b8142-114">appleId</span><span class="sxs-lookup"><span data-stu-id="b8142-114">appleId</span></span>|<span data-ttu-id="b8142-115">String</span><span class="sxs-lookup"><span data-stu-id="b8142-115">String</span></span>|<span data-ttu-id="b8142-116">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="b8142-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b8142-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="b8142-117">organizationName</span></span>|<span data-ttu-id="b8142-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8142-118">String</span></span>|<span data-ttu-id="b8142-119">A organização associada ao token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b8142-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b8142-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b8142-120">availableLicenseCount</span></span>|<span data-ttu-id="b8142-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b8142-121">Int32</span></span>|<span data-ttu-id="b8142-122">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b8142-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="b8142-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b8142-123">usedLicenseCount</span></span>|<span data-ttu-id="b8142-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b8142-124">Int32</span></span>|<span data-ttu-id="b8142-125">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="b8142-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8142-126">Relações</span><span class="sxs-lookup"><span data-stu-id="b8142-126">Relationships</span></span>
<span data-ttu-id="b8142-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8142-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8142-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8142-128">JSON Representation</span></span>
<span data-ttu-id="b8142-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8142-129">Here is a JSON representation of the resource.</span></span>
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



