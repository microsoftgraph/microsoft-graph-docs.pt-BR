---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: tfitzmac
ms.openlocfilehash: 5371554d069237dc6bc017c29574423b415f4f33
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323132"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="3e8fe-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3e8fe-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="3e8fe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e8fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e8fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e8fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e8fe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e8fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e8fe-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="3e8fe-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="3e8fe-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3e8fe-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e8fe-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e8fe-109">Properties</span></span>
|<span data-ttu-id="3e8fe-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e8fe-110">Property</span></span>|<span data-ttu-id="3e8fe-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e8fe-111">Type</span></span>|<span data-ttu-id="3e8fe-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e8fe-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8fe-113">groupId</span><span class="sxs-lookup"><span data-stu-id="3e8fe-113">groupId</span></span>|<span data-ttu-id="3e8fe-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e8fe-114">String</span></span>|<span data-ttu-id="3e8fe-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3e8fe-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e8fe-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3e8fe-116">Relationships</span></span>
<span data-ttu-id="3e8fe-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e8fe-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e8fe-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e8fe-118">JSON Representation</span></span>
<span data-ttu-id="3e8fe-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e8fe-119">Here is a JSON representation of the resource.</span></span>
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





