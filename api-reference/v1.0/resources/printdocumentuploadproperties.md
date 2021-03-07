---
author: nilakhan
description: Representa informações para upload de documento de impressão
title: Tipo de recurso printDocumentUploadProperties
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: e877901b842670e09cb283b40613a1185aabaafe
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516912"
---
# <a name="printdocumentuploadproperties-resource-type"></a><span data-ttu-id="5743e-103">Tipo de recurso printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="5743e-103">printDocumentUploadProperties resource type</span></span>

<span data-ttu-id="5743e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5743e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5743e-105">Descreve o documento que está sendo carregado</span><span class="sxs-lookup"><span data-stu-id="5743e-105">Describes the document that is being uploaded</span></span>

## <a name="properties"></a><span data-ttu-id="5743e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5743e-106">Properties</span></span>
|<span data-ttu-id="5743e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5743e-107">Property</span></span>|<span data-ttu-id="5743e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5743e-108">Type</span></span>|<span data-ttu-id="5743e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5743e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5743e-110">contentType</span><span class="sxs-lookup"><span data-stu-id="5743e-110">contentType</span></span>|<span data-ttu-id="5743e-111">String</span><span class="sxs-lookup"><span data-stu-id="5743e-111">String</span></span>|<span data-ttu-id="5743e-112">Tipo de conteúdo do documento (MIME).</span><span class="sxs-lookup"><span data-stu-id="5743e-112">The document's content (MIME) type.</span></span>|
|<span data-ttu-id="5743e-113">documentName</span><span class="sxs-lookup"><span data-stu-id="5743e-113">documentName</span></span>|<span data-ttu-id="5743e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5743e-114">String</span></span>|<span data-ttu-id="5743e-115">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="5743e-115">The document's name.</span></span>|
|<span data-ttu-id="5743e-116">size</span><span class="sxs-lookup"><span data-stu-id="5743e-116">size</span></span>|<span data-ttu-id="5743e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5743e-117">Int64</span></span>|<span data-ttu-id="5743e-118">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="5743e-118">The document's size in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5743e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5743e-119">Relationships</span></span>
<span data-ttu-id="5743e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5743e-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5743e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5743e-121">JSON representation</span></span>
<span data-ttu-id="5743e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5743e-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printDocumentUploadProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocumentUploadProperties",
  "contentType": "String",
  "documentName": "String",
  "size": "Integer"
}
```

