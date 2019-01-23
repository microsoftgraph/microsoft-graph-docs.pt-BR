---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2039f5917aa5d69b74ccb6c1732496dc567ab673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399420"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="487dc-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="487dc-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="487dc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="487dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="487dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="487dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="487dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="487dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="487dc-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="487dc-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="487dc-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="487dc-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="487dc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="487dc-109">Properties</span></span>
|<span data-ttu-id="487dc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="487dc-110">Property</span></span>|<span data-ttu-id="487dc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="487dc-111">Type</span></span>|<span data-ttu-id="487dc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="487dc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="487dc-113">groupId</span><span class="sxs-lookup"><span data-stu-id="487dc-113">groupId</span></span>|<span data-ttu-id="487dc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="487dc-114">String</span></span>|<span data-ttu-id="487dc-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="487dc-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="487dc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="487dc-116">Relationships</span></span>
<span data-ttu-id="487dc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="487dc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="487dc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="487dc-118">JSON Representation</span></span>
<span data-ttu-id="487dc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="487dc-119">Here is a JSON representation of the resource.</span></span>
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




