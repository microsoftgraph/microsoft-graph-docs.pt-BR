---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ac3c4519cc074c3cce423ca5d0745c8a78d865
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571916"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="9c41b-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9c41b-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="9c41b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c41b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c41b-105">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="9c41b-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="9c41b-106">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9c41b-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c41b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c41b-107">Properties</span></span>
|<span data-ttu-id="9c41b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c41b-108">Property</span></span>|<span data-ttu-id="9c41b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c41b-109">Type</span></span>|<span data-ttu-id="9c41b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c41b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c41b-111">groupId</span><span class="sxs-lookup"><span data-stu-id="9c41b-111">groupId</span></span>|<span data-ttu-id="9c41b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c41b-112">String</span></span>|<span data-ttu-id="9c41b-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c41b-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c41b-114">Relações</span><span class="sxs-lookup"><span data-stu-id="9c41b-114">Relationships</span></span>
<span data-ttu-id="9c41b-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c41b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c41b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c41b-116">JSON Representation</span></span>
<span data-ttu-id="9c41b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c41b-117">Here is a JSON representation of the resource.</span></span>
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



