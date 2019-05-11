---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e30bde3c36346fe1938b245174f971bddddebe20
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938622"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="65d4b-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="65d4b-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="65d4b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65d4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65d4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65d4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65d4b-106">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="65d4b-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="65d4b-107">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="65d4b-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65d4b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65d4b-108">Properties</span></span>
|<span data-ttu-id="65d4b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65d4b-109">Property</span></span>|<span data-ttu-id="65d4b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65d4b-110">Type</span></span>|<span data-ttu-id="65d4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65d4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65d4b-112">groupId</span><span class="sxs-lookup"><span data-stu-id="65d4b-112">groupId</span></span>|<span data-ttu-id="65d4b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65d4b-113">String</span></span>|<span data-ttu-id="65d4b-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="65d4b-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65d4b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="65d4b-115">Relationships</span></span>
<span data-ttu-id="65d4b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65d4b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65d4b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65d4b-117">JSON Representation</span></span>
<span data-ttu-id="65d4b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65d4b-118">Here is a JSON representation of the resource.</span></span>
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




