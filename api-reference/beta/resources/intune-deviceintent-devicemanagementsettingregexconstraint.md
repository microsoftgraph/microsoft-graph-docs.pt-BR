---
title: tipo de recurso deviceManagementSettingRegexConstraint
description: Restrição que impõe a configuração corresponde a um determinado padrão de RegEx
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0f9a04583bfb9b28546e9057f0530f72558a0be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364632"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="d2bb2-103">tipo de recurso deviceManagementSettingRegexConstraint</span><span class="sxs-lookup"><span data-stu-id="d2bb2-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="d2bb2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2bb2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2bb2-106">Restrição que impõe a configuração corresponde a um determinado padrão de RegEx</span><span class="sxs-lookup"><span data-stu-id="d2bb2-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="d2bb2-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d2bb2-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2bb2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2bb2-108">Properties</span></span>
|<span data-ttu-id="d2bb2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2bb2-109">Property</span></span>|<span data-ttu-id="d2bb2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bb2-110">Type</span></span>|<span data-ttu-id="d2bb2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2bb2-112">Regex</span><span class="sxs-lookup"><span data-stu-id="d2bb2-112">regex</span></span>|<span data-ttu-id="d2bb2-113">String</span><span class="sxs-lookup"><span data-stu-id="d2bb2-113">String</span></span>|<span data-ttu-id="d2bb2-114">O padrão RegEx a ser correspondido em relação</span><span class="sxs-lookup"><span data-stu-id="d2bb2-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2bb2-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d2bb2-115">Relationships</span></span>
<span data-ttu-id="d2bb2-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2bb2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2bb2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2bb2-117">JSON Representation</span></span>
<span data-ttu-id="d2bb2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-118">Here is a JSON representation of the resource.</span></span>
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



