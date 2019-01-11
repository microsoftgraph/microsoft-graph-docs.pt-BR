---
title: tipo de recurso de deviceAndAppManagementAssignedRoleIds
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1ae87f1a8430ef2539fe10e813390b0fbd68b267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846337"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="e0ec1-103">tipo de recurso de deviceAndAppManagementAssignedRoleIds</span><span class="sxs-lookup"><span data-stu-id="e0ec1-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="e0ec1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e0ec1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0ec1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e0ec1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0ec1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e0ec1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0ec1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e0ec1-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e0ec1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0ec1-108">Properties</span></span>
|<span data-ttu-id="e0ec1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0ec1-109">Property</span></span>|<span data-ttu-id="e0ec1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0ec1-110">Type</span></span>|<span data-ttu-id="e0ec1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0ec1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0ec1-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="e0ec1-112">roleDefinitionIds</span></span>|<span data-ttu-id="e0ec1-113">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e0ec1-113">Guid collection</span></span>|<span data-ttu-id="e0ec1-114">IDs de definição de função para o specifc definições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0ec1-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="e0ec1-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="e0ec1-115">roleAssignmentIds</span></span>|<span data-ttu-id="e0ec1-116">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="e0ec1-116">Guid collection</span></span>|<span data-ttu-id="e0ec1-117">IDs de atribuição de função para o specifc atribuições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0ec1-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0ec1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e0ec1-118">Relationships</span></span>
<span data-ttu-id="e0ec1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0ec1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0ec1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0ec1-120">JSON Representation</span></span>
<span data-ttu-id="e0ec1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0ec1-121">Here is a JSON representation of the resource.</span></span>
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





