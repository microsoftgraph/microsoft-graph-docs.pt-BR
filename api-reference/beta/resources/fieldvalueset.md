---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: 7108c47aecf842f31382ad170fbb058a1aabb39d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815656"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="cd3ca-102">Recurso de FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="cd3ca-102">FieldValueSet resource</span></span>

> <span data-ttu-id="cd3ca-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd3ca-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd3ca-105">Representa os valores de coluna em um recurso [listItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="cd3ca-105">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd3ca-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd3ca-106">JSON representation</span></span>

<span data-ttu-id="cd3ca-107">Aqui está uma representação JSON de um recurso **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-107">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="cd3ca-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd3ca-108">Properties</span></span>

<span data-ttu-id="cd3ca-109">Cada campo de usuário visível em **listItem** é retornado como um par de nome e valor em **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-109">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="cd3ca-110">O exemplo acima é para uma lista que contém quatro colunas **Autor**, **Nome**, **Cor** e **Quantidade**.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-110">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="cd3ca-111">Campos de pesquisa (como `Author` acima) não são retornados por padrão.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-111">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="cd3ca-112">Em vez disso, o servidor retorna um campo 'LookupId' (como `AuthorLookupId` acima) referenciando o listItem direcionado na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-112">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="cd3ca-113">O nome do campo 'LookupId' é o nome do campo original seguido de `LookupId`.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-113">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="cd3ca-114">Até 12 campos de pesquisa podem ser solicitados em uma única consulta.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-114">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="cd3ca-115">O servidor retornará valores de pesquisa se sua solicitação incluir uma instrução `select` com os campos necessários.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-115">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="cd3ca-116">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="cd3ca-116">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="cd3ca-117">você pode solicitar até 12 campos de pesquisa em uma única consulta, além de qualquer número de campos normais.</span><span class="sxs-lookup"><span data-stu-id="cd3ca-117">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
