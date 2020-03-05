---
title: Tipo de recurso exclusionGroupAssignmentTarget
description: Representa um grupo que deve ser excluído de uma atribuição.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08bf52ab16a29c869366373c5f205f25b352e1b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447840"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="a414b-103">Tipo de recurso exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a414b-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="a414b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a414b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a414b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a414b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a414b-106">Representa um grupo que deve ser excluído de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="a414b-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="a414b-107">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a414b-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a414b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a414b-108">Properties</span></span>
|<span data-ttu-id="a414b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a414b-109">Property</span></span>|<span data-ttu-id="a414b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a414b-110">Type</span></span>|<span data-ttu-id="a414b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a414b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a414b-112">groupId</span><span class="sxs-lookup"><span data-stu-id="a414b-112">groupId</span></span>|<span data-ttu-id="a414b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a414b-113">String</span></span>|<span data-ttu-id="a414b-114">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a414b-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="a414b-115">Herda de [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a414b-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a414b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a414b-116">Relationships</span></span>
<span data-ttu-id="a414b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a414b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a414b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a414b-118">JSON Representation</span></span>
<span data-ttu-id="a414b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a414b-119">Here is a JSON representation of the resource.</span></span>
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




