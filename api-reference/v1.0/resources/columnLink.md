---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: cdae360afb6e626ee481a7e98ed5f90e657203b2
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265117"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="aba8a-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="aba8a-102">ColumnLink resource type</span></span>

<span data-ttu-id="aba8a-103">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="aba8a-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="aba8a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aba8a-105">JSON representation</span></span>

<span data-ttu-id="aba8a-106">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="aba8a-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="aba8a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aba8a-107">Properties</span></span>

| <span data-ttu-id="aba8a-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="aba8a-108">Property name</span></span> | <span data-ttu-id="aba8a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="aba8a-109">Type</span></span>   | <span data-ttu-id="aba8a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aba8a-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="aba8a-111">**id**</span><span class="sxs-lookup"><span data-stu-id="aba8a-111">**id**</span></span>        | <span data-ttu-id="aba8a-112">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba8a-112">string</span></span> | <span data-ttu-id="aba8a-113">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="aba8a-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="aba8a-114">**name**</span><span class="sxs-lookup"><span data-stu-id="aba8a-114">**name**</span></span>      | <span data-ttu-id="aba8a-115">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="aba8a-115">string</span></span> | <span data-ttu-id="aba8a-116">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="aba8a-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
