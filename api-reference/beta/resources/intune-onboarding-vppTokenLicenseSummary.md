---
title: tipo de recurso de vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0766fd4da996b57032154be98bbc22fd8c8a4a5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939956"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="db725-103">tipo de recurso de vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="db725-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="db725-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db725-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db725-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db725-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db725-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="db725-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db725-107">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="db725-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="db725-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db725-108">Properties</span></span>
|<span data-ttu-id="db725-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db725-109">Property</span></span>|<span data-ttu-id="db725-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="db725-110">Type</span></span>|<span data-ttu-id="db725-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="db725-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db725-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="db725-112">vppTokenId</span></span>|<span data-ttu-id="db725-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db725-113">String</span></span>|<span data-ttu-id="db725-114">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="db725-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="db725-115">appleId</span><span class="sxs-lookup"><span data-stu-id="db725-115">appleId</span></span>|<span data-ttu-id="db725-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db725-116">String</span></span>|<span data-ttu-id="db725-117">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="db725-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="db725-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="db725-118">organizationName</span></span>|<span data-ttu-id="db725-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db725-119">String</span></span>|<span data-ttu-id="db725-120">A organização associada com o Token de programa de compra de Volume Apple.</span><span class="sxs-lookup"><span data-stu-id="db725-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="db725-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="db725-121">availableLicenseCount</span></span>|<span data-ttu-id="db725-122">Int32</span><span class="sxs-lookup"><span data-stu-id="db725-122">Int32</span></span>|<span data-ttu-id="db725-123">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="db725-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="db725-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="db725-124">usedLicenseCount</span></span>|<span data-ttu-id="db725-125">Int32</span><span class="sxs-lookup"><span data-stu-id="db725-125">Int32</span></span>|<span data-ttu-id="db725-126">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="db725-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db725-127">Relações</span><span class="sxs-lookup"><span data-stu-id="db725-127">Relationships</span></span>
<span data-ttu-id="db725-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db725-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="db725-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db725-129">JSON Representation</span></span>
<span data-ttu-id="db725-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db725-130">Here is a JSON representation of the resource.</span></span>
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





