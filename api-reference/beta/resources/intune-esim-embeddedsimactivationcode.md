---
title: tipo de recurso embeddedSIMActivationCode
description: O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c44b685c46b300ced8d81d61de9308648c69eacc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787628"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="4a6bc-103">tipo de recurso embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="4a6bc-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="4a6bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a6bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a6bc-106">O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="4a6bc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a6bc-107">Properties</span></span>
|<span data-ttu-id="4a6bc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a6bc-108">Property</span></span>|<span data-ttu-id="4a6bc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a6bc-109">Type</span></span>|<span data-ttu-id="4a6bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a6bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a6bc-111">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a6bc-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="4a6bc-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a6bc-112">String</span></span>|<span data-ttu-id="4a6bc-113">O ICCID (identificador de cartão de circuito integrado) para este código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="4a6bc-114">a entrada deve corresponder à seguinte expressão regular: ' ^\[0-9\]{19}\[0-9\]? $ '.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="4a6bc-115">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a6bc-115">matchingIdentifier</span></span>|<span data-ttu-id="4a6bc-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a6bc-116">String</span></span>|<span data-ttu-id="4a6bc-117">O MatchingIdentifier (matchid) conforme especificado na SGP de associação GSMA. 22 RSP Technical Specification seção 4,1.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="4a6bc-118">A entrada deve corresponder à seguinte expressão regular: ' ^\[a-zA-Z0-9\-\]\* $ '.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="4a6bc-119">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="4a6bc-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="4a6bc-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a6bc-120">String</span></span>|<span data-ttu-id="4a6bc-121">O nome de domínio totalmente qualificado do servidor SM-DP + conforme especificado na especificação técnica SPG da Associação GSM .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="4a6bc-122">A entrada deve corresponder à seguinte expressão regular: ' ^ (\[a-zA-Z0-9\]+ (-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$ '.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a6bc-123">Relações</span><span class="sxs-lookup"><span data-stu-id="4a6bc-123">Relationships</span></span>
<span data-ttu-id="4a6bc-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4a6bc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a6bc-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a6bc-125">JSON Representation</span></span>
<span data-ttu-id="4a6bc-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a6bc-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





