---
title: tipo de recurso complianceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para Parceiro de Gerenciamento de Conformidade
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 638a50d7c8a6f1723c841c21f06d8cb44ac65460
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755648"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="f089d-103">tipo de recurso complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="f089d-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="f089d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f089d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f089d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f089d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f089d-106">Direcionamento de grupo de usuários para Parceiro de Gerenciamento de Conformidade</span><span class="sxs-lookup"><span data-stu-id="f089d-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="f089d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f089d-107">Properties</span></span>
|<span data-ttu-id="f089d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f089d-108">Property</span></span>|<span data-ttu-id="f089d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f089d-109">Type</span></span>|<span data-ttu-id="f089d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f089d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f089d-111">destino</span><span class="sxs-lookup"><span data-stu-id="f089d-111">target</span></span>|[<span data-ttu-id="f089d-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f089d-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f089d-113">Destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="f089d-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f089d-114">Relações</span><span class="sxs-lookup"><span data-stu-id="f089d-114">Relationships</span></span>
<span data-ttu-id="f089d-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f089d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f089d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f089d-116">JSON Representation</span></span>
<span data-ttu-id="f089d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f089d-117">Here is a JSON representation of the resource.</span></span>
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
    "collectionId": "String"
  }
}
```




