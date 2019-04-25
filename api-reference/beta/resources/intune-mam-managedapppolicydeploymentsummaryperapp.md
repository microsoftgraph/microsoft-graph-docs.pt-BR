---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23fb9b2658bb15a851fca169c37bcf080d1c7c1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573884"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="c032a-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="c032a-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="c032a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c032a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c032a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c032a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c032a-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c032a-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="c032a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c032a-107">Properties</span></span>
|<span data-ttu-id="c032a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c032a-108">Property</span></span>|<span data-ttu-id="c032a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c032a-109">Type</span></span>|<span data-ttu-id="c032a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c032a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c032a-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c032a-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="c032a-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c032a-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c032a-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c032a-113">Deployment of an app.</span></span>|
|<span data-ttu-id="c032a-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="c032a-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="c032a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="c032a-115">Int32</span></span>|<span data-ttu-id="c032a-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="c032a-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c032a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c032a-117">Relationships</span></span>
<span data-ttu-id="c032a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c032a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c032a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c032a-119">JSON Representation</span></span>
<span data-ttu-id="c032a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c032a-120">Here is a JSON representation of the resource.</span></span>
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





