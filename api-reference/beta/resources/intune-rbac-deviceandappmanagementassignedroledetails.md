---
title: tipo de recurso de deviceAndAppManagementAssignedRoleDetails
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d6ace16ba496feb24948c3e40c32dd8fcb2fcf48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428836"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="0007a-103">tipo de recurso de deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="0007a-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="0007a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0007a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0007a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0007a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0007a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0007a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0007a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0007a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0007a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0007a-108">Properties</span></span>
|<span data-ttu-id="0007a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0007a-109">Property</span></span>|<span data-ttu-id="0007a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0007a-110">Type</span></span>|<span data-ttu-id="0007a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0007a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0007a-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="0007a-112">roleDefinitionIds</span></span>|<span data-ttu-id="0007a-113">String collection</span><span class="sxs-lookup"><span data-stu-id="0007a-113">String collection</span></span>|<span data-ttu-id="0007a-114">IDs de definição de função para o specifc definições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="0007a-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="0007a-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="0007a-115">roleAssignmentIds</span></span>|<span data-ttu-id="0007a-116">String collection</span><span class="sxs-lookup"><span data-stu-id="0007a-116">String collection</span></span>|<span data-ttu-id="0007a-117">IDs de atribuição de função para o specifc atribuições de função atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="0007a-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0007a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0007a-118">Relationships</span></span>
<span data-ttu-id="0007a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0007a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0007a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0007a-120">JSON Representation</span></span>
<span data-ttu-id="0007a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0007a-121">Here is a JSON representation of the resource.</span></span>
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




