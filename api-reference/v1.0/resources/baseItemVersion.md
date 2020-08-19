---
title: Tipo de recurso BaseItemVersion
description: O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc432af84b67e1781be4193a3e8d2bba29ff67a7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808288"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="05176-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="05176-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="05176-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05176-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05176-105">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="05176-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="05176-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05176-106">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="05176-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05176-107">Properties</span></span>

|      <span data-ttu-id="05176-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="05176-108">Property name</span></span>       |                         <span data-ttu-id="05176-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="05176-109">Type</span></span>                         |                               <span data-ttu-id="05176-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="05176-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="05176-111">**id**</span><span class="sxs-lookup"><span data-stu-id="05176-111">**id**</span></span>                   | <span data-ttu-id="05176-112">string</span><span class="sxs-lookup"><span data-stu-id="05176-112">string</span></span>                                               | <span data-ttu-id="05176-113">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="05176-113">The ID of the version.</span></span> <span data-ttu-id="05176-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05176-114">Read-only.</span></span>                                       |
| <span data-ttu-id="05176-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="05176-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="05176-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="05176-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="05176-117">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="05176-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="05176-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05176-118">Read-only.</span></span>        |
| <span data-ttu-id="05176-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="05176-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="05176-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05176-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="05176-121">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="05176-121">Date and time the version was last modified.</span></span> <span data-ttu-id="05176-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05176-122">Read-only.</span></span>                 |
| <span data-ttu-id="05176-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="05176-123">**publication**</span></span>          | [<span data-ttu-id="05176-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="05176-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="05176-125">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="05176-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="05176-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05176-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
