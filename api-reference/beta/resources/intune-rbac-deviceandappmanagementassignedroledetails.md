---
title: tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de definições de função e atribuições de função atribuídas a um usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771401"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="174c8-103">tipo de recurso deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="174c8-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="174c8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="174c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="174c8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="174c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="174c8-106">O conjunto de definições de função e atribuições de função atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="174c8-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="174c8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="174c8-107">Properties</span></span>
|<span data-ttu-id="174c8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="174c8-108">Property</span></span>|<span data-ttu-id="174c8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="174c8-109">Type</span></span>|<span data-ttu-id="174c8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="174c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="174c8-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="174c8-111">roleDefinitionIds</span></span>|<span data-ttu-id="174c8-112">Coleção String</span><span class="sxs-lookup"><span data-stu-id="174c8-112">String collection</span></span>|<span data-ttu-id="174c8-113">IDs de definição de função para as definições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="174c8-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="174c8-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="174c8-114">roleAssignmentIds</span></span>|<span data-ttu-id="174c8-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="174c8-115">String collection</span></span>|<span data-ttu-id="174c8-116">IDs de atribuição de função para as atribuições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="174c8-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="174c8-117">Relações</span><span class="sxs-lookup"><span data-stu-id="174c8-117">Relationships</span></span>
<span data-ttu-id="174c8-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="174c8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="174c8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="174c8-119">JSON Representation</span></span>
<span data-ttu-id="174c8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="174c8-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```





