---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b54021290b6cc66be6cd33c15bcda3492aca1cb0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730984"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="75ea8-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="75ea8-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="75ea8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ea8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75ea8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75ea8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75ea8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75ea8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ea8-107">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75ea8-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="75ea8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75ea8-108">Properties</span></span>
|<span data-ttu-id="75ea8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75ea8-109">Property</span></span>|<span data-ttu-id="75ea8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75ea8-110">Type</span></span>|<span data-ttu-id="75ea8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75ea8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75ea8-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="75ea8-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="75ea8-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="75ea8-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="75ea8-114">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75ea8-114">Deployment of an app.</span></span>|
|<span data-ttu-id="75ea8-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="75ea8-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="75ea8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="75ea8-116">Int32</span></span>|<span data-ttu-id="75ea8-117">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="75ea8-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75ea8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="75ea8-118">Relationships</span></span>
<span data-ttu-id="75ea8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75ea8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75ea8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75ea8-120">JSON Representation</span></span>
<span data-ttu-id="75ea8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75ea8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "configurationAppliedUserCount": 1024
}
```





