---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
ms.openlocfilehash: 76ea8c56b8022dc832335c575ad52632894f1d60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033842"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="03542-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="03542-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="03542-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="03542-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03542-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03542-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03542-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="03542-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03542-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="03542-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="03542-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="03542-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03542-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03542-109">Properties</span></span>
|<span data-ttu-id="03542-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03542-110">Property</span></span>|<span data-ttu-id="03542-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="03542-111">Type</span></span>|<span data-ttu-id="03542-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="03542-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03542-113">groupId</span><span class="sxs-lookup"><span data-stu-id="03542-113">groupId</span></span>|<span data-ttu-id="03542-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03542-114">String</span></span>|<span data-ttu-id="03542-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="03542-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03542-116">Relações</span><span class="sxs-lookup"><span data-stu-id="03542-116">Relationships</span></span>
<span data-ttu-id="03542-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03542-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03542-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03542-118">JSON Representation</span></span>
<span data-ttu-id="03542-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03542-119">Here is a JSON representation of the resource.</span></span>
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





