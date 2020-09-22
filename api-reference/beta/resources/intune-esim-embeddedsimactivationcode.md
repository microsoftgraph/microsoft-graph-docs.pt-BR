---
title: tipo de recurso embeddedSIMActivationCode
description: O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ce61524e60e59d0fb0f8cdd1633e2c46d463c6e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031519"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="86905-103">tipo de recurso embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="86905-103">embeddedSIMActivationCode resource type</span></span>

<span data-ttu-id="86905-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86905-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86905-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86905-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86905-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86905-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86905-107">O código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="86905-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="86905-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86905-108">Properties</span></span>
|<span data-ttu-id="86905-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86905-109">Property</span></span>|<span data-ttu-id="86905-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="86905-110">Type</span></span>|<span data-ttu-id="86905-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86905-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86905-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="86905-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="86905-113">String</span><span class="sxs-lookup"><span data-stu-id="86905-113">String</span></span>|<span data-ttu-id="86905-114">O ICCID (identificador de cartão de circuito integrado) para este código de ativação do SIM incorporado, conforme fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="86905-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="86905-115">A entrada deve corresponder à seguinte expressão regular: ' ^ \[ 0-9 \] {19} \[ 0-9 \] ? $ '.</span><span class="sxs-lookup"><span data-stu-id="86905-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="86905-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="86905-116">matchingIdentifier</span></span>|<span data-ttu-id="86905-117">String</span><span class="sxs-lookup"><span data-stu-id="86905-117">String</span></span>|<span data-ttu-id="86905-118">O MatchingIdentifier (matchid) conforme especificado na SGP de associação GSMA. 22 RSP Technical Specification seção 4,1.</span><span class="sxs-lookup"><span data-stu-id="86905-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="86905-119">A entrada deve corresponder à seguinte expressão regular: ' ^ \[ a-zA-Z0-9 \- \] \* $ '.</span><span class="sxs-lookup"><span data-stu-id="86905-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="86905-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="86905-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="86905-121">String</span><span class="sxs-lookup"><span data-stu-id="86905-121">String</span></span>|<span data-ttu-id="86905-122">O nome de domínio totalmente qualificado do servidor SM-DP + conforme especificado na especificação técnica SPG da Associação GSM .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="86905-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="86905-123">A entrada deve corresponder à seguinte expressão regular: ' ^ ( \[ a-zA-Z0-9 \] + (- \[ a-zA-Z0-9 \] +) \* \. ) + \[ a-zA-Z \] {2,} $ '.</span><span class="sxs-lookup"><span data-stu-id="86905-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86905-124">Relações</span><span class="sxs-lookup"><span data-stu-id="86905-124">Relationships</span></span>
<span data-ttu-id="86905-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86905-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86905-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86905-126">JSON Representation</span></span>
<span data-ttu-id="86905-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86905-127">Here is a JSON representation of the resource.</span></span>
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






