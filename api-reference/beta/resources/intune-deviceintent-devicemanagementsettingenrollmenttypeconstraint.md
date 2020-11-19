---
title: tipo de recurso deviceManagementSettingEnrollmentTypeConstraint
description: Restrição que impõe os tipos de inscrição aplicados a uma configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 604f9210cf81947617d40b0baec8fe8c5715347f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307448"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="0c9e6-103">tipo de recurso deviceManagementSettingEnrollmentTypeConstraint</span><span class="sxs-lookup"><span data-stu-id="0c9e6-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="0c9e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c9e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c9e6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c9e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c9e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c9e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c9e6-107">Restrição que impõe os tipos de inscrição aplicados a uma configuração</span><span class="sxs-lookup"><span data-stu-id="0c9e6-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="0c9e6-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0c9e6-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c9e6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c9e6-109">Properties</span></span>
|<span data-ttu-id="0c9e6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c9e6-110">Property</span></span>|<span data-ttu-id="0c9e6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c9e6-111">Type</span></span>|<span data-ttu-id="0c9e6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c9e6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c9e6-113">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="0c9e6-113">enrollmentTypes</span></span>|<span data-ttu-id="0c9e6-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c9e6-114">String collection</span></span>|<span data-ttu-id="0c9e6-115">Lista de tipos de registro</span><span class="sxs-lookup"><span data-stu-id="0c9e6-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c9e6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0c9e6-116">Relationships</span></span>
<span data-ttu-id="0c9e6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c9e6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c9e6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c9e6-118">JSON Representation</span></span>
<span data-ttu-id="0c9e6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c9e6-119">Here is a JSON representation of the resource.</span></span>
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




