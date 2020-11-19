---
title: tipo de recurso deviceManagementConfigurationSettingInstance
description: Configuração de instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 757b60c1e290612bbf51ac66ec42d3f27ac57cca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301471"
---
# <a name="devicemanagementconfigurationsettinginstance-resource-type"></a><span data-ttu-id="5f951-103">tipo de recurso deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="5f951-103">deviceManagementConfigurationSettingInstance resource type</span></span>

<span data-ttu-id="5f951-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f951-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f951-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5f951-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f951-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f951-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f951-107">Configuração de instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="5f951-107">Setting instance within policy</span></span>

## <a name="properties"></a><span data-ttu-id="5f951-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f951-108">Properties</span></span>
|<span data-ttu-id="5f951-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f951-109">Property</span></span>|<span data-ttu-id="5f951-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f951-110">Type</span></span>|<span data-ttu-id="5f951-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f951-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f951-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f951-112">settingDefinitionId</span></span>|<span data-ttu-id="5f951-113">String</span><span class="sxs-lookup"><span data-stu-id="5f951-113">String</span></span>|<span data-ttu-id="5f951-114">ID de definição de configuração</span><span class="sxs-lookup"><span data-stu-id="5f951-114">Setting Definition Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f951-115">Relações</span><span class="sxs-lookup"><span data-stu-id="5f951-115">Relationships</span></span>
<span data-ttu-id="5f951-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f951-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f951-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f951-117">JSON Representation</span></span>
<span data-ttu-id="5f951-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f951-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstance",
  "settingDefinitionId": "String"
}
```




