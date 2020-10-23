---
title: tipo de recurso vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9027a2f8c9d99eb829d48f734af272413e62aa18
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704727"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="82e3d-103">tipo de recurso vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="82e3d-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="82e3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82e3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82e3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82e3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82e3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82e3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82e3d-107">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="82e3d-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="82e3d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82e3d-108">Properties</span></span>
|<span data-ttu-id="82e3d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82e3d-109">Property</span></span>|<span data-ttu-id="82e3d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="82e3d-110">Type</span></span>|<span data-ttu-id="82e3d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82e3d-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="82e3d-112">vppTokenId</span></span>|<span data-ttu-id="82e3d-113">String</span><span class="sxs-lookup"><span data-stu-id="82e3d-113">String</span></span>|<span data-ttu-id="82e3d-114">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="82e3d-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="82e3d-115">appleId</span><span class="sxs-lookup"><span data-stu-id="82e3d-115">appleId</span></span>|<span data-ttu-id="82e3d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82e3d-116">String</span></span>|<span data-ttu-id="82e3d-117">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="82e3d-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="82e3d-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="82e3d-118">organizationName</span></span>|<span data-ttu-id="82e3d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82e3d-119">String</span></span>|<span data-ttu-id="82e3d-120">A organização associada ao token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="82e3d-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="82e3d-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="82e3d-121">availableLicenseCount</span></span>|<span data-ttu-id="82e3d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="82e3d-122">Int32</span></span>|<span data-ttu-id="82e3d-123">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="82e3d-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="82e3d-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="82e3d-124">usedLicenseCount</span></span>|<span data-ttu-id="82e3d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="82e3d-125">Int32</span></span>|<span data-ttu-id="82e3d-126">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="82e3d-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82e3d-127">Relações</span><span class="sxs-lookup"><span data-stu-id="82e3d-127">Relationships</span></span>
<span data-ttu-id="82e3d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82e3d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82e3d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82e3d-129">JSON Representation</span></span>
<span data-ttu-id="82e3d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82e3d-130">Here is a JSON representation of the resource.</span></span>
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





