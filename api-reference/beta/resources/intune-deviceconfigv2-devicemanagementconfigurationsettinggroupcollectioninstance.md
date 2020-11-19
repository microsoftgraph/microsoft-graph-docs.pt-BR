---
title: tipo de recurso deviceManagementConfigurationSettingGroupCollectionInstance
description: Configuração de instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e639dca60ff57d577f44a1bab4bc0b4420e174b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241140"
---
# <a name="devicemanagementconfigurationsettinggroupcollectioninstance-resource-type"></a><span data-ttu-id="5388e-103">tipo de recurso deviceManagementConfigurationSettingGroupCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="5388e-103">deviceManagementConfigurationSettingGroupCollectionInstance resource type</span></span>

<span data-ttu-id="5388e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5388e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5388e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5388e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5388e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5388e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5388e-107">Configuração de instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="5388e-107">Setting instance within policy</span></span>


<span data-ttu-id="5388e-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5388e-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5388e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5388e-109">Properties</span></span>
|<span data-ttu-id="5388e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5388e-110">Property</span></span>|<span data-ttu-id="5388e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5388e-111">Type</span></span>|<span data-ttu-id="5388e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5388e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5388e-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5388e-113">settingDefinitionId</span></span>|<span data-ttu-id="5388e-114">String</span><span class="sxs-lookup"><span data-stu-id="5388e-114">String</span></span>|<span data-ttu-id="5388e-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5388e-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5388e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="5388e-116">Relationships</span></span>
<span data-ttu-id="5388e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5388e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5388e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5388e-118">JSON Representation</span></span>
<span data-ttu-id="5388e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5388e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance",
  "settingDefinitionId": "String"
}
```




