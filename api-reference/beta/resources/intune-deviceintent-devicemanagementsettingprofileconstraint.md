---
title: tipo de recurso deviceManagementSettingProfileConstraint
description: Restrição que impõe um determinado perfil de metadados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2244b0fcafb1eb983388a220662c0ce7c874c73f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061158"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="dc132-103">tipo de recurso deviceManagementSettingProfileConstraint</span><span class="sxs-lookup"><span data-stu-id="dc132-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="dc132-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc132-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc132-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc132-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc132-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc132-107">Restrição que impõe um determinado perfil de metadados</span><span class="sxs-lookup"><span data-stu-id="dc132-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="dc132-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="dc132-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc132-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc132-109">Properties</span></span>
|<span data-ttu-id="dc132-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc132-110">Property</span></span>|<span data-ttu-id="dc132-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc132-111">Type</span></span>|<span data-ttu-id="dc132-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc132-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc132-113">source</span><span class="sxs-lookup"><span data-stu-id="dc132-113">source</span></span>|<span data-ttu-id="dc132-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc132-114">String</span></span>|<span data-ttu-id="dc132-115">A origem da entidade</span><span class="sxs-lookup"><span data-stu-id="dc132-115">The source of the entity</span></span>|
|<span data-ttu-id="dc132-116">tipos</span><span class="sxs-lookup"><span data-stu-id="dc132-116">types</span></span>|<span data-ttu-id="dc132-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc132-117">String collection</span></span>|<span data-ttu-id="dc132-118">Uma coleção de tipos que esta entidade transporta</span><span class="sxs-lookup"><span data-stu-id="dc132-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc132-119">Relações</span><span class="sxs-lookup"><span data-stu-id="dc132-119">Relationships</span></span>
<span data-ttu-id="dc132-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc132-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc132-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc132-121">JSON Representation</span></span>
<span data-ttu-id="dc132-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc132-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingProfileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingProfileConstraint",
  "source": "String",
  "types": [
    "String"
  ]
}
```






