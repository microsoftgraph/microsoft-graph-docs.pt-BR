---
title: tipo de recurso deviceManagementSettingRegexConstraint
description: Restrição que impõe a configuração corresponde a um determinado padrão de RegEx
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11d06b2af4273166b3d6cf93a36a76fecc7ec548
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267926"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="065c1-103">tipo de recurso deviceManagementSettingRegexConstraint</span><span class="sxs-lookup"><span data-stu-id="065c1-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="065c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="065c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="065c1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="065c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="065c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="065c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="065c1-107">Restrição que impõe a configuração corresponde a um determinado padrão de RegEx</span><span class="sxs-lookup"><span data-stu-id="065c1-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="065c1-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="065c1-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="065c1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="065c1-109">Properties</span></span>
|<span data-ttu-id="065c1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="065c1-110">Property</span></span>|<span data-ttu-id="065c1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="065c1-111">Type</span></span>|<span data-ttu-id="065c1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="065c1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="065c1-113">Regex</span><span class="sxs-lookup"><span data-stu-id="065c1-113">regex</span></span>|<span data-ttu-id="065c1-114">String</span><span class="sxs-lookup"><span data-stu-id="065c1-114">String</span></span>|<span data-ttu-id="065c1-115">O padrão RegEx a ser correspondido em relação</span><span class="sxs-lookup"><span data-stu-id="065c1-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="065c1-116">Relações</span><span class="sxs-lookup"><span data-stu-id="065c1-116">Relationships</span></span>
<span data-ttu-id="065c1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="065c1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="065c1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="065c1-118">JSON Representation</span></span>
<span data-ttu-id="065c1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="065c1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```




