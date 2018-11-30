---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
ms.openlocfilehash: 7f25a1c16b86a45886cd763c1a8a3aa6142c47e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005038"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="7ccb7-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ccb7-103">mimeContent resource type</span></span>

> <span data-ttu-id="7ccb7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7ccb7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ccb7-105">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="7ccb7-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="7ccb7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ccb7-106">Properties</span></span>
|<span data-ttu-id="7ccb7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ccb7-107">Property</span></span>|<span data-ttu-id="7ccb7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ccb7-108">Type</span></span>|<span data-ttu-id="7ccb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ccb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ccb7-110">type</span><span class="sxs-lookup"><span data-stu-id="7ccb7-110">type</span></span>|<span data-ttu-id="7ccb7-111">String</span><span class="sxs-lookup"><span data-stu-id="7ccb7-111">String</span></span>|<span data-ttu-id="7ccb7-112">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="7ccb7-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="7ccb7-113">valor</span><span class="sxs-lookup"><span data-stu-id="7ccb7-113">value</span></span>|<span data-ttu-id="7ccb7-114">Binário</span><span class="sxs-lookup"><span data-stu-id="7ccb7-114">Binary</span></span>|<span data-ttu-id="7ccb7-115">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="7ccb7-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ccb7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="7ccb7-116">Relationships</span></span>
<span data-ttu-id="7ccb7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ccb7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ccb7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ccb7-118">JSON Representation</span></span>
<span data-ttu-id="7ccb7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ccb7-119">Here is a JSON representation of the resource.</span></span>
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



