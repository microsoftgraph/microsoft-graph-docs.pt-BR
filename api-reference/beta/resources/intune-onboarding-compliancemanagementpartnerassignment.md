---
title: Tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para Parceiro de Gerenciamento de Conformidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46e4e6a5e073e3087267329880cf0f36bb79c4a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161436"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="0a7be-103">Tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="0a7be-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="0a7be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a7be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a7be-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a7be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a7be-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a7be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a7be-107">Direcionamento de grupo de usuários para Parceiro de Gerenciamento de Conformidade</span><span class="sxs-lookup"><span data-stu-id="0a7be-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="0a7be-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a7be-108">Properties</span></span>
|<span data-ttu-id="0a7be-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a7be-109">Property</span></span>|<span data-ttu-id="0a7be-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a7be-110">Type</span></span>|<span data-ttu-id="0a7be-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a7be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a7be-112">destino</span><span class="sxs-lookup"><span data-stu-id="0a7be-112">target</span></span>|[<span data-ttu-id="0a7be-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0a7be-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0a7be-114">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="0a7be-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a7be-115">Relações</span><span class="sxs-lookup"><span data-stu-id="0a7be-115">Relationships</span></span>
<span data-ttu-id="0a7be-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a7be-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a7be-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a7be-117">JSON Representation</span></span>
<span data-ttu-id="0a7be-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a7be-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




