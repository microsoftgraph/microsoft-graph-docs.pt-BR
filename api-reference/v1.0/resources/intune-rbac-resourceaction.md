---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 899075a8ac494daf345fa6f8d91e3cc38126ec53
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441620"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="a8047-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="a8047-103">resourceAction resource type</span></span>

<span data-ttu-id="a8047-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8047-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8047-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8047-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8047-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8047-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a8047-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8047-107">Properties</span></span>
|<span data-ttu-id="a8047-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8047-108">Property</span></span>|<span data-ttu-id="a8047-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8047-109">Type</span></span>|<span data-ttu-id="a8047-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8047-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8047-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a8047-111">allowedResourceActions</span></span>|<span data-ttu-id="a8047-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8047-112">String collection</span></span>|<span data-ttu-id="a8047-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="a8047-113">Allowed Actions</span></span>|
|<span data-ttu-id="a8047-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a8047-114">notAllowedResourceActions</span></span>|<span data-ttu-id="a8047-115">String collection</span><span class="sxs-lookup"><span data-stu-id="a8047-115">String collection</span></span>|<span data-ttu-id="a8047-116">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="a8047-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8047-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a8047-117">Relationships</span></span>
<span data-ttu-id="a8047-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8047-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8047-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8047-119">JSON Representation</span></span>
<span data-ttu-id="a8047-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8047-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```







