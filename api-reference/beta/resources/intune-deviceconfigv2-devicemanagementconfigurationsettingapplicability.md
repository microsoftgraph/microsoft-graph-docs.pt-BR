---
title: tipo de recurso deviceManagementConfigurationSettingApplicability
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f94bfffd8dd3149d11e7ada38a4c238f4ce618a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241146"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a><span data-ttu-id="9fa21-103">tipo de recurso deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="9fa21-103">deviceManagementConfigurationSettingApplicability resource type</span></span>

<span data-ttu-id="9fa21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fa21-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9fa21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fa21-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fa21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa21-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fa21-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9fa21-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fa21-108">Properties</span></span>
|<span data-ttu-id="9fa21-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fa21-109">Property</span></span>|<span data-ttu-id="9fa21-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fa21-110">Type</span></span>|<span data-ttu-id="9fa21-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fa21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa21-112">description</span><span class="sxs-lookup"><span data-stu-id="9fa21-112">description</span></span>|<span data-ttu-id="9fa21-113">String</span><span class="sxs-lookup"><span data-stu-id="9fa21-113">String</span></span>|<span data-ttu-id="9fa21-114">Descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="9fa21-114">description of the setting</span></span>|
|<span data-ttu-id="9fa21-115">plataforma</span><span class="sxs-lookup"><span data-stu-id="9fa21-115">platform</span></span>|[<span data-ttu-id="9fa21-116">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="9fa21-116">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="9fa21-117">A configuração de plataforma pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="9fa21-117">Platform setting can be applied on.</span></span> <span data-ttu-id="9fa21-118">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="9fa21-118">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="9fa21-119">devicemode</span><span class="sxs-lookup"><span data-stu-id="9fa21-119">deviceMode</span></span>|[<span data-ttu-id="9fa21-120">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9fa21-120">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="9fa21-121">O modo de dispositivo para o qual a configuração pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="9fa21-121">Device Mode that setting can be applied on.</span></span> <span data-ttu-id="9fa21-122">Os valores possíveis são: `none` e `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="9fa21-122">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="9fa21-123">tecnologias</span><span class="sxs-lookup"><span data-stu-id="9fa21-123">technologies</span></span>|[<span data-ttu-id="9fa21-124">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="9fa21-124">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="9fa21-125">Quais canais de tecnologia essa configuração pode ser implantada.</span><span class="sxs-lookup"><span data-stu-id="9fa21-125">Which technology channels this setting can be deployed through.</span></span> <span data-ttu-id="9fa21-126">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="9fa21-126">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa21-127">Relações</span><span class="sxs-lookup"><span data-stu-id="9fa21-127">Relationships</span></span>
<span data-ttu-id="9fa21-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fa21-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fa21-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fa21-129">JSON Representation</span></span>
<span data-ttu-id="9fa21-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fa21-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```




