---
title: tipo de recurso vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47d56f27ac08d1b4ca657973cf6e5ae0690ba498
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527698"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="b4164-103">tipo de recurso vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="b4164-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="b4164-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b4164-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4164-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4164-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4164-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4164-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4164-107">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="b4164-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="b4164-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4164-108">Properties</span></span>
|<span data-ttu-id="b4164-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4164-109">Property</span></span>|<span data-ttu-id="b4164-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4164-110">Type</span></span>|<span data-ttu-id="b4164-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4164-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4164-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b4164-112">vppTokenId</span></span>|<span data-ttu-id="b4164-113">String</span><span class="sxs-lookup"><span data-stu-id="b4164-113">String</span></span>|<span data-ttu-id="b4164-114">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="b4164-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="b4164-115">appleId</span><span class="sxs-lookup"><span data-stu-id="b4164-115">appleId</span></span>|<span data-ttu-id="b4164-116">String</span><span class="sxs-lookup"><span data-stu-id="b4164-116">String</span></span>|<span data-ttu-id="b4164-117">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="b4164-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4164-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="b4164-118">organizationName</span></span>|<span data-ttu-id="b4164-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4164-119">String</span></span>|<span data-ttu-id="b4164-120">A organização associada ao token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b4164-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b4164-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b4164-121">availableLicenseCount</span></span>|<span data-ttu-id="b4164-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b4164-122">Int32</span></span>|<span data-ttu-id="b4164-123">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b4164-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="b4164-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b4164-124">usedLicenseCount</span></span>|<span data-ttu-id="b4164-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b4164-125">Int32</span></span>|<span data-ttu-id="b4164-126">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="b4164-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4164-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b4164-127">Relationships</span></span>
<span data-ttu-id="b4164-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4164-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4164-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4164-129">JSON Representation</span></span>
<span data-ttu-id="b4164-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4164-130">Here is a JSON representation of the resource.</span></span>
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



