---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4360ce5a8873fde7d3286f55fc0c8993936a7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571874"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="cb8a1-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb8a1-103">mimeContent resource type</span></span>

> <span data-ttu-id="cb8a1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb8a1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb8a1-105">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="cb8a1-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="cb8a1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb8a1-106">Properties</span></span>
|<span data-ttu-id="cb8a1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb8a1-107">Property</span></span>|<span data-ttu-id="cb8a1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb8a1-108">Type</span></span>|<span data-ttu-id="cb8a1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb8a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb8a1-110">type</span><span class="sxs-lookup"><span data-stu-id="cb8a1-110">type</span></span>|<span data-ttu-id="cb8a1-111">String</span><span class="sxs-lookup"><span data-stu-id="cb8a1-111">String</span></span>|<span data-ttu-id="cb8a1-112">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="cb8a1-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="cb8a1-113">value</span><span class="sxs-lookup"><span data-stu-id="cb8a1-113">value</span></span>|<span data-ttu-id="cb8a1-114">Binária</span><span class="sxs-lookup"><span data-stu-id="cb8a1-114">Binary</span></span>|<span data-ttu-id="cb8a1-115">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="cb8a1-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb8a1-116">Relações</span><span class="sxs-lookup"><span data-stu-id="cb8a1-116">Relationships</span></span>
<span data-ttu-id="cb8a1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb8a1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb8a1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb8a1-118">JSON Representation</span></span>
<span data-ttu-id="cb8a1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb8a1-119">Here is a JSON representation of the resource.</span></span>
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



