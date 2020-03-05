---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b15df3fab9303f56e697eb09305db50d3ddea8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523671"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="f4172-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f4172-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="f4172-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4172-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4172-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4172-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4172-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4172-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4172-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="f4172-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="f4172-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="f4172-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4172-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4172-109">Properties</span></span>
|<span data-ttu-id="f4172-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4172-110">Property</span></span>|<span data-ttu-id="f4172-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4172-111">Type</span></span>|<span data-ttu-id="f4172-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4172-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4172-113">groupId</span><span class="sxs-lookup"><span data-stu-id="f4172-113">groupId</span></span>|<span data-ttu-id="f4172-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4172-114">String</span></span>|<span data-ttu-id="f4172-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="f4172-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4172-116">Relações</span><span class="sxs-lookup"><span data-stu-id="f4172-116">Relationships</span></span>
<span data-ttu-id="f4172-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4172-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4172-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4172-118">JSON Representation</span></span>
<span data-ttu-id="f4172-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4172-119">Here is a JSON representation of the resource.</span></span>
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



