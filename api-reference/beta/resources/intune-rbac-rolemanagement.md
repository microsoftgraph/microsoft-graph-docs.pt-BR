---
title: tipo de recurso roleManagement
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40a74c46f02aef42c8785e666705278980c544c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021494"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="142cd-103">tipo de recurso roleManagement</span><span class="sxs-lookup"><span data-stu-id="142cd-103">roleManagement resource type</span></span>

<span data-ttu-id="142cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="142cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="142cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="142cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="142cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="142cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="142cd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="142cd-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="142cd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="142cd-108">Methods</span></span>
|<span data-ttu-id="142cd-109">Método</span><span class="sxs-lookup"><span data-stu-id="142cd-109">Method</span></span>|<span data-ttu-id="142cd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="142cd-110">Return Type</span></span>|<span data-ttu-id="142cd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="142cd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="142cd-112">Obter roleManagement</span><span class="sxs-lookup"><span data-stu-id="142cd-112">Get roleManagement</span></span>](../api/intune-rbac-rolemanagement-get.md)|[<span data-ttu-id="142cd-113">roleManagement</span><span class="sxs-lookup"><span data-stu-id="142cd-113">roleManagement</span></span>](../resources/intune-rbac-rolemanagement.md)|<span data-ttu-id="142cd-114">Leia as propriedades e as relações do objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="142cd-114">Read properties and relationships of the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>|
|[<span data-ttu-id="142cd-115">Atualizar roleManagement</span><span class="sxs-lookup"><span data-stu-id="142cd-115">Update roleManagement</span></span>](../api/intune-rbac-rolemanagement-update.md)|[<span data-ttu-id="142cd-116">roleManagement</span><span class="sxs-lookup"><span data-stu-id="142cd-116">roleManagement</span></span>](../resources/intune-rbac-rolemanagement.md)|<span data-ttu-id="142cd-117">Atualiza as propriedades de um objeto [roleManagement](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="142cd-117">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="142cd-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="142cd-118">Properties</span></span>
|<span data-ttu-id="142cd-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="142cd-119">Property</span></span>|<span data-ttu-id="142cd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="142cd-120">Type</span></span>|<span data-ttu-id="142cd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="142cd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="142cd-122">id</span><span class="sxs-lookup"><span data-stu-id="142cd-122">id</span></span>|<span data-ttu-id="142cd-123">String</span><span class="sxs-lookup"><span data-stu-id="142cd-123">String</span></span>|<span data-ttu-id="142cd-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="142cd-124">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="142cd-125">Relações</span><span class="sxs-lookup"><span data-stu-id="142cd-125">Relationships</span></span>
|<span data-ttu-id="142cd-126">Relação</span><span class="sxs-lookup"><span data-stu-id="142cd-126">Relationship</span></span>|<span data-ttu-id="142cd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="142cd-127">Type</span></span>|<span data-ttu-id="142cd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="142cd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="142cd-129">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="142cd-129">deviceManagement</span></span>|[<span data-ttu-id="142cd-130">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="142cd-130">rbacApplicationMultiple</span></span>](../resources/intune-rbac-rbacapplicationmultiple.md)|<span data-ttu-id="142cd-131">O RbacApplication para gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="142cd-131">The RbacApplication for Device Management</span></span>|

## <a name="json-representation"></a><span data-ttu-id="142cd-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="142cd-132">JSON Representation</span></span>
<span data-ttu-id="142cd-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="142cd-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "String (identifier)"
}
```






