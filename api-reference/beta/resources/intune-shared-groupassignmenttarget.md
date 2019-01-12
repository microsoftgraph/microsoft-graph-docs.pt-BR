---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96aec1b72233cfe7d553b8f17feb9af382d89cde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971673"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="f66b6-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f66b6-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="f66b6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f66b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f66b6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f66b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f66b6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f66b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f66b6-107">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="f66b6-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="f66b6-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="f66b6-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f66b6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f66b6-109">Properties</span></span>
|<span data-ttu-id="f66b6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f66b6-110">Property</span></span>|<span data-ttu-id="f66b6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f66b6-111">Type</span></span>|<span data-ttu-id="f66b6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f66b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f66b6-113">groupId</span><span class="sxs-lookup"><span data-stu-id="f66b6-113">groupId</span></span>|<span data-ttu-id="f66b6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f66b6-114">String</span></span>|<span data-ttu-id="f66b6-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="f66b6-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f66b6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="f66b6-116">Relationships</span></span>
<span data-ttu-id="f66b6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f66b6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f66b6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f66b6-118">JSON Representation</span></span>
<span data-ttu-id="f66b6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f66b6-119">Here is a JSON representation of the resource.</span></span>
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





