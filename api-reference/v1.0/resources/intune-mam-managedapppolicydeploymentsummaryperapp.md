---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1bcf69e4a8d24af3f0ada2ceae5730cc0cfdc18
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752326"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="37e6a-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="37e6a-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="37e6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37e6a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37e6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e6a-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37e6a-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="37e6a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37e6a-107">Properties</span></span>
|<span data-ttu-id="37e6a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37e6a-108">Property</span></span>|<span data-ttu-id="37e6a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37e6a-109">Type</span></span>|<span data-ttu-id="37e6a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e6a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e6a-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="37e6a-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="37e6a-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="37e6a-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="37e6a-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="37e6a-113">Deployment of an app.</span></span>|
|<span data-ttu-id="37e6a-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="37e6a-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="37e6a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="37e6a-115">Int32</span></span>|<span data-ttu-id="37e6a-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="37e6a-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37e6a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="37e6a-117">Relationships</span></span>
<span data-ttu-id="37e6a-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="37e6a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37e6a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37e6a-119">JSON Representation</span></span>
<span data-ttu-id="37e6a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37e6a-120">Here is a JSON representation of the resource.</span></span>
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




