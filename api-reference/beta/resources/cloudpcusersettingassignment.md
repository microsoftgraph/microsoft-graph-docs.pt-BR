---
title: Tipo de recurso cloudPcUserSettingAssignment
description: Representa uma coleção definida de atribuições de configuração do usuário.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db97ff52ff8eb7ca1ef52563d577d5076273d859
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082178"
---
# <a name="cloudpcusersettingassignment--resource-type"></a><span data-ttu-id="d9b86-103">Tipo de recurso cloudPcUserSettingAssignment</span><span class="sxs-lookup"><span data-stu-id="d9b86-103">cloudPcUserSettingAssignment  resource type</span></span>

<span data-ttu-id="d9b86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9b86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9b86-105">Representa uma coleção definida de atribuições de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b86-105">Represents a defined collection of user setting assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="d9b86-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9b86-106">Properties</span></span>

|<span data-ttu-id="d9b86-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9b86-107">Property</span></span>|<span data-ttu-id="d9b86-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b86-108">Type</span></span>|<span data-ttu-id="d9b86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9b86-110">id</span><span class="sxs-lookup"><span data-stu-id="d9b86-110">id</span></span>|<span data-ttu-id="d9b86-111">String</span><span class="sxs-lookup"><span data-stu-id="d9b86-111">String</span></span>|<span data-ttu-id="d9b86-112">Identificador exclusivo da atribuição de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b86-112">Unique Identifier for the user setting assignment.</span></span> <span data-ttu-id="d9b86-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b86-113">Read-only.</span></span> <span data-ttu-id="d9b86-114">Se `target` for um grupo de usuários, a ID terá essa estrutura: {policyID} \_ {groupID}.</span><span class="sxs-lookup"><span data-stu-id="d9b86-114">If `target` is a user group, the ID has this structure: {policyID}\_{groupID}.</span></span>|
|<span data-ttu-id="d9b86-115">destino</span><span class="sxs-lookup"><span data-stu-id="d9b86-115">target</span></span>|[<span data-ttu-id="d9b86-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9b86-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="d9b86-117">O destino de atribuição para a configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b86-117">The assignment target for the user setting.</span></span> <span data-ttu-id="d9b86-118">Atualmente, o único destino com suporte para essa configuração de usuário é um grupo de usuários.</span><span class="sxs-lookup"><span data-stu-id="d9b86-118">Currently, the only target supported for this user setting is a user group.</span></span> <span data-ttu-id="d9b86-119">Para obter detalhes, [consulte cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="d9b86-119">For details, see [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span></span>|
|<span data-ttu-id="d9b86-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9b86-120">createdDateTime</span></span>|<span data-ttu-id="d9b86-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9b86-121">DateTimeOffset</span></span>|<span data-ttu-id="d9b86-122">A data e a hora em que essa atribuição foi criada.</span><span class="sxs-lookup"><span data-stu-id="d9b86-122">The date and time this assignment was created.</span></span> <span data-ttu-id="d9b86-123">O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d9b86-123">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d9b86-124">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="d9b86-124">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d9b86-125">Relações</span><span class="sxs-lookup"><span data-stu-id="d9b86-125">Relationships</span></span>

<span data-ttu-id="d9b86-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9b86-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9b86-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9b86-127">JSON representation</span></span>
<span data-ttu-id="d9b86-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9b86-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
