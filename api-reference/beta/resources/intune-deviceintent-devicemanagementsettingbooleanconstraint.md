---
title: tipo de recurso deviceManagementSettingBooleanConstraint
description: Restrição o impõe um valor booliano específico
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c39fbb19439572b1e698b3c5db3bcf0bf6c8ea5
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523690"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="e9e55-103">tipo de recurso deviceManagementSettingBooleanConstraint</span><span class="sxs-lookup"><span data-stu-id="e9e55-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="e9e55-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9e55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9e55-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9e55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9e55-106">Restrição o impõe um valor booliano específico</span><span class="sxs-lookup"><span data-stu-id="e9e55-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="e9e55-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e9e55-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9e55-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9e55-108">Properties</span></span>
|<span data-ttu-id="e9e55-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9e55-109">Property</span></span>|<span data-ttu-id="e9e55-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9e55-110">Type</span></span>|<span data-ttu-id="e9e55-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9e55-112">value</span><span class="sxs-lookup"><span data-stu-id="e9e55-112">value</span></span>|<span data-ttu-id="e9e55-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9e55-113">Boolean</span></span>|<span data-ttu-id="e9e55-114">O valor booliano a ser comparado</span><span class="sxs-lookup"><span data-stu-id="e9e55-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9e55-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e9e55-115">Relationships</span></span>
<span data-ttu-id="e9e55-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e9e55-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9e55-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9e55-117">JSON Representation</span></span>
<span data-ttu-id="e9e55-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9e55-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```







