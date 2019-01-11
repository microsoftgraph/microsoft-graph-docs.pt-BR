---
title: tipo de recurso de synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
ms.openlocfilehash: cc6b58444ac56303bfd2e41f1fcae17658f6aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847240"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="f0569-103">tipo de recurso de synchronizationError</span><span class="sxs-lookup"><span data-stu-id="f0569-103">synchronizationError resource type</span></span>

> <span data-ttu-id="f0569-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0569-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0569-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0569-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0569-106">Representa um erro que ocorreu durante o processo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f0569-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="f0569-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0569-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="f0569-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0569-108">Property</span></span>     | <span data-ttu-id="f0569-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0569-109">Type</span></span>   |<span data-ttu-id="f0569-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0569-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0569-111">código</span><span class="sxs-lookup"><span data-stu-id="f0569-111">code</span></span>|<span data-ttu-id="f0569-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0569-112">String</span></span>||
|<span data-ttu-id="f0569-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="f0569-113">message</span></span>|<span data-ttu-id="f0569-114">String</span><span class="sxs-lookup"><span data-stu-id="f0569-114">String</span></span>||
|<span data-ttu-id="f0569-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="f0569-115">tenantActionable</span></span>|<span data-ttu-id="f0569-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0569-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="f0569-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0569-117">JSON representation</span></span>

<span data-ttu-id="f0569-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0569-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
