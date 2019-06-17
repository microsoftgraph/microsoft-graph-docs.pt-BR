---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1174e46f40a7f80944cf686a403edb0db60cb1fd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994724"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="a664b-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a664b-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="a664b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a664b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a664b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a664b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a664b-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a664b-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="a664b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a664b-107">Properties</span></span>
|<span data-ttu-id="a664b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a664b-108">Property</span></span>|<span data-ttu-id="a664b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a664b-109">Type</span></span>|<span data-ttu-id="a664b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a664b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a664b-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a664b-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="a664b-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a664b-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a664b-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a664b-113">Deployment of an app.</span></span>|
|<span data-ttu-id="a664b-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="a664b-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="a664b-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a664b-115">Int32</span></span>|<span data-ttu-id="a664b-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="a664b-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a664b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a664b-117">Relationships</span></span>
<span data-ttu-id="a664b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a664b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a664b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a664b-119">JSON Representation</span></span>
<span data-ttu-id="a664b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a664b-120">Here is a JSON representation of the resource.</span></span>
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





