---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae06b047fc93f09bd2b797a4eeaa296d232a0b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447959"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="90270-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="90270-103">resourceAction resource type</span></span>

<span data-ttu-id="90270-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90270-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90270-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90270-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90270-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="90270-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="90270-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90270-107">Properties</span></span>
|<span data-ttu-id="90270-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90270-108">Property</span></span>|<span data-ttu-id="90270-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="90270-109">Type</span></span>|<span data-ttu-id="90270-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="90270-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90270-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="90270-111">allowedResourceActions</span></span>|<span data-ttu-id="90270-112">String collection</span><span class="sxs-lookup"><span data-stu-id="90270-112">String collection</span></span>|<span data-ttu-id="90270-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="90270-113">Allowed Actions</span></span>|
|<span data-ttu-id="90270-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="90270-114">notAllowedResourceActions</span></span>|<span data-ttu-id="90270-115">String collection</span><span class="sxs-lookup"><span data-stu-id="90270-115">String collection</span></span>|<span data-ttu-id="90270-116">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="90270-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="90270-117">Relações</span><span class="sxs-lookup"><span data-stu-id="90270-117">Relationships</span></span>
<span data-ttu-id="90270-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90270-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90270-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90270-119">JSON Representation</span></span>
<span data-ttu-id="90270-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90270-120">Here is a JSON representation of the resource.</span></span>
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




