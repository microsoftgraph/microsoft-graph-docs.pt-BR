---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4af707320da09c9b72537168f8fd77a424c790
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465430"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="acad9-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="acad9-103">keyValuePair resource type</span></span>

> <span data-ttu-id="acad9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="acad9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acad9-105">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="acad9-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="acad9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acad9-106">Properties</span></span>
|<span data-ttu-id="acad9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acad9-107">Property</span></span>|<span data-ttu-id="acad9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="acad9-108">Type</span></span>|<span data-ttu-id="acad9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="acad9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acad9-110">nome</span><span class="sxs-lookup"><span data-stu-id="acad9-110">name</span></span>|<span data-ttu-id="acad9-111">String</span><span class="sxs-lookup"><span data-stu-id="acad9-111">String</span></span>|<span data-ttu-id="acad9-112">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="acad9-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="acad9-113">value</span><span class="sxs-lookup"><span data-stu-id="acad9-113">value</span></span>|<span data-ttu-id="acad9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acad9-114">String</span></span>|<span data-ttu-id="acad9-115">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="acad9-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="acad9-116">Relações</span><span class="sxs-lookup"><span data-stu-id="acad9-116">Relationships</span></span>
<span data-ttu-id="acad9-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="acad9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acad9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acad9-118">JSON Representation</span></span>
<span data-ttu-id="acad9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acad9-119">Here is a JSON representation of the resource.</span></span>
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



