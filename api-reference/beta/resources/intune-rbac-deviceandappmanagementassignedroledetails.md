---
title: tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de definições de função e atribuições de função atribuídas a um usuário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1590470f436dac6572ebf9d0430d144060f9b7f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773942"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="37570-103">tipo de recurso deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="37570-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="37570-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37570-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37570-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37570-106">O conjunto de definições de função e atribuições de função atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="37570-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="37570-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37570-107">Properties</span></span>
|<span data-ttu-id="37570-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37570-108">Property</span></span>|<span data-ttu-id="37570-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37570-109">Type</span></span>|<span data-ttu-id="37570-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37570-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37570-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="37570-111">roleDefinitionIds</span></span>|<span data-ttu-id="37570-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37570-112">String collection</span></span>|<span data-ttu-id="37570-113">IDs de definição de função para as definições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="37570-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="37570-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="37570-114">roleAssignmentIds</span></span>|<span data-ttu-id="37570-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37570-115">String collection</span></span>|<span data-ttu-id="37570-116">IDs de atribuição de função para as atribuições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="37570-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37570-117">Relações</span><span class="sxs-lookup"><span data-stu-id="37570-117">Relationships</span></span>
<span data-ttu-id="37570-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37570-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37570-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37570-119">JSON Representation</span></span>
<span data-ttu-id="37570-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37570-120">Here is a JSON representation of the resource.</span></span>
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



