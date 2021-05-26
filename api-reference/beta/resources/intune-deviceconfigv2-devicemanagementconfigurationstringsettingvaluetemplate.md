---
title: Tipo de recurso deviceManagementConfigurationStringSettingValueTemplate
description: Modelo de valor de configuração de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db9e15e7aae70b4023aaf9305ef533ea37597e3b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666790"
---
# <a name="devicemanagementconfigurationstringsettingvaluetemplate-resource-type"></a><span data-ttu-id="4c221-103">Tipo de recurso deviceManagementConfigurationStringSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="4c221-103">deviceManagementConfigurationStringSettingValueTemplate resource type</span></span>

<span data-ttu-id="4c221-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c221-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c221-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c221-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c221-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c221-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c221-107">Modelo de valor de configuração de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c221-107">String Setting Value Template</span></span>


<span data-ttu-id="4c221-108">Herda [de deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="4c221-108">Inherits from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c221-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c221-109">Properties</span></span>
|<span data-ttu-id="4c221-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c221-110">Property</span></span>|<span data-ttu-id="4c221-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c221-111">Type</span></span>|<span data-ttu-id="4c221-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c221-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c221-113">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="4c221-113">settingValueTemplateId</span></span>|<span data-ttu-id="4c221-114">String</span><span class="sxs-lookup"><span data-stu-id="4c221-114">String</span></span>|<span data-ttu-id="4c221-115">Definição da ID do Modelo de Valor Herdada [de deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="4c221-115">Setting Value Template Id Inherited from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>|
|<span data-ttu-id="4c221-116">defaultValue</span><span class="sxs-lookup"><span data-stu-id="4c221-116">defaultValue</span></span>|[<span data-ttu-id="4c221-117">deviceManagementConfigurationStringSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="4c221-117">deviceManagementConfigurationStringSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)|<span data-ttu-id="4c221-118">Modelo padrão de valor de configuração de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="4c221-118">String Setting Value Default Template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c221-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4c221-119">Relationships</span></span>
<span data-ttu-id="4c221-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4c221-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c221-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c221-121">JSON Representation</span></span>
<span data-ttu-id="4c221-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c221-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
    "constantValue": "String"
  }
}
```




