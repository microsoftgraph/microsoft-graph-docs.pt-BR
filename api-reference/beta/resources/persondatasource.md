---
title: tipo de recurso de personDataSource
description: Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.
localization_priority: Normal
ms.openlocfilehash: 80e61bd1cd91c0b2a780936a5a311b0916743a17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824966"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="b1763-103">tipo de recurso de personDataSource</span><span class="sxs-lookup"><span data-stu-id="b1763-103">personDataSource resource type</span></span>

> <span data-ttu-id="b1763-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1763-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1763-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1763-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1763-106">Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b1763-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1763-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1763-107">JSON representation</span></span>

<span data-ttu-id="b1763-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b1763-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b1763-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1763-109">Properties</span></span>
| <span data-ttu-id="b1763-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1763-110">Property</span></span>     | <span data-ttu-id="b1763-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1763-111">Type</span></span>   |<span data-ttu-id="b1763-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1763-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1763-113">type</span><span class="sxs-lookup"><span data-stu-id="b1763-113">type</span></span>|<span data-ttu-id="b1763-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1763-114">String</span></span>|<span data-ttu-id="b1763-115">O tipo de fonte de dados.</span><span class="sxs-lookup"><span data-stu-id="b1763-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
