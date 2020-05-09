---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4f9c3af886afa5c5d0e78f23bb55d9f764b0298
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177405"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="fc83e-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="fc83e-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="fc83e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc83e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc83e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc83e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc83e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc83e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc83e-107">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc83e-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="fc83e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc83e-108">Properties</span></span>
|<span data-ttu-id="fc83e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc83e-109">Property</span></span>|<span data-ttu-id="fc83e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc83e-110">Type</span></span>|<span data-ttu-id="fc83e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc83e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc83e-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fc83e-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="fc83e-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fc83e-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fc83e-114">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc83e-114">Deployment of an app.</span></span>|
|<span data-ttu-id="fc83e-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="fc83e-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="fc83e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fc83e-116">Int32</span></span>|<span data-ttu-id="fc83e-117">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="fc83e-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc83e-118">Relações</span><span class="sxs-lookup"><span data-stu-id="fc83e-118">Relationships</span></span>
<span data-ttu-id="fc83e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc83e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc83e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc83e-120">JSON Representation</span></span>
<span data-ttu-id="fc83e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc83e-121">Here is a JSON representation of the resource.</span></span>
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



