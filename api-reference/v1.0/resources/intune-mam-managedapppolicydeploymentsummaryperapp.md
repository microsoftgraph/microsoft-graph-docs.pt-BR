---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84befe8b98b2e0e6883328c09bdee16e2720300d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037937"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="40013-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="40013-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="40013-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40013-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40013-105">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40013-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="40013-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40013-106">Properties</span></span>
|<span data-ttu-id="40013-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40013-107">Property</span></span>|<span data-ttu-id="40013-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="40013-108">Type</span></span>|<span data-ttu-id="40013-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40013-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40013-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="40013-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="40013-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="40013-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="40013-112">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40013-112">Deployment of an app.</span></span>|
|<span data-ttu-id="40013-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="40013-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="40013-114">Int32</span><span class="sxs-lookup"><span data-stu-id="40013-114">Int32</span></span>|<span data-ttu-id="40013-115">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="40013-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40013-116">Relações</span><span class="sxs-lookup"><span data-stu-id="40013-116">Relationships</span></span>
<span data-ttu-id="40013-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40013-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40013-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40013-118">JSON Representation</span></span>
<span data-ttu-id="40013-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40013-119">Here is a JSON representation of the resource.</span></span>
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



