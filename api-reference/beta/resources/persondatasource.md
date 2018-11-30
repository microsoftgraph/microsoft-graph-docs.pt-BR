---
title: tipo de recurso de personDataSource
description: Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.
ms.openlocfilehash: 1c5aeb2cbb36398eb3c7184550235fc7194f5e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035319"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="1dfda-103">tipo de recurso de personDataSource</span><span class="sxs-lookup"><span data-stu-id="1dfda-103">personDataSource resource type</span></span>

> <span data-ttu-id="1dfda-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1dfda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dfda-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1dfda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1dfda-106">Representa as fontes de que dados do usuário provêm, como o diretório e os contatos do Outlook.</span><span class="sxs-lookup"><span data-stu-id="1dfda-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dfda-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dfda-107">JSON representation</span></span>

<span data-ttu-id="1dfda-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1dfda-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1dfda-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dfda-109">Properties</span></span>
| <span data-ttu-id="1dfda-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dfda-110">Property</span></span>     | <span data-ttu-id="1dfda-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dfda-111">Type</span></span>   |<span data-ttu-id="1dfda-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dfda-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dfda-113">type</span><span class="sxs-lookup"><span data-stu-id="1dfda-113">type</span></span>|<span data-ttu-id="1dfda-114">String</span><span class="sxs-lookup"><span data-stu-id="1dfda-114">String</span></span>|<span data-ttu-id="1dfda-115">O tipo de fonte de dados.</span><span class="sxs-lookup"><span data-stu-id="1dfda-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->