---
title: Tipo de recurso managedAppPolicyDeploymentSummaryPerApp
description: Representa o resumo da implantação da política por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8143ce4a88fa40361c2a9c8091532172408b094c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302458"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="60cb1-103">Tipo de recurso managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="60cb1-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="60cb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60cb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60cb1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60cb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60cb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60cb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60cb1-107">Representa o resumo da implantação da política por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="60cb1-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="60cb1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60cb1-108">Properties</span></span>
|<span data-ttu-id="60cb1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60cb1-109">Property</span></span>|<span data-ttu-id="60cb1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="60cb1-110">Type</span></span>|<span data-ttu-id="60cb1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60cb1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60cb1-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="60cb1-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="60cb1-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="60cb1-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="60cb1-114">Implantação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="60cb1-114">Deployment of an app.</span></span>|
|<span data-ttu-id="60cb1-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="60cb1-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="60cb1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="60cb1-116">Int32</span></span>|<span data-ttu-id="60cb1-117">Número de usuários aos quais a política foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="60cb1-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60cb1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="60cb1-118">Relationships</span></span>
<span data-ttu-id="60cb1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60cb1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60cb1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60cb1-120">JSON Representation</span></span>
<span data-ttu-id="60cb1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60cb1-121">Here is a JSON representation of the resource.</span></span>
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




