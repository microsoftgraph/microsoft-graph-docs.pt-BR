---
author: JeremyKelley
description: O recurso baseItemVersion representa uma versão anterior de um item ou de uma entidade.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d5265004eac969fa827e5456183180a4c6434f96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974231"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="077dc-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="077dc-103">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="077dc-104">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="077dc-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="077dc-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="077dc-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="077dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="077dc-106">Properties</span></span>

|      <span data-ttu-id="077dc-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="077dc-107">Property name</span></span>       |                         <span data-ttu-id="077dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="077dc-108">Type</span></span>                         |                               <span data-ttu-id="077dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="077dc-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="077dc-110">**id**</span><span class="sxs-lookup"><span data-stu-id="077dc-110">**id**</span></span>                   | <span data-ttu-id="077dc-111">string</span><span class="sxs-lookup"><span data-stu-id="077dc-111">string</span></span>                                               | <span data-ttu-id="077dc-112">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="077dc-112">The ID of the version.</span></span> <span data-ttu-id="077dc-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="077dc-113">Read-only.</span></span>                                       |
| <span data-ttu-id="077dc-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="077dc-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="077dc-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="077dc-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="077dc-116">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="077dc-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="077dc-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="077dc-117">Read-only.</span></span>        |
| <span data-ttu-id="077dc-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="077dc-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="077dc-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="077dc-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="077dc-120">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="077dc-120">Date and time the version was last modified.</span></span> <span data-ttu-id="077dc-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="077dc-121">Read-only.</span></span>                 |
| <span data-ttu-id="077dc-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="077dc-122">**publication**</span></span>          | [<span data-ttu-id="077dc-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="077dc-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="077dc-124">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="077dc-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="077dc-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="077dc-125">Read-only.</span></span> |


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
