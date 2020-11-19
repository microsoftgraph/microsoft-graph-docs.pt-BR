---
title: tipo de recurso deviceManagementSettingProfileConstraint
description: Restrição que impõe um determinado perfil de metadados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 917483556c71853856ff8b70973167b2c749a3a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267961"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="3f697-103">tipo de recurso deviceManagementSettingProfileConstraint</span><span class="sxs-lookup"><span data-stu-id="3f697-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="3f697-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f697-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f697-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f697-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f697-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f697-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f697-107">Restrição que impõe um determinado perfil de metadados</span><span class="sxs-lookup"><span data-stu-id="3f697-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="3f697-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3f697-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f697-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f697-109">Properties</span></span>
|<span data-ttu-id="3f697-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f697-110">Property</span></span>|<span data-ttu-id="3f697-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f697-111">Type</span></span>|<span data-ttu-id="3f697-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f697-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f697-113">source</span><span class="sxs-lookup"><span data-stu-id="3f697-113">source</span></span>|<span data-ttu-id="3f697-114">String</span><span class="sxs-lookup"><span data-stu-id="3f697-114">String</span></span>|<span data-ttu-id="3f697-115">A origem da entidade</span><span class="sxs-lookup"><span data-stu-id="3f697-115">The source of the entity</span></span>|
|<span data-ttu-id="3f697-116">tipos</span><span class="sxs-lookup"><span data-stu-id="3f697-116">types</span></span>|<span data-ttu-id="3f697-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f697-117">String collection</span></span>|<span data-ttu-id="3f697-118">Uma coleção de tipos que esta entidade transporta</span><span class="sxs-lookup"><span data-stu-id="3f697-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f697-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3f697-119">Relationships</span></span>
<span data-ttu-id="3f697-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f697-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f697-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f697-121">JSON Representation</span></span>
<span data-ttu-id="3f697-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f697-122">Here is a JSON representation of the resource.</span></span>
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




