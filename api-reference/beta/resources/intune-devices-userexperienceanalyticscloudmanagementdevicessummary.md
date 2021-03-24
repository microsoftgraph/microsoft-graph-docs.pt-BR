---
title: tipo de recurso userExperienceAnalyticsCloudManagementDevicesSummary
description: A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0fb4e7d9a8ac5b2ab9c134d45c2e625a935b491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146744"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a><span data-ttu-id="606b9-103">tipo de recurso userExperienceAnalyticsCloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="606b9-103">userExperienceAnalyticsCloudManagementDevicesSummary resource type</span></span>

<span data-ttu-id="606b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="606b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="606b9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="606b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="606b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="606b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="606b9-107">A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.</span><span class="sxs-lookup"><span data-stu-id="606b9-107">The user experience work from anywhere Cloud management devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="606b9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="606b9-108">Properties</span></span>
|<span data-ttu-id="606b9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="606b9-109">Property</span></span>|<span data-ttu-id="606b9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="606b9-110">Type</span></span>|<span data-ttu-id="606b9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="606b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="606b9-112">coManagedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="606b9-112">coManagedDeviceCount</span></span>|<span data-ttu-id="606b9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="606b9-113">Int32</span></span>|<span data-ttu-id="606b9-114">Número total de dispositivos co-gerenciados.</span><span class="sxs-lookup"><span data-stu-id="606b9-114">Total number of  co-managed devices.</span></span>|
|<span data-ttu-id="606b9-115">intuneDeviceCount</span><span class="sxs-lookup"><span data-stu-id="606b9-115">intuneDeviceCount</span></span>|<span data-ttu-id="606b9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="606b9-116">Int32</span></span>|<span data-ttu-id="606b9-117">A contagem de dispositivos do intune que não estão no piloto automático registrado.</span><span class="sxs-lookup"><span data-stu-id="606b9-117">The count of intune devices that are not autopilot registerd.</span></span>|
|<span data-ttu-id="606b9-118">tenantAttachDeviceCount</span><span class="sxs-lookup"><span data-stu-id="606b9-118">tenantAttachDeviceCount</span></span>|<span data-ttu-id="606b9-119">Int32</span><span class="sxs-lookup"><span data-stu-id="606b9-119">Int32</span></span>|<span data-ttu-id="606b9-120">Contagem total de dispositivos de anexação de locatários.</span><span class="sxs-lookup"><span data-stu-id="606b9-120">Total count of tenant attach devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="606b9-121">Relações</span><span class="sxs-lookup"><span data-stu-id="606b9-121">Relationships</span></span>
<span data-ttu-id="606b9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="606b9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="606b9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="606b9-123">JSON Representation</span></span>
<span data-ttu-id="606b9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="606b9-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
  "coManagedDeviceCount": 1024,
  "intuneDeviceCount": 1024,
  "tenantAttachDeviceCount": 1024
}
```




