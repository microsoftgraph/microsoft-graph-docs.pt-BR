---
title: tipo de recurso de vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395178"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="4abd8-103">tipo de recurso de vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="4abd8-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="4abd8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4abd8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4abd8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4abd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4abd8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4abd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4abd8-107">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="4abd8-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="4abd8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4abd8-108">Properties</span></span>
|<span data-ttu-id="4abd8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4abd8-109">Property</span></span>|<span data-ttu-id="4abd8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4abd8-110">Type</span></span>|<span data-ttu-id="4abd8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4abd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4abd8-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="4abd8-112">vppTokenId</span></span>|<span data-ttu-id="4abd8-113">String</span><span class="sxs-lookup"><span data-stu-id="4abd8-113">String</span></span>|<span data-ttu-id="4abd8-114">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="4abd8-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="4abd8-115">appleId</span><span class="sxs-lookup"><span data-stu-id="4abd8-115">appleId</span></span>|<span data-ttu-id="4abd8-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4abd8-116">String</span></span>|<span data-ttu-id="4abd8-117">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="4abd8-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4abd8-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="4abd8-118">organizationName</span></span>|<span data-ttu-id="4abd8-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4abd8-119">String</span></span>|<span data-ttu-id="4abd8-120">A organização associada com o Token de programa de compra de Volume Apple.</span><span class="sxs-lookup"><span data-stu-id="4abd8-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="4abd8-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4abd8-121">availableLicenseCount</span></span>|<span data-ttu-id="4abd8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4abd8-122">Int32</span></span>|<span data-ttu-id="4abd8-123">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4abd8-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="4abd8-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4abd8-124">usedLicenseCount</span></span>|<span data-ttu-id="4abd8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4abd8-125">Int32</span></span>|<span data-ttu-id="4abd8-126">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="4abd8-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4abd8-127">Relações</span><span class="sxs-lookup"><span data-stu-id="4abd8-127">Relationships</span></span>
<span data-ttu-id="4abd8-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4abd8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4abd8-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4abd8-129">JSON Representation</span></span>
<span data-ttu-id="4abd8-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4abd8-130">Here is a JSON representation of the resource.</span></span>
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




