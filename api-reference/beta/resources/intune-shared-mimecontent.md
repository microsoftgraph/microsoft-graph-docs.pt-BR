---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86537f6d93f2ff50c212105fce3f4fb91f137184
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466163"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="b8233-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="b8233-103">mimeContent resource type</span></span>

<span data-ttu-id="b8233-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8233-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8233-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8233-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8233-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8233-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8233-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="b8233-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="b8233-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8233-108">Properties</span></span>
|<span data-ttu-id="b8233-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8233-109">Property</span></span>|<span data-ttu-id="b8233-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8233-110">Type</span></span>|<span data-ttu-id="b8233-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8233-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8233-112">type</span><span class="sxs-lookup"><span data-stu-id="b8233-112">type</span></span>|<span data-ttu-id="b8233-113">String</span><span class="sxs-lookup"><span data-stu-id="b8233-113">String</span></span>|<span data-ttu-id="b8233-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="b8233-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="b8233-115">value</span><span class="sxs-lookup"><span data-stu-id="b8233-115">value</span></span>|<span data-ttu-id="b8233-116">Binária</span><span class="sxs-lookup"><span data-stu-id="b8233-116">Binary</span></span>|<span data-ttu-id="b8233-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="b8233-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8233-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b8233-118">Relationships</span></span>
<span data-ttu-id="b8233-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8233-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8233-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8233-120">JSON Representation</span></span>
<span data-ttu-id="b8233-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8233-121">Here is a JSON representation of the resource.</span></span>
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



