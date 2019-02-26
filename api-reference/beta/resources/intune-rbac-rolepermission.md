---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b56df927cda3cbf98e7d736311aba2db5e53906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145378"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8eab0-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="8eab0-103">rolePermission resource type</span></span>

> <span data-ttu-id="8eab0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8eab0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eab0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8eab0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eab0-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8eab0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8eab0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eab0-107">Properties</span></span>
|<span data-ttu-id="8eab0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eab0-108">Property</span></span>|<span data-ttu-id="8eab0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eab0-109">Type</span></span>|<span data-ttu-id="8eab0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eab0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eab0-111">actions</span><span class="sxs-lookup"><span data-stu-id="8eab0-111">actions</span></span>|<span data-ttu-id="8eab0-112">String collection</span><span class="sxs-lookup"><span data-stu-id="8eab0-112">String collection</span></span>|<span data-ttu-id="8eab0-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="8eab0-113">Allowed Actions</span></span>|
|<span data-ttu-id="8eab0-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8eab0-114">resourceActions</span></span>|<span data-ttu-id="8eab0-115">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="8eab0-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8eab0-116">Ações</span><span class="sxs-lookup"><span data-stu-id="8eab0-116">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eab0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8eab0-117">Relationships</span></span>
<span data-ttu-id="8eab0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8eab0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eab0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eab0-119">JSON Representation</span></span>
<span data-ttu-id="8eab0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8eab0-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```




