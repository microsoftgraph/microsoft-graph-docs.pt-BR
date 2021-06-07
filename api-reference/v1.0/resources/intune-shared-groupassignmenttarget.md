---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d90440ee70ad701b3bb19f159cda53a1355fc7f0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756761"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2ab90-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2ab90-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="2ab90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ab90-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ab90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab90-106">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="2ab90-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="2ab90-107">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2ab90-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ab90-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ab90-108">Properties</span></span>
|<span data-ttu-id="2ab90-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ab90-109">Property</span></span>|<span data-ttu-id="2ab90-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ab90-110">Type</span></span>|<span data-ttu-id="2ab90-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ab90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab90-112">groupId</span><span class="sxs-lookup"><span data-stu-id="2ab90-112">groupId</span></span>|<span data-ttu-id="2ab90-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ab90-113">String</span></span>|<span data-ttu-id="2ab90-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="2ab90-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab90-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2ab90-115">Relationships</span></span>
<span data-ttu-id="2ab90-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2ab90-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ab90-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ab90-117">JSON Representation</span></span>
<span data-ttu-id="2ab90-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ab90-118">Here is a JSON representation of the resource.</span></span>
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




