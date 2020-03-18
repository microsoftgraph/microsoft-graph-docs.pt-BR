---
title: tipo de recurso deviceManagementSettingEnrollmentTypeConstraint
description: Restrição que impõe os tipos de inscrição aplicados a uma configuração
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c5d34f381e7f4b52039551fb120e4691bc40026
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785327"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="9baf1-103">tipo de recurso deviceManagementSettingEnrollmentTypeConstraint</span><span class="sxs-lookup"><span data-stu-id="9baf1-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

> <span data-ttu-id="9baf1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9baf1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9baf1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9baf1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9baf1-106">Restrição que impõe os tipos de inscrição aplicados a uma configuração</span><span class="sxs-lookup"><span data-stu-id="9baf1-106">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="9baf1-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="9baf1-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9baf1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9baf1-108">Properties</span></span>
|<span data-ttu-id="9baf1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9baf1-109">Property</span></span>|<span data-ttu-id="9baf1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9baf1-110">Type</span></span>|<span data-ttu-id="9baf1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9baf1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9baf1-112">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="9baf1-112">enrollmentTypes</span></span>|<span data-ttu-id="9baf1-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9baf1-113">String collection</span></span>|<span data-ttu-id="9baf1-114">Lista de tipos de registro</span><span class="sxs-lookup"><span data-stu-id="9baf1-114">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="9baf1-115">Relações</span><span class="sxs-lookup"><span data-stu-id="9baf1-115">Relationships</span></span>
<span data-ttu-id="9baf1-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9baf1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9baf1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9baf1-117">JSON Representation</span></span>
<span data-ttu-id="9baf1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9baf1-118">Here is a JSON representation of the resource.</span></span>
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



