---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 735931e757297bd9846396d6f6c42988d8cb87fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328230"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="8f847-102">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="8f847-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f847-103">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="8f847-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f847-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f847-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8f847-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f847-105">Properties</span></span>

|      <span data-ttu-id="8f847-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8f847-106">Property name</span></span>       |                         <span data-ttu-id="8f847-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f847-107">Type</span></span>                         |                               <span data-ttu-id="8f847-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f847-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="8f847-109">**id**</span><span class="sxs-lookup"><span data-stu-id="8f847-109">**id**</span></span>                   | <span data-ttu-id="8f847-110">string</span><span class="sxs-lookup"><span data-stu-id="8f847-110">string</span></span>                                               | <span data-ttu-id="8f847-111">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="8f847-111">The ID of the version.</span></span> <span data-ttu-id="8f847-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f847-112">Read-only.</span></span>                                       |
| <span data-ttu-id="8f847-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="8f847-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="8f847-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8f847-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="8f847-115">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8f847-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="8f847-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f847-116">Read-only.</span></span>        |
| <span data-ttu-id="8f847-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8f847-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="8f847-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f847-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="8f847-119">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8f847-119">Date and time the version was last modified.</span></span> <span data-ttu-id="8f847-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f847-120">Read-only.</span></span>                 |
| <span data-ttu-id="8f847-121">**publication**</span><span class="sxs-lookup"><span data-stu-id="8f847-121">**publication**</span></span>          | [<span data-ttu-id="8f847-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="8f847-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="8f847-123">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="8f847-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="8f847-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f847-124">Read-only.</span></span> |


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
