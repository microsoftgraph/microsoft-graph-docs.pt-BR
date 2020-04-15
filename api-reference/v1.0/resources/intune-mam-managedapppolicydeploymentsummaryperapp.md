---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a0a4189c1f26736231155da775f137e7f61bbd23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468490"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="c9f25-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="c9f25-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="c9f25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9f25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9f25-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9f25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9f25-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9f25-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="c9f25-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9f25-107">Properties</span></span>
|<span data-ttu-id="c9f25-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9f25-108">Property</span></span>|<span data-ttu-id="c9f25-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9f25-109">Type</span></span>|<span data-ttu-id="c9f25-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9f25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f25-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9f25-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="c9f25-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9f25-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c9f25-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9f25-113">Deployment of an app.</span></span>|
|<span data-ttu-id="c9f25-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="c9f25-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="c9f25-115">Int32</span><span class="sxs-lookup"><span data-stu-id="c9f25-115">Int32</span></span>|<span data-ttu-id="c9f25-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="c9f25-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9f25-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c9f25-117">Relationships</span></span>
<span data-ttu-id="c9f25-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9f25-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9f25-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9f25-119">JSON Representation</span></span>
<span data-ttu-id="c9f25-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9f25-120">Here is a JSON representation of the resource.</span></span>
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







