---
title: tipo de recurso de vppTokenLicenseSummary
description: Resumo de licenças de um determinado aplicativo em um token.
author: tfitzmac
ms.openlocfilehash: 7847c6265ed526d50215567918698c7732adf947
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319975"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="1449d-103">tipo de recurso de vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="1449d-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="1449d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1449d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1449d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1449d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1449d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1449d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1449d-107">Resumo de licenças de um determinado aplicativo em um token.</span><span class="sxs-lookup"><span data-stu-id="1449d-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="1449d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1449d-108">Properties</span></span>
|<span data-ttu-id="1449d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1449d-109">Property</span></span>|<span data-ttu-id="1449d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1449d-110">Type</span></span>|<span data-ttu-id="1449d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1449d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1449d-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="1449d-112">vppTokenId</span></span>|<span data-ttu-id="1449d-113">String</span><span class="sxs-lookup"><span data-stu-id="1449d-113">String</span></span>|<span data-ttu-id="1449d-114">Identificador do token VPP.</span><span class="sxs-lookup"><span data-stu-id="1449d-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="1449d-115">appleId</span><span class="sxs-lookup"><span data-stu-id="1449d-115">appleId</span></span>|<span data-ttu-id="1449d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1449d-116">String</span></span>|<span data-ttu-id="1449d-117">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="1449d-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1449d-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="1449d-118">organizationName</span></span>|<span data-ttu-id="1449d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1449d-119">String</span></span>|<span data-ttu-id="1449d-120">A organização associada com o Token de programa de compra de Volume Apple.</span><span class="sxs-lookup"><span data-stu-id="1449d-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1449d-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1449d-121">availableLicenseCount</span></span>|<span data-ttu-id="1449d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1449d-122">Int32</span></span>|<span data-ttu-id="1449d-123">O número de licenças VPP disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1449d-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="1449d-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1449d-124">usedLicenseCount</span></span>|<span data-ttu-id="1449d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1449d-125">Int32</span></span>|<span data-ttu-id="1449d-126">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="1449d-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1449d-127">Relações</span><span class="sxs-lookup"><span data-stu-id="1449d-127">Relationships</span></span>
<span data-ttu-id="1449d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1449d-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1449d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1449d-129">JSON Representation</span></span>
<span data-ttu-id="1449d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1449d-130">Here is a JSON representation of the resource.</span></span>
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





