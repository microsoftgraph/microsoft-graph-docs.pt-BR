---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
ms.openlocfilehash: 56b7952049c6ad41ee46f6b77c821aa32b1c4de8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006394"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="ac6a2-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ac6a2-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="ac6a2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ac6a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac6a2-105">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac6a2-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="ac6a2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac6a2-106">Properties</span></span>
|<span data-ttu-id="ac6a2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac6a2-107">Property</span></span>|<span data-ttu-id="ac6a2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac6a2-108">Type</span></span>|<span data-ttu-id="ac6a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac6a2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6a2-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac6a2-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="ac6a2-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac6a2-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ac6a2-112">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac6a2-112">Deployment of an app.</span></span>|
|<span data-ttu-id="ac6a2-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="ac6a2-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="ac6a2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6a2-114">Int32</span></span>|<span data-ttu-id="ac6a2-115">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="ac6a2-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6a2-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ac6a2-116">Relationships</span></span>
<span data-ttu-id="ac6a2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac6a2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac6a2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac6a2-118">JSON Representation</span></span>
<span data-ttu-id="ac6a2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac6a2-119">Here is a JSON representation of the resource.</span></span>
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



