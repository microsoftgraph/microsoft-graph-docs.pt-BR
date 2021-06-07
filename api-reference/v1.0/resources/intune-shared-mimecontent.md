---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e17fd6abb6470fe46c836f7ed4b9f38362abb74d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751549"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="ec23d-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="ec23d-103">mimeContent resource type</span></span>

<span data-ttu-id="ec23d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec23d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec23d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec23d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec23d-106">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="ec23d-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="ec23d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec23d-107">Properties</span></span>
|<span data-ttu-id="ec23d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec23d-108">Property</span></span>|<span data-ttu-id="ec23d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec23d-109">Type</span></span>|<span data-ttu-id="ec23d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec23d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec23d-111">tipo</span><span class="sxs-lookup"><span data-stu-id="ec23d-111">type</span></span>|<span data-ttu-id="ec23d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec23d-112">String</span></span>|<span data-ttu-id="ec23d-113">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="ec23d-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="ec23d-114">value</span><span class="sxs-lookup"><span data-stu-id="ec23d-114">value</span></span>|<span data-ttu-id="ec23d-115">Binária</span><span class="sxs-lookup"><span data-stu-id="ec23d-115">Binary</span></span>|<span data-ttu-id="ec23d-116">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="ec23d-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec23d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ec23d-117">Relationships</span></span>
<span data-ttu-id="ec23d-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ec23d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec23d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec23d-119">JSON Representation</span></span>
<span data-ttu-id="ec23d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec23d-120">Here is a JSON representation of the resource.</span></span>
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




