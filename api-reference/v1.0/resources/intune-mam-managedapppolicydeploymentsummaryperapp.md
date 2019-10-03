---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70c46530f979f7372b3592c310d4434246c5f0c1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367795"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="ef5e7-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ef5e7-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="ef5e7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef5e7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef5e7-105">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ef5e7-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="ef5e7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef5e7-106">Properties</span></span>
|<span data-ttu-id="ef5e7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef5e7-107">Property</span></span>|<span data-ttu-id="ef5e7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef5e7-108">Type</span></span>|<span data-ttu-id="ef5e7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef5e7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef5e7-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ef5e7-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="ef5e7-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ef5e7-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ef5e7-112">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ef5e7-112">Deployment of an app.</span></span>|
|<span data-ttu-id="ef5e7-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="ef5e7-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="ef5e7-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ef5e7-114">Int32</span></span>|<span data-ttu-id="ef5e7-115">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="ef5e7-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef5e7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ef5e7-116">Relationships</span></span>
<span data-ttu-id="ef5e7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef5e7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef5e7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef5e7-118">JSON Representation</span></span>
<span data-ttu-id="ef5e7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef5e7-119">Here is a JSON representation of the resource.</span></span>
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




