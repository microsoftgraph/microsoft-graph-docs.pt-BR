---
title: Tipo de recurso deviceManagementConfigurationSettingApplicability
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b95e92c7ee9d6e520a326cb8918dcbfe05f83725
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665074"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a><span data-ttu-id="dada2-103">Tipo de recurso deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="dada2-103">deviceManagementConfigurationSettingApplicability resource type</span></span>

<span data-ttu-id="dada2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dada2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dada2-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dada2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dada2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dada2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dada2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dada2-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dada2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dada2-108">Properties</span></span>
|<span data-ttu-id="dada2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dada2-109">Property</span></span>|<span data-ttu-id="dada2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dada2-110">Type</span></span>|<span data-ttu-id="dada2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dada2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dada2-112">description</span><span class="sxs-lookup"><span data-stu-id="dada2-112">description</span></span>|<span data-ttu-id="dada2-113">String</span><span class="sxs-lookup"><span data-stu-id="dada2-113">String</span></span>|<span data-ttu-id="dada2-114">descrição da configuração</span><span class="sxs-lookup"><span data-stu-id="dada2-114">description of the setting</span></span>|
|<span data-ttu-id="dada2-115">plataforma</span><span class="sxs-lookup"><span data-stu-id="dada2-115">platform</span></span>|[<span data-ttu-id="dada2-116">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="dada2-116">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="dada2-117">A configuração da plataforma pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="dada2-117">Platform setting can be applied on.</span></span> <span data-ttu-id="dada2-118">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="dada2-118">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="dada2-119">deviceMode</span><span class="sxs-lookup"><span data-stu-id="dada2-119">deviceMode</span></span>|[<span data-ttu-id="dada2-120">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dada2-120">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="dada2-121">Modo de Dispositivo em que a configuração pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="dada2-121">Device Mode that setting can be applied on.</span></span> <span data-ttu-id="dada2-122">Os valores possíveis são: `none` e `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="dada2-122">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="dada2-123">technologies</span><span class="sxs-lookup"><span data-stu-id="dada2-123">technologies</span></span>|[<span data-ttu-id="dada2-124">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="dada2-124">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="dada2-125">Por quais canais de tecnologia essa configuração pode ser implantada.</span><span class="sxs-lookup"><span data-stu-id="dada2-125">Which technology channels this setting can be deployed through.</span></span> <span data-ttu-id="dada2-126">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="dada2-126">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dada2-127">Relações</span><span class="sxs-lookup"><span data-stu-id="dada2-127">Relationships</span></span>
<span data-ttu-id="dada2-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dada2-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dada2-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dada2-129">JSON Representation</span></span>
<span data-ttu-id="dada2-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dada2-130">Here is a JSON representation of the resource.</span></span>
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




