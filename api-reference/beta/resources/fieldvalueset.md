---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: ed10b586ee55ccd32e81b03bdc6359ee13605877
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480163"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="636ad-102">Recurso de FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="636ad-102">FieldValueSet resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="636ad-103">Representa os valores de coluna em um recurso [listItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="636ad-103">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="636ad-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="636ad-104">JSON representation</span></span>

<span data-ttu-id="636ad-105">Aqui está uma representação JSON de um recurso **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="636ad-105">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="636ad-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="636ad-106">Properties</span></span>

<span data-ttu-id="636ad-107">Cada campo de usuário visível em **listItem** é retornado como um par de nome e valor em **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="636ad-107">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="636ad-108">O exemplo acima é para uma lista que contém quatro colunas **Autor**, **Nome**, **Cor** e **Quantidade**.</span><span class="sxs-lookup"><span data-stu-id="636ad-108">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="636ad-109">Campos de pesquisa (como `Author` acima) não são retornados por padrão.</span><span class="sxs-lookup"><span data-stu-id="636ad-109">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="636ad-110">Em vez disso, o servidor retorna um campo 'LookupId' (como `AuthorLookupId` acima) referenciando o listItem direcionado na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="636ad-110">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="636ad-111">O nome do campo 'LookupId' é o nome do campo original seguido de `LookupId`.</span><span class="sxs-lookup"><span data-stu-id="636ad-111">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="636ad-112">Até 12 campos de pesquisa podem ser solicitados em uma única consulta.</span><span class="sxs-lookup"><span data-stu-id="636ad-112">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="636ad-113">O servidor retornará valores de pesquisa se sua solicitação incluir uma instrução `select` com os campos necessários.</span><span class="sxs-lookup"><span data-stu-id="636ad-113">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="636ad-114">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="636ad-114">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="636ad-115">você pode solicitar até 12 campos de pesquisa em uma única consulta, além de qualquer número de campos normais.</span><span class="sxs-lookup"><span data-stu-id="636ad-115">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/fieldvalueset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
