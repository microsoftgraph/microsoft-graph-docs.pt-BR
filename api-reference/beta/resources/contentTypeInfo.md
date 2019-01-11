---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: e394d52a5f7ed5e8dce1c61d31d787d62bd36e56
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892334"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="6cb7f-102">Tipo de recurso ContentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="6cb7f-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="6cb7f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6cb7f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cb7f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6cb7f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cb7f-105">O recurso **contentTypeInfo** indica o tipo de conteúdo do SharePoint de um item.</span><span class="sxs-lookup"><span data-stu-id="6cb7f-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6cb7f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cb7f-106">JSON representation</span></span>

<span data-ttu-id="6cb7f-107">Aqui está uma representação JSON de um recurso **contentTypeInfo**.</span><span class="sxs-lookup"><span data-stu-id="6cb7f-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6cb7f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cb7f-108">Properties</span></span>

| <span data-ttu-id="6cb7f-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6cb7f-109">Property name</span></span>  | <span data-ttu-id="6cb7f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cb7f-110">Type</span></span>    | <span data-ttu-id="6cb7f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb7f-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="6cb7f-112">**id**</span><span class="sxs-lookup"><span data-stu-id="6cb7f-112">**id**</span></span>         | <span data-ttu-id="6cb7f-113">string</span><span class="sxs-lookup"><span data-stu-id="6cb7f-113">string</span></span>  | <span data-ttu-id="6cb7f-114">A id do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6cb7f-114">The id of the content type.</span></span>
| <span data-ttu-id="6cb7f-115">**name**</span><span class="sxs-lookup"><span data-stu-id="6cb7f-115">**name**</span></span>       | <span data-ttu-id="6cb7f-116">string</span><span class="sxs-lookup"><span data-stu-id="6cb7f-116">string</span></span>  | <span data-ttu-id="6cb7f-117">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6cb7f-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
