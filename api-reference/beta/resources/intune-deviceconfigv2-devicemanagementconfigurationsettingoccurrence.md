---
title: tipo de recurso deviceManagementConfigurationSettingOccurrence
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b8a93c75f011dba9816ee84a9ef8bf5cd05d275
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301470"
---
# <a name="devicemanagementconfigurationsettingoccurrence-resource-type"></a><span data-ttu-id="15c53-103">tipo de recurso deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="15c53-103">deviceManagementConfigurationSettingOccurrence resource type</span></span>

<span data-ttu-id="15c53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15c53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15c53-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15c53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15c53-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15c53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15c53-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15c53-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="15c53-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15c53-108">Properties</span></span>
|<span data-ttu-id="15c53-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15c53-109">Property</span></span>|<span data-ttu-id="15c53-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="15c53-110">Type</span></span>|<span data-ttu-id="15c53-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="15c53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c53-112">minDeviceOccurrence</span><span class="sxs-lookup"><span data-stu-id="15c53-112">minDeviceOccurrence</span></span>|<span data-ttu-id="15c53-113">Int32</span><span class="sxs-lookup"><span data-stu-id="15c53-113">Int32</span></span>|<span data-ttu-id="15c53-114">A configuração de horários mínimos pode ser definida em Device.</span><span class="sxs-lookup"><span data-stu-id="15c53-114">Minimum times setting can be set on device.</span></span> <span data-ttu-id="15c53-115">Um MinDeviceOccurrence de 0 significa que A configuração é opcional</span><span class="sxs-lookup"><span data-stu-id="15c53-115">A MinDeviceOccurrence of 0 means setting is optional</span></span>|
|<span data-ttu-id="15c53-116">maxDeviceOccurrence</span><span class="sxs-lookup"><span data-stu-id="15c53-116">maxDeviceOccurrence</span></span>|<span data-ttu-id="15c53-117">Int32</span><span class="sxs-lookup"><span data-stu-id="15c53-117">Int32</span></span>|<span data-ttu-id="15c53-118">A configuração de horários máximos pode ser definida em Device.</span><span class="sxs-lookup"><span data-stu-id="15c53-118">Maximum times setting can be set on device.</span></span> |

## <a name="relationships"></a><span data-ttu-id="15c53-119">Relações</span><span class="sxs-lookup"><span data-stu-id="15c53-119">Relationships</span></span>
<span data-ttu-id="15c53-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15c53-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15c53-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15c53-121">JSON Representation</span></span>
<span data-ttu-id="15c53-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15c53-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingOccurrence",
  "minDeviceOccurrence": 1024,
  "maxDeviceOccurrence": 1024
}
```




