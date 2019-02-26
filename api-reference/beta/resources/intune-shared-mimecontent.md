---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f446983d5dfe101c89171baa776b32759726f279
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161653"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="9aa5f-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="9aa5f-103">mimeContent resource type</span></span>

> <span data-ttu-id="9aa5f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9aa5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9aa5f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9aa5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aa5f-106">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="9aa5f-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="9aa5f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9aa5f-107">Properties</span></span>
|<span data-ttu-id="9aa5f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aa5f-108">Property</span></span>|<span data-ttu-id="9aa5f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aa5f-109">Type</span></span>|<span data-ttu-id="9aa5f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa5f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa5f-111">type</span><span class="sxs-lookup"><span data-stu-id="9aa5f-111">type</span></span>|<span data-ttu-id="9aa5f-112">String</span><span class="sxs-lookup"><span data-stu-id="9aa5f-112">String</span></span>|<span data-ttu-id="9aa5f-113">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="9aa5f-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="9aa5f-114">valor</span><span class="sxs-lookup"><span data-stu-id="9aa5f-114">value</span></span>|<span data-ttu-id="9aa5f-115">Binária</span><span class="sxs-lookup"><span data-stu-id="9aa5f-115">Binary</span></span>|<span data-ttu-id="9aa5f-116">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="9aa5f-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aa5f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="9aa5f-117">Relationships</span></span>
<span data-ttu-id="9aa5f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9aa5f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aa5f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9aa5f-119">JSON Representation</span></span>
<span data-ttu-id="9aa5f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9aa5f-120">Here is a JSON representation of the resource.</span></span>
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




