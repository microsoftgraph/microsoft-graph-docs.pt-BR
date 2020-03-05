---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f103315cc0c0499545a7fe3adb8bc31f9d24880
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447833"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="8652e-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8652e-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="8652e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8652e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8652e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8652e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8652e-106">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="8652e-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="8652e-107">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="8652e-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8652e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8652e-108">Properties</span></span>
|<span data-ttu-id="8652e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8652e-109">Property</span></span>|<span data-ttu-id="8652e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8652e-110">Type</span></span>|<span data-ttu-id="8652e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8652e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8652e-112">groupId</span><span class="sxs-lookup"><span data-stu-id="8652e-112">groupId</span></span>|<span data-ttu-id="8652e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8652e-113">String</span></span>|<span data-ttu-id="8652e-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="8652e-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8652e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="8652e-115">Relationships</span></span>
<span data-ttu-id="8652e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8652e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8652e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8652e-117">JSON Representation</span></span>
<span data-ttu-id="8652e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8652e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```




