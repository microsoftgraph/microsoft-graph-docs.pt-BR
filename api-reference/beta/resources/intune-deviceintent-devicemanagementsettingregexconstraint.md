---
title: tipo de recurso deviceManagementSettingRegexConstraint
description: Restrição que impõe a configuração corresponde a um determinado padrão de RegEx
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52369b5309768bd5530d176a7ccfbfabb1365b62
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522374"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="2be2f-103">tipo de recurso deviceManagementSettingRegexConstraint</span><span class="sxs-lookup"><span data-stu-id="2be2f-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="2be2f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2be2f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2be2f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2be2f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2be2f-106">Restrição que impõe a configuração corresponde a um determinado padrão de RegEx</span><span class="sxs-lookup"><span data-stu-id="2be2f-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="2be2f-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="2be2f-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2be2f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2be2f-108">Properties</span></span>
|<span data-ttu-id="2be2f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2be2f-109">Property</span></span>|<span data-ttu-id="2be2f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2be2f-110">Type</span></span>|<span data-ttu-id="2be2f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2be2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2be2f-112">Regex</span><span class="sxs-lookup"><span data-stu-id="2be2f-112">regex</span></span>|<span data-ttu-id="2be2f-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2be2f-113">String</span></span>|<span data-ttu-id="2be2f-114">O padrão RegEx a ser correspondido em relação</span><span class="sxs-lookup"><span data-stu-id="2be2f-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="2be2f-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2be2f-115">Relationships</span></span>
<span data-ttu-id="2be2f-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2be2f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2be2f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2be2f-117">JSON Representation</span></span>
<span data-ttu-id="2be2f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2be2f-118">Here is a JSON representation of the resource.</span></span>
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







