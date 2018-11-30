---
title: tipo de recurso de embeddedSIMActivationCode
description: O código de ativação SIM incorporado como fornecido pela operadora móvel.
ms.openlocfilehash: ad0b5d9ff2ac06387d81354cf74f2784d4838600
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039089"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="bda9a-103">tipo de recurso de embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="bda9a-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="bda9a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bda9a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bda9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bda9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bda9a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bda9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bda9a-107">O código de ativação SIM incorporado como fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="bda9a-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="bda9a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bda9a-108">Properties</span></span>
|<span data-ttu-id="bda9a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bda9a-109">Property</span></span>|<span data-ttu-id="bda9a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bda9a-110">Type</span></span>|<span data-ttu-id="bda9a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bda9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda9a-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="bda9a-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="bda9a-113">String</span><span class="sxs-lookup"><span data-stu-id="bda9a-113">String</span></span>|<span data-ttu-id="bda9a-114">O identificador de cartão de circuito integrado (ICCID) para que isso incorporada código de ativação SIM conforme fornecido pela operadora móvel.</span><span class="sxs-lookup"><span data-stu-id="bda9a-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="bda9a-115">A entrada deve coincidir com a seguinte expressão regular: ' ^\[0-9\]{19}\[0-9\]?$ '.</span><span class="sxs-lookup"><span data-stu-id="bda9a-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="bda9a-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="bda9a-116">matchingIdentifier</span></span>|<span data-ttu-id="bda9a-117">String</span><span class="sxs-lookup"><span data-stu-id="bda9a-117">String</span></span>|<span data-ttu-id="bda9a-118">MatchingIdentifier (MatchingID) conforme especificado na GSMA associação SGP.22 RSP especificação técnica da seção 4.1.</span><span class="sxs-lookup"><span data-stu-id="bda9a-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="bda9a-119">A entrada deve coincidir com a seguinte expressão regular: ' ^\[a-zA-Z0-9\-\]\* $'.</span><span class="sxs-lookup"><span data-stu-id="bda9a-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="bda9a-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="bda9a-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="bda9a-121">String</span><span class="sxs-lookup"><span data-stu-id="bda9a-121">String</span></span>|<span data-ttu-id="bda9a-122">O nome de domínio totalmente qualificado da SM-DP + servidor conforme especificado na especificação técnica RSP GSM associação SPG.22.</span><span class="sxs-lookup"><span data-stu-id="bda9a-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="bda9a-123">A entrada deve coincidir com a seguinte expressão regular: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$'.</span><span class="sxs-lookup"><span data-stu-id="bda9a-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda9a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="bda9a-124">Relationships</span></span>
<span data-ttu-id="bda9a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bda9a-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bda9a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bda9a-126">JSON Representation</span></span>
<span data-ttu-id="bda9a-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bda9a-127">Here is a JSON representation of the resource.</span></span>
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





