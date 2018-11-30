---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037455"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="e5385-102">Tipo de recurso ContentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="e5385-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="e5385-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5385-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5385-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5385-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5385-105">O recurso **contentTypeInfo** indica o tipo de conteúdo do SharePoint de um item.</span><span class="sxs-lookup"><span data-stu-id="e5385-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5385-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5385-106">JSON representation</span></span>

<span data-ttu-id="e5385-107">Aqui está uma representação JSON de um recurso **contentTypeInfo**.</span><span class="sxs-lookup"><span data-stu-id="e5385-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e5385-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5385-108">Properties</span></span>

| <span data-ttu-id="e5385-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e5385-109">Property name</span></span>  | <span data-ttu-id="e5385-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5385-110">Type</span></span>    | <span data-ttu-id="e5385-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5385-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="e5385-112">**id**</span><span class="sxs-lookup"><span data-stu-id="e5385-112">**id**</span></span>         | <span data-ttu-id="e5385-113">string</span><span class="sxs-lookup"><span data-stu-id="e5385-113">string</span></span>  | <span data-ttu-id="e5385-114">A id do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e5385-114">The id of the content type.</span></span>
| <span data-ttu-id="e5385-115">**name**</span><span class="sxs-lookup"><span data-stu-id="e5385-115">**name**</span></span>       | <span data-ttu-id="e5385-116">string</span><span class="sxs-lookup"><span data-stu-id="e5385-116">string</span></span>  | <span data-ttu-id="e5385-117">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e5385-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
