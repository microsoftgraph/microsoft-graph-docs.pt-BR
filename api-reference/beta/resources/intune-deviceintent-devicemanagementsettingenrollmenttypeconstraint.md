---
title: tipo de recurso deviceManagementSettingEnrollmentTypeConstraint
description: Restrição que impõe os tipos de inscrição aplicados a uma configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bb3f19b62bc8e289a5312f39f45bb15f2f5ab46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061193"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="1ce1f-103">tipo de recurso deviceManagementSettingEnrollmentTypeConstraint</span><span class="sxs-lookup"><span data-stu-id="1ce1f-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="1ce1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ce1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ce1f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ce1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ce1f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ce1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce1f-107">Restrição que impõe os tipos de inscrição aplicados a uma configuração</span><span class="sxs-lookup"><span data-stu-id="1ce1f-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="1ce1f-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="1ce1f-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ce1f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ce1f-109">Properties</span></span>
|<span data-ttu-id="1ce1f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ce1f-110">Property</span></span>|<span data-ttu-id="1ce1f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ce1f-111">Type</span></span>|<span data-ttu-id="1ce1f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ce1f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce1f-113">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="1ce1f-113">enrollmentTypes</span></span>|<span data-ttu-id="1ce1f-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ce1f-114">String collection</span></span>|<span data-ttu-id="1ce1f-115">Lista de tipos de registro</span><span class="sxs-lookup"><span data-stu-id="1ce1f-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ce1f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1ce1f-116">Relationships</span></span>
<span data-ttu-id="1ce1f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ce1f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ce1f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ce1f-118">JSON Representation</span></span>
<span data-ttu-id="1ce1f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ce1f-119">Here is a JSON representation of the resource.</span></span>
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






