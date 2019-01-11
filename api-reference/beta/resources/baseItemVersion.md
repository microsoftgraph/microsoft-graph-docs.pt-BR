---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 9a5181e9cbc089832e8f73e0b8222ca63b69ca30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894478"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="3e881-102">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="3e881-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="3e881-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e881-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e881-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e881-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e881-105">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="3e881-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3e881-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e881-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3e881-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e881-107">Properties</span></span>

|      <span data-ttu-id="3e881-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3e881-108">Property name</span></span>       |                         <span data-ttu-id="3e881-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e881-109">Type</span></span>                         |                               <span data-ttu-id="3e881-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e881-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="3e881-111">**id**</span><span class="sxs-lookup"><span data-stu-id="3e881-111">**id**</span></span>                   | <span data-ttu-id="3e881-112">string</span><span class="sxs-lookup"><span data-stu-id="3e881-112">string</span></span>                                               | <span data-ttu-id="3e881-113">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="3e881-113">The ID of the version.</span></span> <span data-ttu-id="3e881-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e881-114">Read-only.</span></span>                                       |
| <span data-ttu-id="3e881-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="3e881-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="3e881-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3e881-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="3e881-117">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3e881-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="3e881-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e881-118">Read-only.</span></span>        |
| <span data-ttu-id="3e881-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="3e881-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="3e881-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e881-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="3e881-121">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3e881-121">Date and time the version was last modified.</span></span> <span data-ttu-id="3e881-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e881-122">Read-only.</span></span>                 |
| <span data-ttu-id="3e881-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="3e881-123">**publication**</span></span>          | [<span data-ttu-id="3e881-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="3e881-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="3e881-125">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="3e881-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="3e881-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e881-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
