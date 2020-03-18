---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6fc230ab7644724ca971639c98394ebc256c1194
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768916"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="18a01-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="18a01-103">mimeContent resource type</span></span>

> <span data-ttu-id="18a01-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18a01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18a01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a01-106">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="18a01-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="18a01-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18a01-107">Properties</span></span>
|<span data-ttu-id="18a01-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a01-108">Property</span></span>|<span data-ttu-id="18a01-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a01-109">Type</span></span>|<span data-ttu-id="18a01-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a01-111">type</span><span class="sxs-lookup"><span data-stu-id="18a01-111">type</span></span>|<span data-ttu-id="18a01-112">String</span><span class="sxs-lookup"><span data-stu-id="18a01-112">String</span></span>|<span data-ttu-id="18a01-113">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="18a01-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="18a01-114">value</span><span class="sxs-lookup"><span data-stu-id="18a01-114">value</span></span>|<span data-ttu-id="18a01-115">Binária</span><span class="sxs-lookup"><span data-stu-id="18a01-115">Binary</span></span>|<span data-ttu-id="18a01-116">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="18a01-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a01-117">Relações</span><span class="sxs-lookup"><span data-stu-id="18a01-117">Relationships</span></span>
<span data-ttu-id="18a01-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a01-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18a01-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18a01-119">JSON Representation</span></span>
<span data-ttu-id="18a01-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18a01-120">Here is a JSON representation of the resource.</span></span>
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



