---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
ms.openlocfilehash: 05088fa472c8f8a71adabbb0c807e7b2f0b80b09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333492"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="5a138-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="5a138-103">mimeContent resource type</span></span>

> <span data-ttu-id="5a138-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a138-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a138-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a138-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a138-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a138-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a138-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="5a138-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="5a138-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a138-108">Properties</span></span>
|<span data-ttu-id="5a138-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a138-109">Property</span></span>|<span data-ttu-id="5a138-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a138-110">Type</span></span>|<span data-ttu-id="5a138-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a138-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a138-112">type</span><span class="sxs-lookup"><span data-stu-id="5a138-112">type</span></span>|<span data-ttu-id="5a138-113">String</span><span class="sxs-lookup"><span data-stu-id="5a138-113">String</span></span>|<span data-ttu-id="5a138-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="5a138-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="5a138-115">valor</span><span class="sxs-lookup"><span data-stu-id="5a138-115">value</span></span>|<span data-ttu-id="5a138-116">Binária</span><span class="sxs-lookup"><span data-stu-id="5a138-116">Binary</span></span>|<span data-ttu-id="5a138-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="5a138-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a138-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5a138-118">Relationships</span></span>
<span data-ttu-id="5a138-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a138-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a138-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a138-120">JSON Representation</span></span>
<span data-ttu-id="5a138-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a138-121">Here is a JSON representation of the resource.</span></span>
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





