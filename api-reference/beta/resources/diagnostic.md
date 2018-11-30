---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
ms.openlocfilehash: 29e30d44a9fde91b79778042be19461b880216ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038948"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="d0ced-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="d0ced-103">diagnostic resource type</span></span>

> <span data-ttu-id="d0ced-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0ced-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0ced-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0ced-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0ced-106">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d0ced-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0ced-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0ced-107">JSON representation</span></span>

<span data-ttu-id="d0ced-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d0ced-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d0ced-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0ced-109">Properties</span></span>
| <span data-ttu-id="d0ced-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0ced-110">Property</span></span>     | <span data-ttu-id="d0ced-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0ced-111">Type</span></span>   |<span data-ttu-id="d0ced-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0ced-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0ced-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="d0ced-113">message</span></span>|<span data-ttu-id="d0ced-114">String</span><span class="sxs-lookup"><span data-stu-id="d0ced-114">String</span></span>|<span data-ttu-id="d0ced-115">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="d0ced-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="d0ced-116">url</span><span class="sxs-lookup"><span data-stu-id="d0ced-116">url</span></span>|<span data-ttu-id="d0ced-117">String</span><span class="sxs-lookup"><span data-stu-id="d0ced-117">String</span></span>|<span data-ttu-id="d0ced-118">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="d0ced-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->