---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6a2365223904f61b6c0b4aada6a26cf5888acf0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445826"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="5c9b5-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="5c9b5-103">keyValuePair resource type</span></span>

<span data-ttu-id="5c9b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c9b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c9b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c9b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c9b5-106">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="5c9b5-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="5c9b5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c9b5-107">Properties</span></span>
|<span data-ttu-id="5c9b5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c9b5-108">Property</span></span>|<span data-ttu-id="5c9b5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c9b5-109">Type</span></span>|<span data-ttu-id="5c9b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c9b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c9b5-111">nome</span><span class="sxs-lookup"><span data-stu-id="5c9b5-111">name</span></span>|<span data-ttu-id="5c9b5-112">String</span><span class="sxs-lookup"><span data-stu-id="5c9b5-112">String</span></span>|<span data-ttu-id="5c9b5-113">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="5c9b5-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="5c9b5-114">value</span><span class="sxs-lookup"><span data-stu-id="5c9b5-114">value</span></span>|<span data-ttu-id="5c9b5-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c9b5-115">String</span></span>|<span data-ttu-id="5c9b5-116">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="5c9b5-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c9b5-117">Relações</span><span class="sxs-lookup"><span data-stu-id="5c9b5-117">Relationships</span></span>
<span data-ttu-id="5c9b5-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c9b5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c9b5-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c9b5-119">JSON Representation</span></span>
<span data-ttu-id="5c9b5-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c9b5-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```







