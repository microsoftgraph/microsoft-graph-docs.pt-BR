---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c3c5f909d0960b9d83c5a5a38e12fe19f26b9af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258952"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="eae65-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="eae65-103">mimeContent resource type</span></span>

<span data-ttu-id="eae65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eae65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eae65-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eae65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eae65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eae65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eae65-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="eae65-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="eae65-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eae65-108">Properties</span></span>
|<span data-ttu-id="eae65-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eae65-109">Property</span></span>|<span data-ttu-id="eae65-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eae65-110">Type</span></span>|<span data-ttu-id="eae65-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eae65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eae65-112">tipo</span><span class="sxs-lookup"><span data-stu-id="eae65-112">type</span></span>|<span data-ttu-id="eae65-113">String</span><span class="sxs-lookup"><span data-stu-id="eae65-113">String</span></span>|<span data-ttu-id="eae65-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="eae65-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="eae65-115">value</span><span class="sxs-lookup"><span data-stu-id="eae65-115">value</span></span>|<span data-ttu-id="eae65-116">Binária</span><span class="sxs-lookup"><span data-stu-id="eae65-116">Binary</span></span>|<span data-ttu-id="eae65-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="eae65-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eae65-118">Relações</span><span class="sxs-lookup"><span data-stu-id="eae65-118">Relationships</span></span>
<span data-ttu-id="eae65-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eae65-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eae65-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eae65-120">JSON Representation</span></span>
<span data-ttu-id="eae65-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eae65-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```




