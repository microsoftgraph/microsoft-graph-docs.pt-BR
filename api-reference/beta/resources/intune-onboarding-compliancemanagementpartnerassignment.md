---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a04caf164e6761c95676b9029a2533cd86e7370
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524199"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="fa758-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="fa758-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="fa758-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa758-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa758-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa758-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa758-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa758-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa758-107">Direcionamento de grupo de usuários para parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="fa758-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="fa758-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa758-108">Properties</span></span>
|<span data-ttu-id="fa758-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa758-109">Property</span></span>|<span data-ttu-id="fa758-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa758-110">Type</span></span>|<span data-ttu-id="fa758-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa758-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa758-112">destino</span><span class="sxs-lookup"><span data-stu-id="fa758-112">target</span></span>|[<span data-ttu-id="fa758-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa758-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fa758-114">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="fa758-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa758-115">Relações</span><span class="sxs-lookup"><span data-stu-id="fa758-115">Relationships</span></span>
<span data-ttu-id="fa758-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa758-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa758-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa758-117">JSON Representation</span></span>
<span data-ttu-id="fa758-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa758-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



