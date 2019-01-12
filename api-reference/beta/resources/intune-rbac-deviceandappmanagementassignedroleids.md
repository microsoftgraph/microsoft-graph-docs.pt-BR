---
title: tipo de recurso de deviceAndAppManagementAssignedRoleIds
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2dbabca28f9ed8aa491d01f6eada5dc11b76867b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923373"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="ef5df-103">tipo de recurso de deviceAndAppManagementAssignedRoleIds</span><span class="sxs-lookup"><span data-stu-id="ef5df-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="ef5df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef5df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef5df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef5df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef5df-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef5df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef5df-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ef5df-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ef5df-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef5df-108">Properties</span></span>
|<span data-ttu-id="ef5df-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef5df-109">Property</span></span>|<span data-ttu-id="ef5df-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef5df-110">Type</span></span>|<span data-ttu-id="ef5df-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef5df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef5df-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="ef5df-112">roleDefinitionIds</span></span>|<span data-ttu-id="ef5df-113">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="ef5df-113">Guid collection</span></span>|<span data-ttu-id="ef5df-114">IDs de definição de função para o specifc definições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="ef5df-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="ef5df-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="ef5df-115">roleAssignmentIds</span></span>|<span data-ttu-id="ef5df-116">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="ef5df-116">Guid collection</span></span>|<span data-ttu-id="ef5df-117">IDs de atribuição de função para o specifc atribuições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="ef5df-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef5df-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ef5df-118">Relationships</span></span>
<span data-ttu-id="ef5df-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef5df-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef5df-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef5df-120">JSON Representation</span></span>
<span data-ttu-id="ef5df-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef5df-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





