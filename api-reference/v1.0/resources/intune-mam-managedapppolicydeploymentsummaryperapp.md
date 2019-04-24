---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 149a578f60ba5953f77c83ca2fbc3810931dffff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465297"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="f2374-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="f2374-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="f2374-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2374-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2374-105">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2374-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="f2374-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2374-106">Properties</span></span>
|<span data-ttu-id="f2374-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2374-107">Property</span></span>|<span data-ttu-id="f2374-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2374-108">Type</span></span>|<span data-ttu-id="f2374-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2374-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2374-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2374-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="f2374-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2374-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f2374-112">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2374-112">Deployment of an app.</span></span>|
|<span data-ttu-id="f2374-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="f2374-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="f2374-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f2374-114">Int32</span></span>|<span data-ttu-id="f2374-115">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="f2374-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2374-116">Relações</span><span class="sxs-lookup"><span data-stu-id="f2374-116">Relationships</span></span>
<span data-ttu-id="f2374-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f2374-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2374-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2374-118">JSON Representation</span></span>
<span data-ttu-id="f2374-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2374-119">Here is a JSON representation of the resource.</span></span>
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



