---
title: tipo de recurso de destinatários
description: Veja a seguir uma representação JSON do recurso
localization_priority: Normal
ms.openlocfilehash: c0afde5b7bd427389b5b81be055781dfaff194e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829579"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="2861e-103">tipo de recurso de destinatários</span><span class="sxs-lookup"><span data-stu-id="2861e-103">recipients resource type</span></span>

> <span data-ttu-id="2861e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2861e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2861e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2861e-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2861e-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2861e-106">JSON representation</span></span>

<span data-ttu-id="2861e-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2861e-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2861e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2861e-108">Properties</span></span>
| <span data-ttu-id="2861e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2861e-109">Property</span></span>     | <span data-ttu-id="2861e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2861e-110">Type</span></span>   |<span data-ttu-id="2861e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2861e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2861e-112">alias</span><span class="sxs-lookup"><span data-stu-id="2861e-112">alias</span></span>|<span data-ttu-id="2861e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2861e-113">String</span></span>||
|<span data-ttu-id="2861e-114">email</span><span class="sxs-lookup"><span data-stu-id="2861e-114">email</span></span>|<span data-ttu-id="2861e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2861e-115">String</span></span>||
|<span data-ttu-id="2861e-116">objectId</span><span class="sxs-lookup"><span data-stu-id="2861e-116">objectId</span></span>|<span data-ttu-id="2861e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2861e-117">String</span></span>||
|<span data-ttu-id="2861e-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="2861e-118">permissionIdentityType</span></span>|<span data-ttu-id="2861e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2861e-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
