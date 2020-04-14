---
title: tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de definições de função e atribuições de função atribuídas a um usuário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 061929eadd3b636ab8fcc4d89a45489bacfa9aae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467693"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="8a06e-103">tipo de recurso deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="8a06e-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="8a06e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a06e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a06e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a06e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a06e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a06e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a06e-107">O conjunto de definições de função e atribuições de função atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a06e-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="8a06e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a06e-108">Properties</span></span>
|<span data-ttu-id="8a06e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a06e-109">Property</span></span>|<span data-ttu-id="8a06e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a06e-110">Type</span></span>|<span data-ttu-id="8a06e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a06e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a06e-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="8a06e-112">roleDefinitionIds</span></span>|<span data-ttu-id="8a06e-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a06e-113">String collection</span></span>|<span data-ttu-id="8a06e-114">IDs de definição de função para as definições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a06e-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="8a06e-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="8a06e-115">roleAssignmentIds</span></span>|<span data-ttu-id="8a06e-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a06e-116">String collection</span></span>|<span data-ttu-id="8a06e-117">IDs de atribuição de função para as atribuições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a06e-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a06e-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8a06e-118">Relationships</span></span>
<span data-ttu-id="8a06e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a06e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a06e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a06e-120">JSON Representation</span></span>
<span data-ttu-id="8a06e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a06e-121">Here is a JSON representation of the resource.</span></span>
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



