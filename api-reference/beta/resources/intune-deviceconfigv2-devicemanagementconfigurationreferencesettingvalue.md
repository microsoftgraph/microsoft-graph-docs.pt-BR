---
title: Tipo de recurso deviceManagementConfigurationReferenceSettingValue
description: Modelo para ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1656b3e50094a55b4f2fe9ad422bbd54bd62bd6b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666454"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a><span data-ttu-id="6af48-103">Tipo de recurso deviceManagementConfigurationReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="6af48-103">deviceManagementConfigurationReferenceSettingValue resource type</span></span>

<span data-ttu-id="6af48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6af48-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6af48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6af48-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6af48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6af48-107">Modelo para ReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="6af48-107">Model for ReferenceSettingValue</span></span>


<span data-ttu-id="6af48-108">Herda [de deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6af48-108">Inherits from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6af48-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6af48-109">Properties</span></span>
|<span data-ttu-id="6af48-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6af48-110">Property</span></span>|<span data-ttu-id="6af48-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6af48-111">Type</span></span>|<span data-ttu-id="6af48-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6af48-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6af48-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="6af48-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="6af48-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="6af48-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="6af48-115">Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6af48-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="6af48-116">value</span><span class="sxs-lookup"><span data-stu-id="6af48-116">value</span></span>|<span data-ttu-id="6af48-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6af48-117">String</span></span>|<span data-ttu-id="6af48-118">Valor da configuração da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="6af48-118">Value of the string setting.</span></span> <span data-ttu-id="6af48-119">Herdado [de deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6af48-119">Inherited from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>|
|<span data-ttu-id="6af48-120">observação</span><span class="sxs-lookup"><span data-stu-id="6af48-120">note</span></span>|<span data-ttu-id="6af48-121">String</span><span class="sxs-lookup"><span data-stu-id="6af48-121">String</span></span>|<span data-ttu-id="6af48-122">Uma observação que o administrador pode usar para colocar algumas informações contextuais</span><span class="sxs-lookup"><span data-stu-id="6af48-122">A note that admin can use to put some contextual information</span></span>|

## <a name="relationships"></a><span data-ttu-id="6af48-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6af48-123">Relationships</span></span>
<span data-ttu-id="6af48-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6af48-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6af48-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6af48-125">JSON Representation</span></span>
<span data-ttu-id="6af48-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6af48-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "note": "String"
}
```




