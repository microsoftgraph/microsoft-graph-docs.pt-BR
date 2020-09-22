---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 941ebf1c7a56e04acaa118bf0d0ed8594172c726
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037805"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="59850-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="59850-103">resourceAction resource type</span></span>

<span data-ttu-id="59850-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59850-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59850-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59850-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59850-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="59850-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="59850-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59850-107">Properties</span></span>
|<span data-ttu-id="59850-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59850-108">Property</span></span>|<span data-ttu-id="59850-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="59850-109">Type</span></span>|<span data-ttu-id="59850-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="59850-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59850-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="59850-111">allowedResourceActions</span></span>|<span data-ttu-id="59850-112">String collection</span><span class="sxs-lookup"><span data-stu-id="59850-112">String collection</span></span>|<span data-ttu-id="59850-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="59850-113">Allowed Actions</span></span>|
|<span data-ttu-id="59850-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="59850-114">notAllowedResourceActions</span></span>|<span data-ttu-id="59850-115">String collection</span><span class="sxs-lookup"><span data-stu-id="59850-115">String collection</span></span>|<span data-ttu-id="59850-116">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="59850-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="59850-117">Relações</span><span class="sxs-lookup"><span data-stu-id="59850-117">Relationships</span></span>
<span data-ttu-id="59850-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59850-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59850-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59850-119">JSON Representation</span></span>
<span data-ttu-id="59850-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59850-120">Here is a JSON representation of the resource.</span></span>
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









