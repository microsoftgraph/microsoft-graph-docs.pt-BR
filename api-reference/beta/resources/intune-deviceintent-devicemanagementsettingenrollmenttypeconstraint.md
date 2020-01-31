---
title: tipo de recurso deviceManagementSettingEnrollmentTypeConstraint
description: Restrição que impõe os tipos de inscrição aplicados a uma configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8959d245c17060a75e48195e30ff546c929ca7a
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636704"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="d573f-103">tipo de recurso deviceManagementSettingEnrollmentTypeConstraint</span><span class="sxs-lookup"><span data-stu-id="d573f-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

> <span data-ttu-id="d573f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d573f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d573f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d573f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d573f-106">Restrição que impõe os tipos de inscrição aplicados a uma configuração</span><span class="sxs-lookup"><span data-stu-id="d573f-106">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="d573f-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d573f-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d573f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d573f-108">Properties</span></span>
|<span data-ttu-id="d573f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d573f-109">Property</span></span>|<span data-ttu-id="d573f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d573f-110">Type</span></span>|<span data-ttu-id="d573f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d573f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d573f-112">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="d573f-112">enrollmentTypes</span></span>|<span data-ttu-id="d573f-113">String collection</span><span class="sxs-lookup"><span data-stu-id="d573f-113">String collection</span></span>|<span data-ttu-id="d573f-114">Lista de tipos de registro</span><span class="sxs-lookup"><span data-stu-id="d573f-114">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="d573f-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d573f-115">Relationships</span></span>
<span data-ttu-id="d573f-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d573f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d573f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d573f-117">JSON Representation</span></span>
<span data-ttu-id="d573f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d573f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



