---
title: tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de definições de função e atribuições de função atribuídas a um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9dff637f950d980b3fc0de89ecfde26da6b40de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070797"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="84ab5-103">tipo de recurso deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="84ab5-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="84ab5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ab5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ab5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84ab5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ab5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84ab5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ab5-107">O conjunto de definições de função e atribuições de função atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="84ab5-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="84ab5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84ab5-108">Properties</span></span>
|<span data-ttu-id="84ab5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84ab5-109">Property</span></span>|<span data-ttu-id="84ab5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="84ab5-110">Type</span></span>|<span data-ttu-id="84ab5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ab5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ab5-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="84ab5-112">roleDefinitionIds</span></span>|<span data-ttu-id="84ab5-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84ab5-113">String collection</span></span>|<span data-ttu-id="84ab5-114">IDs de definição de função para as definições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="84ab5-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="84ab5-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="84ab5-115">roleAssignmentIds</span></span>|<span data-ttu-id="84ab5-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="84ab5-116">String collection</span></span>|<span data-ttu-id="84ab5-117">IDs de atribuição de função para as atribuições de função especialmente atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="84ab5-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84ab5-118">Relações</span><span class="sxs-lookup"><span data-stu-id="84ab5-118">Relationships</span></span>
<span data-ttu-id="84ab5-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84ab5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84ab5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84ab5-120">JSON Representation</span></span>
<span data-ttu-id="84ab5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84ab5-121">Here is a JSON representation of the resource.</span></span>
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






