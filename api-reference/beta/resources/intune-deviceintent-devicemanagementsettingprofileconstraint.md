---
title: tipo de recurso deviceManagementSettingProfileConstraint
description: Restrição que impõe um determinado perfil de metadados
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdd9e308f332d446ad9032736e5f08e8e3545d9e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955684"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="3635d-103">tipo de recurso deviceManagementSettingProfileConstraint</span><span class="sxs-lookup"><span data-stu-id="3635d-103">deviceManagementSettingProfileConstraint resource type</span></span>

> <span data-ttu-id="3635d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3635d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3635d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3635d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3635d-106">Restrição que impõe um determinado perfil de metadados</span><span class="sxs-lookup"><span data-stu-id="3635d-106">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="3635d-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3635d-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3635d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3635d-108">Properties</span></span>
|<span data-ttu-id="3635d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3635d-109">Property</span></span>|<span data-ttu-id="3635d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3635d-110">Type</span></span>|<span data-ttu-id="3635d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3635d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3635d-112">source</span><span class="sxs-lookup"><span data-stu-id="3635d-112">source</span></span>|<span data-ttu-id="3635d-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3635d-113">String</span></span>|<span data-ttu-id="3635d-114">A origem da entidade</span><span class="sxs-lookup"><span data-stu-id="3635d-114">The source of the entity</span></span>|
|<span data-ttu-id="3635d-115">tipos</span><span class="sxs-lookup"><span data-stu-id="3635d-115">types</span></span>|<span data-ttu-id="3635d-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3635d-116">String collection</span></span>|<span data-ttu-id="3635d-117">Uma coleção de tipos que esta entidade transporta</span><span class="sxs-lookup"><span data-stu-id="3635d-117">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="3635d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3635d-118">Relationships</span></span>
<span data-ttu-id="3635d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3635d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3635d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3635d-120">JSON Representation</span></span>
<span data-ttu-id="3635d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3635d-121">Here is a JSON representation of the resource.</span></span>
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



