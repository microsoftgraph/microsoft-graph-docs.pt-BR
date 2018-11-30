---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: a6b83627d86bbb35357f03dbee3605c6fb1df7a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040114"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="4b35a-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="4b35a-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="4b35a-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b35a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b35a-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b35a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b35a-105">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b35a-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b35a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b35a-106">JSON representation</span></span>

<span data-ttu-id="4b35a-107">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="4b35a-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="4b35a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b35a-108">Properties</span></span>

| <span data-ttu-id="4b35a-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4b35a-109">Property name</span></span> | <span data-ttu-id="4b35a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b35a-110">Type</span></span>    | <span data-ttu-id="4b35a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b35a-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="4b35a-112">**default**</span><span class="sxs-lookup"><span data-stu-id="4b35a-112">**default**</span></span>   | <span data-ttu-id="4b35a-113">booliano</span><span class="sxs-lookup"><span data-stu-id="4b35a-113">boolean</span></span> | <span data-ttu-id="4b35a-114">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="4b35a-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="4b35a-115">**position**</span><span class="sxs-lookup"><span data-stu-id="4b35a-115">**position**</span></span>  | <span data-ttu-id="4b35a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4b35a-116">Int32</span></span>   | <span data-ttu-id="4b35a-117">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b35a-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
