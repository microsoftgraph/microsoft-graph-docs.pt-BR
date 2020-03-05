---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05ddc4b1b1c4c27d72a128460b6d156d78542764
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447819"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="d6ef9-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="d6ef9-103">mimeContent resource type</span></span>

<span data-ttu-id="d6ef9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d6ef9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6ef9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6ef9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6ef9-106">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="d6ef9-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="d6ef9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6ef9-107">Properties</span></span>
|<span data-ttu-id="d6ef9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6ef9-108">Property</span></span>|<span data-ttu-id="d6ef9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ef9-109">Type</span></span>|<span data-ttu-id="d6ef9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ef9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6ef9-111">type</span><span class="sxs-lookup"><span data-stu-id="d6ef9-111">type</span></span>|<span data-ttu-id="d6ef9-112">String</span><span class="sxs-lookup"><span data-stu-id="d6ef9-112">String</span></span>|<span data-ttu-id="d6ef9-113">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="d6ef9-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="d6ef9-114">value</span><span class="sxs-lookup"><span data-stu-id="d6ef9-114">value</span></span>|<span data-ttu-id="d6ef9-115">Binária</span><span class="sxs-lookup"><span data-stu-id="d6ef9-115">Binary</span></span>|<span data-ttu-id="d6ef9-116">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="d6ef9-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6ef9-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d6ef9-117">Relationships</span></span>
<span data-ttu-id="d6ef9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6ef9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6ef9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6ef9-119">JSON Representation</span></span>
<span data-ttu-id="d6ef9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6ef9-120">Here is a JSON representation of the resource.</span></span>
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




