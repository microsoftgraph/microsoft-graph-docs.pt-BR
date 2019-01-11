---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 826606d41feb0f0a156a1b8240bde7f4ac926a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838224"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="ab47f-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="ab47f-103">mimeContent resource type</span></span>

> <span data-ttu-id="ab47f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab47f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab47f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab47f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab47f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ab47f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab47f-107">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="ab47f-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="ab47f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab47f-108">Properties</span></span>
|<span data-ttu-id="ab47f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab47f-109">Property</span></span>|<span data-ttu-id="ab47f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab47f-110">Type</span></span>|<span data-ttu-id="ab47f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab47f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab47f-112">type</span><span class="sxs-lookup"><span data-stu-id="ab47f-112">type</span></span>|<span data-ttu-id="ab47f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab47f-113">String</span></span>|<span data-ttu-id="ab47f-114">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="ab47f-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="ab47f-115">valor</span><span class="sxs-lookup"><span data-stu-id="ab47f-115">value</span></span>|<span data-ttu-id="ab47f-116">Binária</span><span class="sxs-lookup"><span data-stu-id="ab47f-116">Binary</span></span>|<span data-ttu-id="ab47f-117">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="ab47f-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab47f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ab47f-118">Relationships</span></span>
<span data-ttu-id="ab47f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab47f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ab47f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab47f-120">JSON Representation</span></span>
<span data-ttu-id="ab47f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab47f-121">Here is a JSON representation of the resource.</span></span>
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





