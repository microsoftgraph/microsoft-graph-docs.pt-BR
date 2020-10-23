---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 78805e0948a1c77be363a629a9c84f2fe426f22f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732548"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="99a85-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="99a85-103">keyValue resource type</span></span>

<span data-ttu-id="99a85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99a85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99a85-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99a85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99a85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99a85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99a85-107">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="99a85-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="99a85-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99a85-108">Properties</span></span>
|<span data-ttu-id="99a85-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99a85-109">Property</span></span>|<span data-ttu-id="99a85-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="99a85-110">Type</span></span>|<span data-ttu-id="99a85-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99a85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99a85-112">key</span><span class="sxs-lookup"><span data-stu-id="99a85-112">key</span></span>|<span data-ttu-id="99a85-113">String</span><span class="sxs-lookup"><span data-stu-id="99a85-113">String</span></span>|<span data-ttu-id="99a85-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="99a85-114">Key.</span></span>|
|<span data-ttu-id="99a85-115">value</span><span class="sxs-lookup"><span data-stu-id="99a85-115">value</span></span>|<span data-ttu-id="99a85-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99a85-116">String</span></span>|<span data-ttu-id="99a85-117">Valor.</span><span class="sxs-lookup"><span data-stu-id="99a85-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99a85-118">Relações</span><span class="sxs-lookup"><span data-stu-id="99a85-118">Relationships</span></span>
<span data-ttu-id="99a85-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99a85-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99a85-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99a85-120">JSON Representation</span></span>
<span data-ttu-id="99a85-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99a85-121">Here is a JSON representation of the resource.</span></span>
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





