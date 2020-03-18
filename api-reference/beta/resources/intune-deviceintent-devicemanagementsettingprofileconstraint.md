---
title: tipo de recurso deviceManagementSettingProfileConstraint
description: Restrição que impõe um determinado perfil de metadados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4b565321069c27949fbd5814c4ddc1c4eb1451b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785299"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="727cb-103">tipo de recurso deviceManagementSettingProfileConstraint</span><span class="sxs-lookup"><span data-stu-id="727cb-103">deviceManagementSettingProfileConstraint resource type</span></span>

> <span data-ttu-id="727cb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="727cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="727cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="727cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="727cb-106">Restrição que impõe um determinado perfil de metadados</span><span class="sxs-lookup"><span data-stu-id="727cb-106">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="727cb-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="727cb-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="727cb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="727cb-108">Properties</span></span>
|<span data-ttu-id="727cb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="727cb-109">Property</span></span>|<span data-ttu-id="727cb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="727cb-110">Type</span></span>|<span data-ttu-id="727cb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="727cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="727cb-112">source</span><span class="sxs-lookup"><span data-stu-id="727cb-112">source</span></span>|<span data-ttu-id="727cb-113">String</span><span class="sxs-lookup"><span data-stu-id="727cb-113">String</span></span>|<span data-ttu-id="727cb-114">A origem da entidade</span><span class="sxs-lookup"><span data-stu-id="727cb-114">The source of the entity</span></span>|
|<span data-ttu-id="727cb-115">tipos</span><span class="sxs-lookup"><span data-stu-id="727cb-115">types</span></span>|<span data-ttu-id="727cb-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="727cb-116">String collection</span></span>|<span data-ttu-id="727cb-117">Uma coleção de tipos que esta entidade transporta</span><span class="sxs-lookup"><span data-stu-id="727cb-117">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="727cb-118">Relações</span><span class="sxs-lookup"><span data-stu-id="727cb-118">Relationships</span></span>
<span data-ttu-id="727cb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="727cb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="727cb-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="727cb-120">JSON Representation</span></span>
<span data-ttu-id="727cb-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="727cb-121">Here is a JSON representation of the resource.</span></span>
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



