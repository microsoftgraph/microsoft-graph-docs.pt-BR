---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5802d8f1d29174a8e4e01ee10e4bf66081d12ca6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373074"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="b63d1-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="b63d1-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="b63d1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b63d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b63d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b63d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b63d1-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b63d1-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="b63d1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b63d1-107">Properties</span></span>
|<span data-ttu-id="b63d1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b63d1-108">Property</span></span>|<span data-ttu-id="b63d1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b63d1-109">Type</span></span>|<span data-ttu-id="b63d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b63d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b63d1-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b63d1-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="b63d1-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b63d1-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b63d1-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b63d1-113">Deployment of an app.</span></span>|
|<span data-ttu-id="b63d1-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="b63d1-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="b63d1-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b63d1-115">Int32</span></span>|<span data-ttu-id="b63d1-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="b63d1-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b63d1-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b63d1-117">Relationships</span></span>
<span data-ttu-id="b63d1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b63d1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b63d1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b63d1-119">JSON Representation</span></span>
<span data-ttu-id="b63d1-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b63d1-120">Here is a JSON representation of the resource.</span></span>
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



