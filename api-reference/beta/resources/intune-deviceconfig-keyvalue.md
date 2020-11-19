---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0d112c76e03f45ba7bf28fea3b6d219745c4332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283215"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="6c68e-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="6c68e-103">keyValue resource type</span></span>

<span data-ttu-id="6c68e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c68e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c68e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c68e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c68e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c68e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c68e-107">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="6c68e-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6c68e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c68e-108">Properties</span></span>
|<span data-ttu-id="6c68e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c68e-109">Property</span></span>|<span data-ttu-id="6c68e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c68e-110">Type</span></span>|<span data-ttu-id="6c68e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c68e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c68e-112">key</span><span class="sxs-lookup"><span data-stu-id="6c68e-112">key</span></span>|<span data-ttu-id="6c68e-113">String</span><span class="sxs-lookup"><span data-stu-id="6c68e-113">String</span></span>|<span data-ttu-id="6c68e-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="6c68e-114">Key.</span></span>|
|<span data-ttu-id="6c68e-115">value</span><span class="sxs-lookup"><span data-stu-id="6c68e-115">value</span></span>|<span data-ttu-id="6c68e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c68e-116">String</span></span>|<span data-ttu-id="6c68e-117">Valor.</span><span class="sxs-lookup"><span data-stu-id="6c68e-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c68e-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6c68e-118">Relationships</span></span>
<span data-ttu-id="6c68e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c68e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c68e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c68e-120">JSON Representation</span></span>
<span data-ttu-id="6c68e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c68e-121">Here is a JSON representation of the resource.</span></span>
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




