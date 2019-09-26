---
title: tipo de recurso keyTypedValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor digitado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 392988272257bdaf7fc3e5b8bafd6d7ca652547d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199683"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="e2bd8-103">tipo de recurso keyTypedValuePair</span><span class="sxs-lookup"><span data-stu-id="e2bd8-103">keyTypedValuePair resource type</span></span>

> <span data-ttu-id="e2bd8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2bd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2bd8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2bd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2bd8-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor digitado.</span><span class="sxs-lookup"><span data-stu-id="e2bd8-106">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="e2bd8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2bd8-107">Properties</span></span>
|<span data-ttu-id="e2bd8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2bd8-108">Property</span></span>|<span data-ttu-id="e2bd8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2bd8-109">Type</span></span>|<span data-ttu-id="e2bd8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2bd8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2bd8-111">key</span><span class="sxs-lookup"><span data-stu-id="e2bd8-111">key</span></span>|<span data-ttu-id="e2bd8-112">String</span><span class="sxs-lookup"><span data-stu-id="e2bd8-112">String</span></span>|<span data-ttu-id="e2bd8-113">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="e2bd8-113">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2bd8-114">Relações</span><span class="sxs-lookup"><span data-stu-id="e2bd8-114">Relationships</span></span>
<span data-ttu-id="e2bd8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2bd8-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2bd8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2bd8-116">JSON Representation</span></span>
<span data-ttu-id="e2bd8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2bd8-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyTypedValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyTypedValuePair",
  "key": "String"
}
```



