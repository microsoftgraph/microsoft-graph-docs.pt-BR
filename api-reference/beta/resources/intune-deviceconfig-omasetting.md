---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88b5a45d466a50f3bdc9a5b53790ff5c10f53904
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024042"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="058a2-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="058a2-103">omaSetting resource type</span></span>

<span data-ttu-id="058a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="058a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="058a2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="058a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="058a2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="058a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="058a2-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="058a2-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="058a2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="058a2-108">Properties</span></span>
|<span data-ttu-id="058a2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="058a2-109">Property</span></span>|<span data-ttu-id="058a2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="058a2-110">Type</span></span>|<span data-ttu-id="058a2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="058a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="058a2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="058a2-112">displayName</span></span>|<span data-ttu-id="058a2-113">String</span><span class="sxs-lookup"><span data-stu-id="058a2-113">String</span></span>|<span data-ttu-id="058a2-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="058a2-114">Display Name.</span></span>|
|<span data-ttu-id="058a2-115">description</span><span class="sxs-lookup"><span data-stu-id="058a2-115">description</span></span>|<span data-ttu-id="058a2-116">String</span><span class="sxs-lookup"><span data-stu-id="058a2-116">String</span></span>|<span data-ttu-id="058a2-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="058a2-117">Description.</span></span>|
|<span data-ttu-id="058a2-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="058a2-118">omaUri</span></span>|<span data-ttu-id="058a2-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="058a2-119">String</span></span>|<span data-ttu-id="058a2-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="058a2-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="058a2-121">Relações</span><span class="sxs-lookup"><span data-stu-id="058a2-121">Relationships</span></span>
<span data-ttu-id="058a2-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="058a2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="058a2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="058a2-123">JSON Representation</span></span>
<span data-ttu-id="058a2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="058a2-124">Here is a JSON representation of the resource.</span></span>
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






