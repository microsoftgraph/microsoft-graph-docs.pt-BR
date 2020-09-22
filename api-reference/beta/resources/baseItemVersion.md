---
author: JeremyKelley
description: O recurso baseItemVersion representa uma versão anterior de um item ou de uma entidade.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0d007d18f6329763fa6a7a426f1f944ef1fb4106
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089725"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="25586-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="25586-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="25586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25586-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25586-105">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="25586-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="25586-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25586-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="25586-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25586-107">Properties</span></span>

|      <span data-ttu-id="25586-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="25586-108">Property name</span></span>       |                         <span data-ttu-id="25586-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="25586-109">Type</span></span>                         |                               <span data-ttu-id="25586-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="25586-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="25586-111">**id**</span><span class="sxs-lookup"><span data-stu-id="25586-111">**id**</span></span>                   | <span data-ttu-id="25586-112">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25586-112">string</span></span>                                               | <span data-ttu-id="25586-113">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="25586-113">The ID of the version.</span></span> <span data-ttu-id="25586-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25586-114">Read-only.</span></span>                                       |
| <span data-ttu-id="25586-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="25586-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="25586-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="25586-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="25586-117">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="25586-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="25586-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25586-118">Read-only.</span></span>        |
| <span data-ttu-id="25586-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="25586-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="25586-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25586-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="25586-121">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="25586-121">Date and time the version was last modified.</span></span> <span data-ttu-id="25586-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25586-122">Read-only.</span></span>                 |
| <span data-ttu-id="25586-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="25586-123">**publication**</span></span>          | [<span data-ttu-id="25586-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="25586-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="25586-125">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="25586-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="25586-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25586-126">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->


