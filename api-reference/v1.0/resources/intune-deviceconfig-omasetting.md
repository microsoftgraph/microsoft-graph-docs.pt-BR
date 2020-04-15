---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0172d3cb6955df6e154758750fdc87aef2789292
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473075"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="612fd-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="612fd-103">omaSetting resource type</span></span>

<span data-ttu-id="612fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="612fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="612fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="612fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="612fd-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="612fd-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="612fd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="612fd-107">Properties</span></span>
|<span data-ttu-id="612fd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="612fd-108">Property</span></span>|<span data-ttu-id="612fd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="612fd-109">Type</span></span>|<span data-ttu-id="612fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="612fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="612fd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="612fd-111">displayName</span></span>|<span data-ttu-id="612fd-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="612fd-112">String</span></span>|<span data-ttu-id="612fd-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="612fd-113">Display Name.</span></span>|
|<span data-ttu-id="612fd-114">description</span><span class="sxs-lookup"><span data-stu-id="612fd-114">description</span></span>|<span data-ttu-id="612fd-115">String</span><span class="sxs-lookup"><span data-stu-id="612fd-115">String</span></span>|<span data-ttu-id="612fd-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="612fd-116">Description.</span></span>|
|<span data-ttu-id="612fd-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="612fd-117">omaUri</span></span>|<span data-ttu-id="612fd-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="612fd-118">String</span></span>|<span data-ttu-id="612fd-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="612fd-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="612fd-120">Relações</span><span class="sxs-lookup"><span data-stu-id="612fd-120">Relationships</span></span>
<span data-ttu-id="612fd-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="612fd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="612fd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="612fd-122">JSON Representation</span></span>
<span data-ttu-id="612fd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="612fd-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```







