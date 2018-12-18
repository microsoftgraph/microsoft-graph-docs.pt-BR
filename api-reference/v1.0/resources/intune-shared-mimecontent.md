---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
ms.openlocfilehash: 53776793fdd057ef057118decf2d72bb0b61a042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307060"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="f47d0-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="f47d0-103">mimeContent resource type</span></span>

> <span data-ttu-id="f47d0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f47d0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f47d0-105">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="f47d0-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="f47d0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f47d0-106">Properties</span></span>
|<span data-ttu-id="f47d0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f47d0-107">Property</span></span>|<span data-ttu-id="f47d0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f47d0-108">Type</span></span>|<span data-ttu-id="f47d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f47d0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f47d0-110">type</span><span class="sxs-lookup"><span data-stu-id="f47d0-110">type</span></span>|<span data-ttu-id="f47d0-111">String</span><span class="sxs-lookup"><span data-stu-id="f47d0-111">String</span></span>|<span data-ttu-id="f47d0-112">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="f47d0-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="f47d0-113">valor</span><span class="sxs-lookup"><span data-stu-id="f47d0-113">value</span></span>|<span data-ttu-id="f47d0-114">Binária</span><span class="sxs-lookup"><span data-stu-id="f47d0-114">Binary</span></span>|<span data-ttu-id="f47d0-115">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="f47d0-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f47d0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="f47d0-116">Relationships</span></span>
<span data-ttu-id="f47d0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f47d0-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f47d0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f47d0-118">JSON Representation</span></span>
<span data-ttu-id="f47d0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f47d0-119">Here is a JSON representation of the resource.</span></span>
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



