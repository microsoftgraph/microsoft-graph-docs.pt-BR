---
title: tipo de recurso deviceManagementConfigurationSimpleSettingInstance
description: Instância de configuração simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52ee180adbdd19ac95aa70159f198797d75ec302
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241246"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a><span data-ttu-id="e6212-103">tipo de recurso deviceManagementConfigurationSimpleSettingInstance</span><span class="sxs-lookup"><span data-stu-id="e6212-103">deviceManagementConfigurationSimpleSettingInstance resource type</span></span>

<span data-ttu-id="e6212-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6212-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6212-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6212-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6212-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6212-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6212-107">Instância de configuração simples</span><span class="sxs-lookup"><span data-stu-id="e6212-107">Simple setting instance</span></span>


<span data-ttu-id="e6212-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e6212-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6212-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6212-109">Properties</span></span>
|<span data-ttu-id="e6212-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6212-110">Property</span></span>|<span data-ttu-id="e6212-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6212-111">Type</span></span>|<span data-ttu-id="e6212-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6212-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6212-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e6212-113">settingDefinitionId</span></span>|<span data-ttu-id="e6212-114">String</span><span class="sxs-lookup"><span data-stu-id="e6212-114">String</span></span>|<span data-ttu-id="e6212-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e6212-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="e6212-116">simpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="e6212-116">simpleSettingValue</span></span>|[<span data-ttu-id="e6212-117">deviceManagementConfigurationSimpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="e6212-117">deviceManagementConfigurationSimpleSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|<span data-ttu-id="e6212-118">Valor de instância da configuração simples</span><span class="sxs-lookup"><span data-stu-id="e6212-118">Simple setting instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6212-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e6212-119">Relationships</span></span>
<span data-ttu-id="e6212-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6212-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6212-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6212-121">JSON Representation</span></span>
<span data-ttu-id="e6212-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6212-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstance",
  "settingDefinitionId": "String",
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "value": "String"
  }
}
```




