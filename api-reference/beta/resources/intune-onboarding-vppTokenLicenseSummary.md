---
title: tipo de recurso de vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e5972341aa3b390ae226d19f7d85fe918345c627
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824861"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="edaa4-103">tipo de recurso de vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="edaa4-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="edaa4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="edaa4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edaa4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="edaa4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edaa4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="edaa4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edaa4-107">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="edaa4-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="edaa4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edaa4-108">Properties</span></span>
|<span data-ttu-id="edaa4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edaa4-109">Property</span></span>|<span data-ttu-id="edaa4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="edaa4-110">Type</span></span>|<span data-ttu-id="edaa4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="edaa4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edaa4-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="edaa4-112">vppTokenId</span></span>|<span data-ttu-id="edaa4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edaa4-113">String</span></span>|<span data-ttu-id="edaa4-114">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="edaa4-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="edaa4-115">appleId</span><span class="sxs-lookup"><span data-stu-id="edaa4-115">appleId</span></span>|<span data-ttu-id="edaa4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edaa4-116">String</span></span>|<span data-ttu-id="edaa4-117">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="edaa4-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="edaa4-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="edaa4-118">organizationName</span></span>|<span data-ttu-id="edaa4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edaa4-119">String</span></span>|<span data-ttu-id="edaa4-120">A organização associada com o Token de programa de compra de Volume Apple.</span><span class="sxs-lookup"><span data-stu-id="edaa4-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="edaa4-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="edaa4-121">availableLicenseCount</span></span>|<span data-ttu-id="edaa4-122">Int32</span><span class="sxs-lookup"><span data-stu-id="edaa4-122">Int32</span></span>|<span data-ttu-id="edaa4-123">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="edaa4-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="edaa4-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="edaa4-124">usedLicenseCount</span></span>|<span data-ttu-id="edaa4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="edaa4-125">Int32</span></span>|<span data-ttu-id="edaa4-126">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="edaa4-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edaa4-127">Relações</span><span class="sxs-lookup"><span data-stu-id="edaa4-127">Relationships</span></span>
<span data-ttu-id="edaa4-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="edaa4-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="edaa4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edaa4-129">JSON Representation</span></span>
<span data-ttu-id="edaa4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edaa4-130">Here is a JSON representation of the resource.</span></span>
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





