---
title: tipo de recurso deviceManagementConfigurationSimpleSettingCollectionInstance
description: Instância de coleção de configurações simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0886b7665f1f3ce16780f2ecccc77635fd70cf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241230"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a><span data-ttu-id="f8fbc-103">tipo de recurso deviceManagementConfigurationSimpleSettingCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="f8fbc-103">deviceManagementConfigurationSimpleSettingCollectionInstance resource type</span></span>

<span data-ttu-id="f8fbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8fbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8fbc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8fbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8fbc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8fbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8fbc-107">Instância de coleção de configurações simples</span><span class="sxs-lookup"><span data-stu-id="f8fbc-107">Simple setting collection instance</span></span>


<span data-ttu-id="f8fbc-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="f8fbc-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8fbc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8fbc-109">Properties</span></span>
|<span data-ttu-id="f8fbc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8fbc-110">Property</span></span>|<span data-ttu-id="f8fbc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8fbc-111">Type</span></span>|<span data-ttu-id="f8fbc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8fbc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8fbc-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f8fbc-113">settingDefinitionId</span></span>|<span data-ttu-id="f8fbc-114">String</span><span class="sxs-lookup"><span data-stu-id="f8fbc-114">String</span></span>|<span data-ttu-id="f8fbc-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="f8fbc-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="f8fbc-116">simpleSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="f8fbc-116">simpleSettingCollectionValue</span></span>|<span data-ttu-id="f8fbc-117">coleção [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f8fbc-117">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) collection</span></span>|<span data-ttu-id="f8fbc-118">Valor de instância da coleção de configurações simples</span><span class="sxs-lookup"><span data-stu-id="f8fbc-118">Simple setting collection instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8fbc-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f8fbc-119">Relationships</span></span>
<span data-ttu-id="f8fbc-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8fbc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8fbc-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8fbc-121">JSON Representation</span></span>
<span data-ttu-id="f8fbc-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8fbc-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "value": "String"
    }
  ]
}
```




