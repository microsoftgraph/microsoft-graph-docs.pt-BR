---
title: tipo de recurso de deviceAndAppManagementAssignedRoleIds
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 034120b891812a43c6c1683f61e52f071dc89816
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353379"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="7ddb2-103">tipo de recurso de deviceAndAppManagementAssignedRoleIds</span><span class="sxs-lookup"><span data-stu-id="7ddb2-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="7ddb2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7ddb2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ddb2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7ddb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ddb2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7ddb2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ddb2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7ddb2-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7ddb2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ddb2-108">Properties</span></span>
|<span data-ttu-id="7ddb2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ddb2-109">Property</span></span>|<span data-ttu-id="7ddb2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ddb2-110">Type</span></span>|<span data-ttu-id="7ddb2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ddb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ddb2-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="7ddb2-112">roleDefinitionIds</span></span>|<span data-ttu-id="7ddb2-113">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="7ddb2-113">Guid collection</span></span>|<span data-ttu-id="7ddb2-114">IDs de definição de função para o specifc definições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ddb2-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="7ddb2-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="7ddb2-115">roleAssignmentIds</span></span>|<span data-ttu-id="7ddb2-116">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="7ddb2-116">Guid collection</span></span>|<span data-ttu-id="7ddb2-117">IDs de atribuição de função para o specifc atribuições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="7ddb2-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ddb2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7ddb2-118">Relationships</span></span>
<span data-ttu-id="7ddb2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ddb2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ddb2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ddb2-120">JSON Representation</span></span>
<span data-ttu-id="7ddb2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ddb2-121">Here is a JSON representation of the resource.</span></span>
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





