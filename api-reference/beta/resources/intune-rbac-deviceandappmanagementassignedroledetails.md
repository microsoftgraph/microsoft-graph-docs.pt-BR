---
title: tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de definições de função e atribuições de função atribuídas a um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a9aaa700b2c06f12dc9451adf697a983fd60225
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696073"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="2c33d-103">tipo de recurso deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="2c33d-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="2c33d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c33d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c33d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c33d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c33d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c33d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c33d-107">O conjunto de definições de função e atribuições de função atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="2c33d-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="2c33d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c33d-108">Properties</span></span>
|<span data-ttu-id="2c33d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c33d-109">Property</span></span>|<span data-ttu-id="2c33d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c33d-110">Type</span></span>|<span data-ttu-id="2c33d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c33d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c33d-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="2c33d-112">roleDefinitionIds</span></span>|<span data-ttu-id="2c33d-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c33d-113">String collection</span></span>|<span data-ttu-id="2c33d-114">IDs de definição de função para as definições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="2c33d-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="2c33d-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="2c33d-115">roleAssignmentIds</span></span>|<span data-ttu-id="2c33d-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c33d-116">String collection</span></span>|<span data-ttu-id="2c33d-117">IDs de atribuição de função para as atribuições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="2c33d-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c33d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2c33d-118">Relationships</span></span>
<span data-ttu-id="2c33d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c33d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c33d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c33d-120">JSON Representation</span></span>
<span data-ttu-id="2c33d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c33d-121">Here is a JSON representation of the resource.</span></span>
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





