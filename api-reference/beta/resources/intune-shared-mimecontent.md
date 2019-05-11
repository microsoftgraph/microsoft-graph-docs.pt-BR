---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f2224d255e8aa4ceb48554fdc01356277ffbc89
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939109"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="9e32e-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="9e32e-103">mimeContent resource type</span></span>

> <span data-ttu-id="9e32e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e32e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e32e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e32e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e32e-106">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="9e32e-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="9e32e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e32e-107">Properties</span></span>
|<span data-ttu-id="9e32e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e32e-108">Property</span></span>|<span data-ttu-id="9e32e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e32e-109">Type</span></span>|<span data-ttu-id="9e32e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e32e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e32e-111">type</span><span class="sxs-lookup"><span data-stu-id="9e32e-111">type</span></span>|<span data-ttu-id="9e32e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e32e-112">String</span></span>|<span data-ttu-id="9e32e-113">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="9e32e-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="9e32e-114">value</span><span class="sxs-lookup"><span data-stu-id="9e32e-114">value</span></span>|<span data-ttu-id="9e32e-115">Binária</span><span class="sxs-lookup"><span data-stu-id="9e32e-115">Binary</span></span>|<span data-ttu-id="9e32e-116">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="9e32e-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e32e-117">Relações</span><span class="sxs-lookup"><span data-stu-id="9e32e-117">Relationships</span></span>
<span data-ttu-id="9e32e-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e32e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e32e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e32e-119">JSON Representation</span></span>
<span data-ttu-id="9e32e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e32e-120">Here is a JSON representation of the resource.</span></span>
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




