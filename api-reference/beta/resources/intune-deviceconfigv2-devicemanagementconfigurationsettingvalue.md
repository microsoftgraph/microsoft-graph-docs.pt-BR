---
title: Tipo de recurso deviceManagementConfigurationSettingValue
description: Valor de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 882946dbcf9440ceacc37a1c843f169ed9e2b1a0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666237"
---
# <a name="devicemanagementconfigurationsettingvalue-resource-type"></a><span data-ttu-id="77cb1-103">Tipo de recurso deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="77cb1-103">deviceManagementConfigurationSettingValue resource type</span></span>

<span data-ttu-id="77cb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77cb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77cb1-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77cb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77cb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77cb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77cb1-107">Valor de configuração</span><span class="sxs-lookup"><span data-stu-id="77cb1-107">Setting value</span></span>

## <a name="properties"></a><span data-ttu-id="77cb1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77cb1-108">Properties</span></span>
|<span data-ttu-id="77cb1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77cb1-109">Property</span></span>|<span data-ttu-id="77cb1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="77cb1-110">Type</span></span>|<span data-ttu-id="77cb1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77cb1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77cb1-112">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="77cb1-112">settingValueTemplateReference</span></span>|[<span data-ttu-id="77cb1-113">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="77cb1-113">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="77cb1-114">Referência do modelo de valor de configuração</span><span class="sxs-lookup"><span data-stu-id="77cb1-114">Setting value template reference</span></span>|

## <a name="relationships"></a><span data-ttu-id="77cb1-115">Relações</span><span class="sxs-lookup"><span data-stu-id="77cb1-115">Relationships</span></span>
<span data-ttu-id="77cb1-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="77cb1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77cb1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77cb1-117">JSON Representation</span></span>
<span data-ttu-id="77cb1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77cb1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```




