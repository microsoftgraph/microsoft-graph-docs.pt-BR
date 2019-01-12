---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac5acf2536b669c42a324fd5761bed6333dbf05a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932956"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="a51c7-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a51c7-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="a51c7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a51c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a51c7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a51c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a51c7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a51c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a51c7-107">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a51c7-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="a51c7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a51c7-108">Properties</span></span>
|<span data-ttu-id="a51c7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a51c7-109">Property</span></span>|<span data-ttu-id="a51c7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a51c7-110">Type</span></span>|<span data-ttu-id="a51c7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a51c7-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a51c7-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="a51c7-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a51c7-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a51c7-114">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a51c7-114">Deployment of an app.</span></span>|
|<span data-ttu-id="a51c7-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="a51c7-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="a51c7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a51c7-116">Int32</span></span>|<span data-ttu-id="a51c7-117">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="a51c7-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a51c7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a51c7-118">Relationships</span></span>
<span data-ttu-id="a51c7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a51c7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a51c7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a51c7-120">JSON Representation</span></span>
<span data-ttu-id="a51c7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a51c7-121">Here is a JSON representation of the resource.</span></span>
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





