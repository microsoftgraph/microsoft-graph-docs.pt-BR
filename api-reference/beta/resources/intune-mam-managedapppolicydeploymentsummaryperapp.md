---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4e55ad697ca091ac650f47a92f384ec847d2d08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030231"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="86a44-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="86a44-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="86a44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86a44-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86a44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a44-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86a44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a44-107">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86a44-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="86a44-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86a44-108">Properties</span></span>
|<span data-ttu-id="86a44-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86a44-109">Property</span></span>|<span data-ttu-id="86a44-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a44-110">Type</span></span>|<span data-ttu-id="86a44-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a44-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="86a44-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="86a44-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="86a44-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="86a44-114">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86a44-114">Deployment of an app.</span></span>|
|<span data-ttu-id="86a44-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="86a44-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="86a44-116">Int32</span><span class="sxs-lookup"><span data-stu-id="86a44-116">Int32</span></span>|<span data-ttu-id="86a44-117">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="86a44-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86a44-118">Relações</span><span class="sxs-lookup"><span data-stu-id="86a44-118">Relationships</span></span>
<span data-ttu-id="86a44-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86a44-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86a44-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86a44-120">JSON Representation</span></span>
<span data-ttu-id="86a44-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86a44-121">Here is a JSON representation of the resource.</span></span>
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






