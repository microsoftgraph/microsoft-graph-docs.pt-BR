---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
ms.openlocfilehash: 28cdd1c07bab0494a69cfb7ce6a5284238e1ff19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845987"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="2c784-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="2c784-103">diagnostic resource type</span></span>

> <span data-ttu-id="2c784-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c784-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c784-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c784-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c784-106">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="2c784-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c784-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c784-107">JSON representation</span></span>

<span data-ttu-id="2c784-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2c784-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2c784-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c784-109">Properties</span></span>
| <span data-ttu-id="2c784-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c784-110">Property</span></span>     | <span data-ttu-id="2c784-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c784-111">Type</span></span>   |<span data-ttu-id="2c784-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c784-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c784-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="2c784-113">message</span></span>|<span data-ttu-id="2c784-114">String</span><span class="sxs-lookup"><span data-stu-id="2c784-114">String</span></span>|<span data-ttu-id="2c784-115">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="2c784-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="2c784-116">url</span><span class="sxs-lookup"><span data-stu-id="2c784-116">url</span></span>|<span data-ttu-id="2c784-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c784-117">String</span></span>|<span data-ttu-id="2c784-118">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="2c784-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
