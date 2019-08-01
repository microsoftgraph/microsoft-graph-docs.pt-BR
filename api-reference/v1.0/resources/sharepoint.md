---
title: Trabalhar com sites do SharePoint no Microsoft Graph
description: 'A API do SharePoint no Microsoft Graph oferece suporte aos seguintes cenários principais:'
localization_priority: Priority
ms.prod: sharepoint
author: ''
doc_type: conceptualPageType
ms.openlocfilehash: b276193418573cd93baa8459564d22dde73e8bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034269"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a><span data-ttu-id="1bdad-103">Trabalhar com sites do SharePoint no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1bdad-103">Working with SharePoint sites in Microsoft Graph</span></span>

<span data-ttu-id="1bdad-104">A API do SharePoint no Microsoft Graph suporta os seguintes cenários principais:</span><span class="sxs-lookup"><span data-stu-id="1bdad-104">The SharePoint API in Microsoft Graph supports the following core scenarios:</span></span>

* <span data-ttu-id="1bdad-105">Acesso aos **sites**, **lists** e **drives** do SharePoint (bibliotecas de documentos)</span><span class="sxs-lookup"><span data-stu-id="1bdad-105">Access to SharePoint **sites**, **lists**, and **drives** (document libraries)</span></span>
* <span data-ttu-id="1bdad-106">Suporte somente leitura para recursos de **site** (nenhuma capacidade de criar novos sites)</span><span class="sxs-lookup"><span data-stu-id="1bdad-106">Read-only support for **site** resources (no ability to create new sites)</span></span>
* <span data-ttu-id="1bdad-107">Suporte a leitura e gravação para **lists**, **listItems** e **driveItems**</span><span class="sxs-lookup"><span data-stu-id="1bdad-107">Read-write support for **lists**, **listItems**, and **driveItems**</span></span>
* <span data-ttu-id="1bdad-108">Lidar com recursos por ID do SharePoint, URL ou caminho relativo</span><span class="sxs-lookup"><span data-stu-id="1bdad-108">Address resources by SharePoint ID, URL, or relative path</span></span>

<span data-ttu-id="1bdad-109">A API do SharePoint expõe três tipos de recursos principais:</span><span class="sxs-lookup"><span data-stu-id="1bdad-109">The SharePoint API exposes three major resource types:</span></span>

* <span data-ttu-id="1bdad-110">[Site](site.md) _(objeto de nível superior)_</span><span class="sxs-lookup"><span data-stu-id="1bdad-110">[Site](site.md) _(top-level object)_</span></span>
* [<span data-ttu-id="1bdad-111">Lista</span><span class="sxs-lookup"><span data-stu-id="1bdad-111">List</span></span>](list.md)
* [<span data-ttu-id="1bdad-112">ListItem</span><span class="sxs-lookup"><span data-stu-id="1bdad-112">ListItem</span></span>](listitem.md)

<span data-ttu-id="1bdad-113">A seguir está um exemplo de um recurso listItem.</span><span class="sxs-lookup"><span data-stu-id="1bdad-113">The following is an example of a listItem resource.</span></span>

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

<span data-ttu-id="1bdad-114">Recursos expõem dados de três maneiras diferentes:</span><span class="sxs-lookup"><span data-stu-id="1bdad-114">Resources expose data in three different ways:</span></span>

* <span data-ttu-id="1bdad-115">_Propriedades_ (como **id** e **name**) expõem valores simples.</span><span class="sxs-lookup"><span data-stu-id="1bdad-115">_Properties_ (like **id** and **name**) expose simple values.</span></span>
* <span data-ttu-id="1bdad-116">_Facetas_ (como **campos** e **createdBy**) expõem valores complexos.</span><span class="sxs-lookup"><span data-stu-id="1bdad-116">_Facets_ (like **fields** and **createdBy**) expose complex values.</span></span>
* <span data-ttu-id="1bdad-117">_Referências_ (como **itens**) apontam para conjuntos de outros recursos.</span><span class="sxs-lookup"><span data-stu-id="1bdad-117">_References_ (like **items**) point to collections of other resources.</span></span>

<span data-ttu-id="1bdad-118">Você pode expandir referências na URL com o parâmetro de consulta _expand_; por exemplo, `?expand=fields`.</span><span class="sxs-lookup"><span data-stu-id="1bdad-118">You can expand references in your URL with the _expand_ query parameter; for example, `?expand=fields`.</span></span>
<span data-ttu-id="1bdad-119">Você pode solicitar propriedades e facetas específicas com o parâmetro de consulta _select_; por exemplo, `?select=id,name`.</span><span class="sxs-lookup"><span data-stu-id="1bdad-119">You can request specific properties and facets with the _select_ query parameter; for example, `?select=id,name`.</span></span>
<span data-ttu-id="1bdad-120">Por padrão, a maioria das propriedades e facetas retorna enquanto todas as referências ficam ocultas.</span><span class="sxs-lookup"><span data-stu-id="1bdad-120">By default, most properties and facets are returned while all references are hidden.</span></span>
<span data-ttu-id="1bdad-121">Por questões de eficiência, recomendamos que você especifique _selecionar_ e _expandir_ para só retornar os dados mais importantes para você.</span><span class="sxs-lookup"><span data-stu-id="1bdad-121">For efficiency, we recommend that you specify _select_ and _expand_ to only return the data you care about.</span></span>

## <a name="sharepoint-api-root-resources"></a><span data-ttu-id="1bdad-122">Recursos de raiz da API do SharePoint</span><span class="sxs-lookup"><span data-stu-id="1bdad-122">SharePoint API root resources</span></span>

<span data-ttu-id="1bdad-123">Os exemplos a seguir são relativos a `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="1bdad-123">The following examples are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="1bdad-124">Caminho</span><span class="sxs-lookup"><span data-stu-id="1bdad-124">Path</span></span>                                   | <span data-ttu-id="1bdad-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bdad-125">Description</span></span>
|:---------------------------------------|:------------------------------------
| <span data-ttu-id="1bdad-126">/sites/root</span><span class="sxs-lookup"><span data-stu-id="1bdad-126">/sites/root</span></span>                            | <span data-ttu-id="1bdad-127">[Site][] padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="1bdad-127">Organization's default [site][].</span></span>
| <span data-ttu-id="1bdad-128">/sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="1bdad-128">/sites/{site-id}</span></span>                       | <span data-ttu-id="1bdad-129">Acessar um [site][] específico por sua identificação.</span><span class="sxs-lookup"><span data-stu-id="1bdad-129">Access a specific [site][] by its ID.</span></span>
| <span data-ttu-id="1bdad-130">/sites/{site-id}/drive</span><span class="sxs-lookup"><span data-stu-id="1bdad-130">/sites/{site-id}/drive</span></span>                 | <span data-ttu-id="1bdad-131">Acessar a [unidade](drive.md) padrão (biblioteca de documentos) desse [site][].</span><span class="sxs-lookup"><span data-stu-id="1bdad-131">Access the default [drive](drive.md) (document library) for the given [site][].</span></span>
| <span data-ttu-id="1bdad-132">/sites/{site-id}/drives</span><span class="sxs-lookup"><span data-stu-id="1bdad-132">/sites/{site-id}/drives</span></span>                | <span data-ttu-id="1bdad-133">Enumerar as [unidades](drive.md) (bibliotecas de documentos) no [site][].</span><span class="sxs-lookup"><span data-stu-id="1bdad-133">Enumerate the [drives](drive.md) (document libraries) under the [site][].</span></span>
| <span data-ttu-id="1bdad-134">/sites/{site-id}/sites</span><span class="sxs-lookup"><span data-stu-id="1bdad-134">/sites/{site-id}/sites</span></span>                 | <span data-ttu-id="1bdad-135">Enumerar os subsites no [site][].</span><span class="sxs-lookup"><span data-stu-id="1bdad-135">Enumerate the sub-sites under the [site][].</span></span>
| <span data-ttu-id="1bdad-136">/sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="1bdad-136">/sites/{site-id}/lists</span></span>                 | <span data-ttu-id="1bdad-137">Enumerar as [listas](list.md) sob o [site](site.md).</span><span class="sxs-lookup"><span data-stu-id="1bdad-137">Enumerate the [lists](list.md) under the [site](site.md).</span></span>
| <span data-ttu-id="1bdad-138">/sites/{site-id}/lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="1bdad-138">/sites/{site-id}/lists/{list-id}/items</span></span> | <span data-ttu-id="1bdad-139">Enumerar [listItems](listitem.md) sob a [lista](list.md).</span><span class="sxs-lookup"><span data-stu-id="1bdad-139">Enumerate the [listItems](listitem.md) under the [list](list.md).</span></span>
| <span data-ttu-id="1bdad-140">/groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="1bdad-140">/groups/{group-id}/sites/root</span></span>          | <span data-ttu-id="1bdad-141">Acesse um [site][] de equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="1bdad-141">Access a group's team [site][].</span></span>

<span data-ttu-id="1bdad-p102">Sites também podem ser tratados pelo caminho usando o nome de host do SharePoint, seguido por dois pontos e o caminho relativo para o site. Opcionalmente, você pode fazer a transição para lidar com o modelo de recurso colocando outros dois pontos no final.</span><span class="sxs-lookup"><span data-stu-id="1bdad-p102">Sites can also be addressed by path by using the SharePoint hostname, followed by a colon and the relative path to the site. You can optionally transition back to addressing the resource model by putting another colon at the end.</span></span>

| <span data-ttu-id="1bdad-144">Caminho</span><span class="sxs-lookup"><span data-stu-id="1bdad-144">Path</span></span>                                           | <span data-ttu-id="1bdad-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bdad-145">Description</span></span>
|:-----------------------------------------------|:-----------------------------------
| <span data-ttu-id="1bdad-146">/sites/contoso.sharepoint.com:/teams/hr</span><span class="sxs-lookup"><span data-stu-id="1bdad-146">/sites/contoso.sharepoint.com:/teams/hr</span></span>        | <span data-ttu-id="1bdad-147">O site associado comhttps://contoso.sharepoint.com/teams/hr</span><span class="sxs-lookup"><span data-stu-id="1bdad-147">The site associated with https://contoso.sharepoint.com/teams/hr</span></span>
| <span data-ttu-id="1bdad-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span><span class="sxs-lookup"><span data-stu-id="1bdad-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span></span> | <span data-ttu-id="1bdad-149">Acessar a [unidade](drive.md) padrão desse.</span><span class="sxs-lookup"><span data-stu-id="1bdad-149">Access the default [drive](drive.md) for this site.</span></span>

## <a name="note-for-existing-sharepoint-developers"></a><span data-ttu-id="1bdad-150">Observação para desenvolvedores do SharePoint existentes</span><span class="sxs-lookup"><span data-stu-id="1bdad-150">Note for existing SharePoint developers</span></span>

<span data-ttu-id="1bdad-151">A API do Microsoft Graph do SharePoint tem algumas diferenças essenciais das APIs CSOM.</span><span class="sxs-lookup"><span data-stu-id="1bdad-151">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs.</span></span>
<span data-ttu-id="1bdad-152">Os recurso do [site][] mapeia para `SPWeb`.</span><span class="sxs-lookup"><span data-stu-id="1bdad-152">The [site][] resource maps to `SPWeb`.</span></span>
<span data-ttu-id="1bdad-153">O [site][] (`SPWeb`) raiz em um conjunto de sites tem uma faceta [siteCollection](sitecollection.md), que contém informações sobre `SPSite`.</span><span class="sxs-lookup"><span data-stu-id="1bdad-153">The root [site][] (`SPWeb`) in a site collection has a [siteCollection](sitecollection.md) facet, which contains information about the `SPSite`.</span></span>
<span data-ttu-id="1bdad-154">Como as IDs de sites são exclusivas penas em sua coleção de site, abordar um site por ID requer o fornecimento do identificador de coleção de site e identificador de site.</span><span class="sxs-lookup"><span data-stu-id="1bdad-154">Because IDs for sites are only unique within their site collection, addressing a site by ID requires providing both the site collection identifier and the site identifier.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
<span data-ttu-id="1bdad-155">Uma URL construída com apenas o nome do host apontará para o site raiz (`SPWeb`) na coleção de sites padrão.</span><span class="sxs-lookup"><span data-stu-id="1bdad-155">A URL constructed with only the hostname will point to the root site (`SPWeb`) in the default site collection.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

<span data-ttu-id="1bdad-156">Uma URL construída apenas com o nome do host e ID de siteCollection (`SPSite`) apontará o site raiz (`SPWeb`) na coleção de sites determinada.</span><span class="sxs-lookup"><span data-stu-id="1bdad-156">A URL constructed with only the hostname and siteCollection (`SPSite`) ID will point to the root site (`SPWeb`) in the given site collection.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
