---
title: tipo de recurso de personDataSource
description: Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 540ffa81b20b40f9df2694ba634777250742daaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978498"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="48bd2-103">tipo de recurso de personDataSource</span><span class="sxs-lookup"><span data-stu-id="48bd2-103">personDataSource resource type</span></span>

> <span data-ttu-id="48bd2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48bd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48bd2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48bd2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48bd2-106">Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="48bd2-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48bd2-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48bd2-107">JSON representation</span></span>

<span data-ttu-id="48bd2-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="48bd2-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="48bd2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48bd2-109">Properties</span></span>
| <span data-ttu-id="48bd2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48bd2-110">Property</span></span>     | <span data-ttu-id="48bd2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="48bd2-111">Type</span></span>   |<span data-ttu-id="48bd2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="48bd2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48bd2-113">type</span><span class="sxs-lookup"><span data-stu-id="48bd2-113">type</span></span>|<span data-ttu-id="48bd2-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48bd2-114">String</span></span>|<span data-ttu-id="48bd2-115">O tipo de fonte de dados.</span><span class="sxs-lookup"><span data-stu-id="48bd2-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
