---
title: tipo de recurso de embeddedSIMActivationCode
description: O código de ativação SIM incorporado como fornecido pela operadora móvel.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74f1725ab8f12cb103144dc1897e9bf965c5361b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422464"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="1689b-103">tipo de recurso de embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="1689b-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="1689b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1689b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1689b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1689b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1689b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1689b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1689b-107">O código de ativação SIM incorporado como fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="1689b-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="1689b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1689b-108">Properties</span></span>
|<span data-ttu-id="1689b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1689b-109">Property</span></span>|<span data-ttu-id="1689b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1689b-110">Type</span></span>|<span data-ttu-id="1689b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1689b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1689b-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="1689b-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="1689b-113">String</span><span class="sxs-lookup"><span data-stu-id="1689b-113">String</span></span>|<span data-ttu-id="1689b-114">O identificador de cartão de circuito integrado (ICCID) para que isso incorporada código de ativação SIM conforme fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="1689b-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="1689b-115">A entrada deve coincidir com a seguinte expressão regular: ' ^\[0-9\]{19}\[0-9\]?$ '.</span><span class="sxs-lookup"><span data-stu-id="1689b-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="1689b-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="1689b-116">matchingIdentifier</span></span>|<span data-ttu-id="1689b-117">String</span><span class="sxs-lookup"><span data-stu-id="1689b-117">String</span></span>|<span data-ttu-id="1689b-118">MatchingIdentifier (MatchingID) conforme especificado na GSMA associação SGP.22 RSP especificação técnica da seção 4.1.</span><span class="sxs-lookup"><span data-stu-id="1689b-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="1689b-119">A entrada deve coincidir com a seguinte expressão regular: ' ^\[a-zA-Z0-9\-\]\* $'.</span><span class="sxs-lookup"><span data-stu-id="1689b-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="1689b-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="1689b-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="1689b-121">String</span><span class="sxs-lookup"><span data-stu-id="1689b-121">String</span></span>|<span data-ttu-id="1689b-122">O nome de domínio totalmente qualificado da SM-DP + servidor conforme especificado na especificação técnica RSP GSM associação SPG.22.</span><span class="sxs-lookup"><span data-stu-id="1689b-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="1689b-123">A entrada deve coincidir com a seguinte expressão regular: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$'.</span><span class="sxs-lookup"><span data-stu-id="1689b-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1689b-124">Relações</span><span class="sxs-lookup"><span data-stu-id="1689b-124">Relationships</span></span>
<span data-ttu-id="1689b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1689b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1689b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1689b-126">JSON Representation</span></span>
<span data-ttu-id="1689b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1689b-127">Here is a JSON representation of the resource.</span></span>
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




