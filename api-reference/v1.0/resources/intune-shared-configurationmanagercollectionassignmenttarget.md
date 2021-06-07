---
title: tipo de recurso configurationManagerCollectionAssignmentTarget
description: Representa uma atribuição a uma coleção configuration manager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28aa1e4e7fbb0d65a74f9a7b84bc48df19f3201c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751743"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="3818e-103">tipo de recurso configurationManagerCollectionAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3818e-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="3818e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3818e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3818e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3818e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3818e-106">Representa uma atribuição a uma coleção configuration manager.</span><span class="sxs-lookup"><span data-stu-id="3818e-106">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="3818e-107">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3818e-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3818e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3818e-108">Properties</span></span>
|<span data-ttu-id="3818e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3818e-109">Property</span></span>|<span data-ttu-id="3818e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3818e-110">Type</span></span>|<span data-ttu-id="3818e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3818e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3818e-112">collectionId</span><span class="sxs-lookup"><span data-stu-id="3818e-112">collectionId</span></span>|<span data-ttu-id="3818e-113">String</span><span class="sxs-lookup"><span data-stu-id="3818e-113">String</span></span>|<span data-ttu-id="3818e-114">A ID da coleção que é o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3818e-114">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3818e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="3818e-115">Relationships</span></span>
<span data-ttu-id="3818e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3818e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3818e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3818e-117">JSON Representation</span></span>
<span data-ttu-id="3818e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3818e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "collectionId": "String"
}
```




