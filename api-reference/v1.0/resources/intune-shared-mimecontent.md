---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a486753c95afce9dff6ceec5846ff618b9103b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971897"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="61514-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="61514-103">mimeContent resource type</span></span>

> <span data-ttu-id="61514-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61514-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61514-105">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="61514-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="61514-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61514-106">Properties</span></span>
|<span data-ttu-id="61514-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61514-107">Property</span></span>|<span data-ttu-id="61514-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="61514-108">Type</span></span>|<span data-ttu-id="61514-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="61514-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61514-110">type</span><span class="sxs-lookup"><span data-stu-id="61514-110">type</span></span>|<span data-ttu-id="61514-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61514-111">String</span></span>|<span data-ttu-id="61514-112">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="61514-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="61514-113">valor</span><span class="sxs-lookup"><span data-stu-id="61514-113">value</span></span>|<span data-ttu-id="61514-114">Binária</span><span class="sxs-lookup"><span data-stu-id="61514-114">Binary</span></span>|<span data-ttu-id="61514-115">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="61514-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61514-116">Relações</span><span class="sxs-lookup"><span data-stu-id="61514-116">Relationships</span></span>
<span data-ttu-id="61514-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61514-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61514-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61514-118">JSON Representation</span></span>
<span data-ttu-id="61514-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61514-119">Here is a JSON representation of the resource.</span></span>
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



