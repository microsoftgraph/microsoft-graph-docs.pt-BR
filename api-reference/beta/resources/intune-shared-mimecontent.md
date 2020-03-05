---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a867133dca99fb15044452163b050fdcb2f3d14
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527361"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="04137-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="04137-103">mimeContent resource type</span></span>

<span data-ttu-id="04137-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04137-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04137-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04137-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04137-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04137-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="04137-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="04137-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04137-108">Properties</span></span>
|<span data-ttu-id="04137-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04137-109">Property</span></span>|<span data-ttu-id="04137-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04137-110">Type</span></span>|<span data-ttu-id="04137-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04137-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04137-112">type</span><span class="sxs-lookup"><span data-stu-id="04137-112">type</span></span>|<span data-ttu-id="04137-113">String</span><span class="sxs-lookup"><span data-stu-id="04137-113">String</span></span>|<span data-ttu-id="04137-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="04137-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="04137-115">value</span><span class="sxs-lookup"><span data-stu-id="04137-115">value</span></span>|<span data-ttu-id="04137-116">Binária</span><span class="sxs-lookup"><span data-stu-id="04137-116">Binary</span></span>|<span data-ttu-id="04137-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="04137-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04137-118">Relações</span><span class="sxs-lookup"><span data-stu-id="04137-118">Relationships</span></span>
<span data-ttu-id="04137-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04137-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04137-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04137-120">JSON Representation</span></span>
<span data-ttu-id="04137-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04137-121">Here is a JSON representation of the resource.</span></span>
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



