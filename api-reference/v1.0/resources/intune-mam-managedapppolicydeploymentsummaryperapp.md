---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 025103e40e3babde67437952fe8730b0f04410d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855164"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="86ee4-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="86ee4-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="86ee4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="86ee4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86ee4-105">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86ee4-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="86ee4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86ee4-106">Properties</span></span>
|<span data-ttu-id="86ee4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86ee4-107">Property</span></span>|<span data-ttu-id="86ee4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="86ee4-108">Type</span></span>|<span data-ttu-id="86ee4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86ee4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ee4-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="86ee4-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="86ee4-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="86ee4-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="86ee4-112">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86ee4-112">Deployment of an app.</span></span>|
|<span data-ttu-id="86ee4-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="86ee4-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="86ee4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="86ee4-114">Int32</span></span>|<span data-ttu-id="86ee4-115">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="86ee4-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86ee4-116">Relações</span><span class="sxs-lookup"><span data-stu-id="86ee4-116">Relationships</span></span>
<span data-ttu-id="86ee4-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86ee4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86ee4-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86ee4-118">JSON Representation</span></span>
<span data-ttu-id="86ee4-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86ee4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```



