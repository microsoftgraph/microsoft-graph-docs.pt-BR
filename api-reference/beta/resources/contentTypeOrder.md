---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ad25ececa9a32a1aaab7f25bf909f7e1ef640dec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825750"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="ff6a7-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="ff6a7-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="ff6a7-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff6a7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff6a7-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff6a7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff6a7-105">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff6a7-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff6a7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff6a7-106">JSON representation</span></span>

<span data-ttu-id="ff6a7-107">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="ff6a7-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="ff6a7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff6a7-108">Properties</span></span>

| <span data-ttu-id="ff6a7-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ff6a7-109">Property name</span></span> | <span data-ttu-id="ff6a7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff6a7-110">Type</span></span>    | <span data-ttu-id="ff6a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff6a7-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="ff6a7-112">**default**</span><span class="sxs-lookup"><span data-stu-id="ff6a7-112">**default**</span></span>   | <span data-ttu-id="ff6a7-113">booliano</span><span class="sxs-lookup"><span data-stu-id="ff6a7-113">boolean</span></span> | <span data-ttu-id="ff6a7-114">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="ff6a7-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="ff6a7-115">**position**</span><span class="sxs-lookup"><span data-stu-id="ff6a7-115">**position**</span></span>  | <span data-ttu-id="ff6a7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ff6a7-116">Int32</span></span>   | <span data-ttu-id="ff6a7-117">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff6a7-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
