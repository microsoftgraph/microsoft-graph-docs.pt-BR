---
title: tipo de recurso deviceManagementSettingProfileConstraint
description: Restrição que impõe um determinado perfil de metadados
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb6784fa929aa298579cc889b39cfa90b475a014
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525226"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="144b4-103">tipo de recurso deviceManagementSettingProfileConstraint</span><span class="sxs-lookup"><span data-stu-id="144b4-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="144b4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="144b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="144b4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="144b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="144b4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="144b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="144b4-107">Restrição que impõe um determinado perfil de metadados</span><span class="sxs-lookup"><span data-stu-id="144b4-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="144b4-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="144b4-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="144b4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="144b4-109">Properties</span></span>
|<span data-ttu-id="144b4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="144b4-110">Property</span></span>|<span data-ttu-id="144b4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="144b4-111">Type</span></span>|<span data-ttu-id="144b4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="144b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="144b4-113">source</span><span class="sxs-lookup"><span data-stu-id="144b4-113">source</span></span>|<span data-ttu-id="144b4-114">String</span><span class="sxs-lookup"><span data-stu-id="144b4-114">String</span></span>|<span data-ttu-id="144b4-115">A origem da entidade</span><span class="sxs-lookup"><span data-stu-id="144b4-115">The source of the entity</span></span>|
|<span data-ttu-id="144b4-116">tipos</span><span class="sxs-lookup"><span data-stu-id="144b4-116">types</span></span>|<span data-ttu-id="144b4-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="144b4-117">String collection</span></span>|<span data-ttu-id="144b4-118">Uma coleção de tipos que esta entidade transporta</span><span class="sxs-lookup"><span data-stu-id="144b4-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="144b4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="144b4-119">Relationships</span></span>
<span data-ttu-id="144b4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="144b4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="144b4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="144b4-121">JSON Representation</span></span>
<span data-ttu-id="144b4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="144b4-122">Here is a JSON representation of the resource.</span></span>
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



