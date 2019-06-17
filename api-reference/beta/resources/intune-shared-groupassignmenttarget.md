---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b050a25f7770870a7cd756c78ed448312a41f51
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996075"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="ab04e-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ab04e-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="ab04e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab04e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab04e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab04e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab04e-106">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="ab04e-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="ab04e-107">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ab04e-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ab04e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab04e-108">Properties</span></span>
|<span data-ttu-id="ab04e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab04e-109">Property</span></span>|<span data-ttu-id="ab04e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab04e-110">Type</span></span>|<span data-ttu-id="ab04e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab04e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab04e-112">groupId</span><span class="sxs-lookup"><span data-stu-id="ab04e-112">groupId</span></span>|<span data-ttu-id="ab04e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab04e-113">String</span></span>|<span data-ttu-id="ab04e-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ab04e-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab04e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="ab04e-115">Relationships</span></span>
<span data-ttu-id="ab04e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab04e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab04e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab04e-117">JSON Representation</span></span>
<span data-ttu-id="ab04e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab04e-118">Here is a JSON representation of the resource.</span></span>
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





