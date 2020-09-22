---
title: tipo de recurso deviceManagementSettingAbstractImplementationConstraint
description: A restrição que impõe um tipo de AbstractComplex tem ou está definida para um valor específico
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62b257e7d6199798d2a4f13a3210e98d53b82de6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061312"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a><span data-ttu-id="e51f0-103">tipo de recurso deviceManagementSettingAbstractImplementationConstraint</span><span class="sxs-lookup"><span data-stu-id="e51f0-103">deviceManagementSettingAbstractImplementationConstraint resource type</span></span>

<span data-ttu-id="e51f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e51f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e51f0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e51f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e51f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e51f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e51f0-107">A restrição que impõe um tipo de AbstractComplex tem ou está definida para um valor específico</span><span class="sxs-lookup"><span data-stu-id="e51f0-107">Constraint that enforces an AbstractComplex type has or is set to a particular value</span></span>


<span data-ttu-id="e51f0-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e51f0-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e51f0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e51f0-109">Properties</span></span>
|<span data-ttu-id="e51f0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e51f0-110">Property</span></span>|<span data-ttu-id="e51f0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e51f0-111">Type</span></span>|<span data-ttu-id="e51f0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e51f0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e51f0-113">allowedAbstractImplementationDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="e51f0-113">allowedAbstractImplementationDefinitionIds</span></span>|<span data-ttu-id="e51f0-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e51f0-114">String collection</span></span>|<span data-ttu-id="e51f0-115">Lista de valores que significa não configurado para a configuração</span><span class="sxs-lookup"><span data-stu-id="e51f0-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="e51f0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e51f0-116">Relationships</span></span>
<span data-ttu-id="e51f0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e51f0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e51f0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e51f0-118">JSON Representation</span></span>
<span data-ttu-id="e51f0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e51f0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAbstractImplementationConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAbstractImplementationConstraint",
  "allowedAbstractImplementationDefinitionIds": [
    "String"
  ]
}
```






