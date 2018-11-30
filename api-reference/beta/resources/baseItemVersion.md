---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
ms.openlocfilehash: dfda19af6057bc1d6e1757d24f6a2c99979a8622
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033138"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="73e46-102">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="73e46-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="73e46-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73e46-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73e46-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73e46-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73e46-105">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="73e46-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="73e46-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73e46-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="73e46-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73e46-107">Properties</span></span>

|      <span data-ttu-id="73e46-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="73e46-108">Property name</span></span>       |                         <span data-ttu-id="73e46-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="73e46-109">Type</span></span>                         |                               <span data-ttu-id="73e46-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e46-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="73e46-111">**id**</span><span class="sxs-lookup"><span data-stu-id="73e46-111">**id**</span></span>                   | <span data-ttu-id="73e46-112">string</span><span class="sxs-lookup"><span data-stu-id="73e46-112">string</span></span>                                               | <span data-ttu-id="73e46-113">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="73e46-113">The ID of the version.</span></span> <span data-ttu-id="73e46-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e46-114">Read-only.</span></span>                                       |
| <span data-ttu-id="73e46-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="73e46-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="73e46-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="73e46-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="73e46-117">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="73e46-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="73e46-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e46-118">Read-only.</span></span>        |
| <span data-ttu-id="73e46-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="73e46-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="73e46-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73e46-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="73e46-121">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="73e46-121">Date and time the version was last modified.</span></span> <span data-ttu-id="73e46-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e46-122">Read-only.</span></span>                 |
| <span data-ttu-id="73e46-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="73e46-123">**publication**</span></span>          | [<span data-ttu-id="73e46-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="73e46-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="73e46-125">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="73e46-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="73e46-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e46-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->