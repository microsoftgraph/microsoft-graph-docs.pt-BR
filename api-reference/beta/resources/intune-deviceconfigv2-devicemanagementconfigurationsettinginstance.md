---
title: Tipo de recurso deviceManagementConfigurationSettingInstance
description: Definindo instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84b3b3a641fc8710bdd1b4266f15436084d01bdc
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665599"
---
# <a name="devicemanagementconfigurationsettinginstance-resource-type"></a><span data-ttu-id="2af75-103">Tipo de recurso deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2af75-103">deviceManagementConfigurationSettingInstance resource type</span></span>

<span data-ttu-id="2af75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2af75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2af75-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2af75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2af75-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2af75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2af75-107">Definindo instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="2af75-107">Setting instance within policy</span></span>

## <a name="properties"></a><span data-ttu-id="2af75-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2af75-108">Properties</span></span>
|<span data-ttu-id="2af75-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2af75-109">Property</span></span>|<span data-ttu-id="2af75-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2af75-110">Type</span></span>|<span data-ttu-id="2af75-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2af75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2af75-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2af75-112">settingDefinitionId</span></span>|<span data-ttu-id="2af75-113">String</span><span class="sxs-lookup"><span data-stu-id="2af75-113">String</span></span>|<span data-ttu-id="2af75-114">Definindo id de definição</span><span class="sxs-lookup"><span data-stu-id="2af75-114">Setting Definition Id</span></span>|
|<span data-ttu-id="2af75-115">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="2af75-115">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="2af75-116">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="2af75-116">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="2af75-117">Referência do modelo de instância de configuração</span><span class="sxs-lookup"><span data-stu-id="2af75-117">Setting Instance Template Reference</span></span>|

## <a name="relationships"></a><span data-ttu-id="2af75-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2af75-118">Relationships</span></span>
<span data-ttu-id="2af75-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2af75-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2af75-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2af75-120">JSON Representation</span></span>
<span data-ttu-id="2af75-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2af75-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




