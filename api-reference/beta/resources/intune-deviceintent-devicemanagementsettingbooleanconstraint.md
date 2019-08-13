---
title: tipo de recurso deviceManagementSettingBooleanConstraint
description: Restrição o impõe um valor booliano específico
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a83a0747e0960aeebaa0de472fae4d587111946
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364723"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="3505c-103">tipo de recurso deviceManagementSettingBooleanConstraint</span><span class="sxs-lookup"><span data-stu-id="3505c-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="3505c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3505c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3505c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3505c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3505c-106">Restrição o impõe um valor booliano específico</span><span class="sxs-lookup"><span data-stu-id="3505c-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="3505c-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3505c-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3505c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3505c-108">Properties</span></span>
|<span data-ttu-id="3505c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3505c-109">Property</span></span>|<span data-ttu-id="3505c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3505c-110">Type</span></span>|<span data-ttu-id="3505c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3505c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3505c-112">valor</span><span class="sxs-lookup"><span data-stu-id="3505c-112">value</span></span>|<span data-ttu-id="3505c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="3505c-113">Boolean</span></span>|<span data-ttu-id="3505c-114">O valor booliano a ser comparado</span><span class="sxs-lookup"><span data-stu-id="3505c-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="3505c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="3505c-115">Relationships</span></span>
<span data-ttu-id="3505c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3505c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3505c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3505c-117">JSON Representation</span></span>
<span data-ttu-id="3505c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3505c-118">Here is a JSON representation of the resource.</span></span>
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



