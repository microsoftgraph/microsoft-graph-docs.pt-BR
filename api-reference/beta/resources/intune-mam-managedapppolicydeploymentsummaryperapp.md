---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23fb9b2658bb15a851fca169c37bcf080d1c7c1c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803707"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="d6e6d-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="d6e6d-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="d6e6d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6e6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6e6d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6e6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6e6d-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6e6d-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="d6e6d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6e6d-107">Properties</span></span>
|<span data-ttu-id="d6e6d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6e6d-108">Property</span></span>|<span data-ttu-id="d6e6d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6e6d-109">Type</span></span>|<span data-ttu-id="d6e6d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6e6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6e6d-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6e6d-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="d6e6d-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6e6d-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d6e6d-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d6e6d-113">Deployment of an app.</span></span>|
|<span data-ttu-id="d6e6d-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="d6e6d-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="d6e6d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d6e6d-115">Int32</span></span>|<span data-ttu-id="d6e6d-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="d6e6d-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6e6d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d6e6d-117">Relationships</span></span>
<span data-ttu-id="d6e6d-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d6e6d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6e6d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6e6d-119">JSON Representation</span></span>
<span data-ttu-id="d6e6d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6e6d-120">Here is a JSON representation of the resource.</span></span>
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





