---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 657df623da3498588d9d6aa6f6d6fb121285c33e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529764"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="41833-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="41833-103">keyValue resource type</span></span>

<span data-ttu-id="41833-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41833-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41833-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41833-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41833-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41833-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41833-107">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="41833-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="41833-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41833-108">Properties</span></span>
|<span data-ttu-id="41833-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41833-109">Property</span></span>|<span data-ttu-id="41833-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41833-110">Type</span></span>|<span data-ttu-id="41833-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41833-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41833-112">key</span><span class="sxs-lookup"><span data-stu-id="41833-112">key</span></span>|<span data-ttu-id="41833-113">String</span><span class="sxs-lookup"><span data-stu-id="41833-113">String</span></span>|<span data-ttu-id="41833-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="41833-114">Key.</span></span>|
|<span data-ttu-id="41833-115">value</span><span class="sxs-lookup"><span data-stu-id="41833-115">value</span></span>|<span data-ttu-id="41833-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41833-116">String</span></span>|<span data-ttu-id="41833-117">Valor.</span><span class="sxs-lookup"><span data-stu-id="41833-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41833-118">Relações</span><span class="sxs-lookup"><span data-stu-id="41833-118">Relationships</span></span>
<span data-ttu-id="41833-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41833-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41833-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41833-120">JSON Representation</span></span>
<span data-ttu-id="41833-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41833-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```



