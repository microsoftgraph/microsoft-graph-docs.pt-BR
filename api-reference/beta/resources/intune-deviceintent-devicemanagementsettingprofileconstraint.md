---
title: tipo de recurso deviceManagementSettingProfileConstraint
description: Restrição que impõe um determinado perfil de metadados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4edff7e73ff73970baa6d168655b94e189ccc40e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730443"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="3d022-103">tipo de recurso deviceManagementSettingProfileConstraint</span><span class="sxs-lookup"><span data-stu-id="3d022-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="3d022-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d022-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d022-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d022-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d022-107">Restrição que impõe um determinado perfil de metadados</span><span class="sxs-lookup"><span data-stu-id="3d022-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="3d022-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3d022-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d022-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d022-109">Properties</span></span>
|<span data-ttu-id="3d022-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d022-110">Property</span></span>|<span data-ttu-id="3d022-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d022-111">Type</span></span>|<span data-ttu-id="3d022-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d022-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d022-113">source</span><span class="sxs-lookup"><span data-stu-id="3d022-113">source</span></span>|<span data-ttu-id="3d022-114">String</span><span class="sxs-lookup"><span data-stu-id="3d022-114">String</span></span>|<span data-ttu-id="3d022-115">A origem da entidade</span><span class="sxs-lookup"><span data-stu-id="3d022-115">The source of the entity</span></span>|
|<span data-ttu-id="3d022-116">tipos</span><span class="sxs-lookup"><span data-stu-id="3d022-116">types</span></span>|<span data-ttu-id="3d022-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d022-117">String collection</span></span>|<span data-ttu-id="3d022-118">Uma coleção de tipos que esta entidade transporta</span><span class="sxs-lookup"><span data-stu-id="3d022-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d022-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3d022-119">Relationships</span></span>
<span data-ttu-id="3d022-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d022-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d022-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d022-121">JSON Representation</span></span>
<span data-ttu-id="3d022-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d022-122">Here is a JSON representation of the resource.</span></span>
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





