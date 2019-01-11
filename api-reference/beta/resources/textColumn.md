---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 87a5e27544a49613d1d1e44cd6f3e0e3b7fcf8c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822565"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="bddc7-102">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="bddc7-102">TextColumn resource type</span></span>

> <span data-ttu-id="bddc7-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bddc7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bddc7-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bddc7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bddc7-105">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="bddc7-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bddc7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bddc7-106">JSON representation</span></span>

<span data-ttu-id="bddc7-107">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="bddc7-107">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="bddc7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bddc7-108">Properties</span></span>

| <span data-ttu-id="bddc7-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bddc7-109">Property name</span></span>                   | <span data-ttu-id="bddc7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bddc7-110">Type</span></span>   | <span data-ttu-id="bddc7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bddc7-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="bddc7-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="bddc7-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="bddc7-113">string</span><span class="sxs-lookup"><span data-stu-id="bddc7-113">string</span></span> | <span data-ttu-id="bddc7-114">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="bddc7-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="bddc7-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="bddc7-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="bddc7-116">string</span><span class="sxs-lookup"><span data-stu-id="bddc7-116">string</span></span> | <span data-ttu-id="bddc7-117">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="bddc7-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="bddc7-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="bddc7-118">**linesForEditing**</span></span>             | <span data-ttu-id="bddc7-119">int</span><span class="sxs-lookup"><span data-stu-id="bddc7-119">int</span></span>    | <span data-ttu-id="bddc7-120">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="bddc7-120">The size of the text box.</span></span>
| <span data-ttu-id="bddc7-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="bddc7-121">**maxLength**</span></span>                   | <span data-ttu-id="bddc7-122">int</span><span class="sxs-lookup"><span data-stu-id="bddc7-122">int</span></span>    | <span data-ttu-id="bddc7-123">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="bddc7-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="bddc7-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="bddc7-124">**textType**</span></span>                    | <span data-ttu-id="bddc7-125">string</span><span class="sxs-lookup"><span data-stu-id="bddc7-125">string</span></span> | <span data-ttu-id="bddc7-126">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="bddc7-126">The type of text being stored.</span></span> <span data-ttu-id="bddc7-127">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="bddc7-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
