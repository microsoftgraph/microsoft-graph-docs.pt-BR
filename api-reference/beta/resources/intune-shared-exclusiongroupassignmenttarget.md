---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: tfitzmac
ms.openlocfilehash: 783231c451668169ba85e8ce1cfecd669b5c0b7d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343180"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="7d03c-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7d03c-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="7d03c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d03c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d03c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d03c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d03c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d03c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d03c-107">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="7d03c-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="7d03c-108">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7d03c-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d03c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d03c-109">Properties</span></span>
|<span data-ttu-id="7d03c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d03c-110">Property</span></span>|<span data-ttu-id="7d03c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d03c-111">Type</span></span>|<span data-ttu-id="7d03c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d03c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d03c-113">groupId</span><span class="sxs-lookup"><span data-stu-id="7d03c-113">groupId</span></span>|<span data-ttu-id="7d03c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d03c-114">String</span></span>|<span data-ttu-id="7d03c-115">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7d03c-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="7d03c-116">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7d03c-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d03c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="7d03c-117">Relationships</span></span>
<span data-ttu-id="7d03c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d03c-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d03c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d03c-119">JSON Representation</span></span>
<span data-ttu-id="7d03c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d03c-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```





