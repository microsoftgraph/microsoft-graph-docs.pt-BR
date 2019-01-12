---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e2928817a4d8bf287c3a941ddea80e7a3c4e19fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951716"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="cc7bf-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cc7bf-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="cc7bf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cc7bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc7bf-105">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="cc7bf-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="cc7bf-106">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="cc7bf-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc7bf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc7bf-107">Properties</span></span>
|<span data-ttu-id="cc7bf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc7bf-108">Property</span></span>|<span data-ttu-id="cc7bf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc7bf-109">Type</span></span>|<span data-ttu-id="cc7bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc7bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc7bf-111">groupId</span><span class="sxs-lookup"><span data-stu-id="cc7bf-111">groupId</span></span>|<span data-ttu-id="cc7bf-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc7bf-112">String</span></span>|<span data-ttu-id="cc7bf-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="cc7bf-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc7bf-114">Relações</span><span class="sxs-lookup"><span data-stu-id="cc7bf-114">Relationships</span></span>
<span data-ttu-id="cc7bf-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc7bf-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc7bf-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc7bf-116">JSON Representation</span></span>
<span data-ttu-id="cc7bf-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc7bf-117">Here is a JSON representation of the resource.</span></span>
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



