---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.
localization_priority: Normal
ms.openlocfilehash: 5286334378aa5d208cf171ecab0bdc1777a4073b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871222"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="c9b49-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="c9b49-103">emailAddress resource type</span></span>

> <span data-ttu-id="c9b49-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9b49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9b49-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9b49-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9b49-106">Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.</span><span class="sxs-lookup"><span data-stu-id="c9b49-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="c9b49-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9b49-107">Properties</span></span>
| <span data-ttu-id="c9b49-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9b49-108">Property</span></span>     | <span data-ttu-id="c9b49-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9b49-109">Type</span></span>   |<span data-ttu-id="c9b49-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9b49-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9b49-111">address</span><span class="sxs-lookup"><span data-stu-id="c9b49-111">address</span></span>|<span data-ttu-id="c9b49-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9b49-112">String</span></span>|<span data-ttu-id="c9b49-113">O endereço de email de uma instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c9b49-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="c9b49-114">name</span><span class="sxs-lookup"><span data-stu-id="c9b49-114">name</span></span>|<span data-ttu-id="c9b49-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9b49-115">String</span></span>|<span data-ttu-id="c9b49-116">O nome de exibição de uma instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c9b49-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9b49-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9b49-117">JSON representation</span></span>

<span data-ttu-id="c9b49-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c9b49-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
