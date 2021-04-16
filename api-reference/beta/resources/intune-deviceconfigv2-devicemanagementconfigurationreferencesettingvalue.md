---
title: Tipo de recurso deviceManagementConfigurationReferenceSettingValue
description: Modelo para ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1dc92606270cf4c2febcee68905f0c8bd29ced13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868299"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a><span data-ttu-id="bb687-103">Tipo de recurso deviceManagementConfigurationReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="bb687-103">deviceManagementConfigurationReferenceSettingValue resource type</span></span>

<span data-ttu-id="bb687-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb687-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb687-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb687-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb687-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb687-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb687-107">Modelo para ReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="bb687-107">Model for ReferenceSettingValue</span></span>


<span data-ttu-id="bb687-108">Herda [de deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bb687-108">Inherits from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb687-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb687-109">Properties</span></span>
|<span data-ttu-id="bb687-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb687-110">Property</span></span>|<span data-ttu-id="bb687-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb687-111">Type</span></span>|<span data-ttu-id="bb687-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb687-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb687-113">valor</span><span class="sxs-lookup"><span data-stu-id="bb687-113">value</span></span>|<span data-ttu-id="bb687-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb687-114">String</span></span>|<span data-ttu-id="bb687-115">Valor da configuração da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="bb687-115">Value of the string setting.</span></span> <span data-ttu-id="bb687-116">Herdado [de deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bb687-116">Inherited from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>|
|<span data-ttu-id="bb687-117">observação</span><span class="sxs-lookup"><span data-stu-id="bb687-117">note</span></span>|<span data-ttu-id="bb687-118">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="bb687-118">String</span></span>|<span data-ttu-id="bb687-119">Uma observação que o administrador pode usar para colocar algumas informações contextuais</span><span class="sxs-lookup"><span data-stu-id="bb687-119">A note that admin can use to put some contextual information</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb687-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bb687-120">Relationships</span></span>
<span data-ttu-id="bb687-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb687-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb687-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb687-122">JSON Representation</span></span>
<span data-ttu-id="bb687-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb687-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "value": "String",
  "note": "String"
}
```




