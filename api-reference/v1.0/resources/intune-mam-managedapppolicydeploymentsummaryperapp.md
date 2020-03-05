---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf9ff99bdcbfb7ea484a656c540449161a53d45d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448358"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="f5dc4-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="f5dc4-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="f5dc4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5dc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5dc4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5dc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5dc4-106">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5dc4-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="f5dc4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5dc4-107">Properties</span></span>
|<span data-ttu-id="f5dc4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5dc4-108">Property</span></span>|<span data-ttu-id="f5dc4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5dc4-109">Type</span></span>|<span data-ttu-id="f5dc4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5dc4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5dc4-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f5dc4-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="f5dc4-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f5dc4-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f5dc4-113">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5dc4-113">Deployment of an app.</span></span>|
|<span data-ttu-id="f5dc4-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="f5dc4-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="f5dc4-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f5dc4-115">Int32</span></span>|<span data-ttu-id="f5dc4-116">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="f5dc4-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5dc4-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f5dc4-117">Relationships</span></span>
<span data-ttu-id="f5dc4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5dc4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5dc4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5dc4-119">JSON Representation</span></span>
<span data-ttu-id="f5dc4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5dc4-120">Here is a JSON representation of the resource.</span></span>
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




