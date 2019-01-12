---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c06849a73f4246653b8d78dcd392c4e4f6686a46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932788"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="308e6-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="308e6-103">emailAddress resource type</span></span>

> <span data-ttu-id="308e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="308e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="308e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="308e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="308e6-106">Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.</span><span class="sxs-lookup"><span data-stu-id="308e6-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="308e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="308e6-107">Properties</span></span>
| <span data-ttu-id="308e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="308e6-108">Property</span></span>     | <span data-ttu-id="308e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="308e6-109">Type</span></span>   |<span data-ttu-id="308e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="308e6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="308e6-111">address</span><span class="sxs-lookup"><span data-stu-id="308e6-111">address</span></span>|<span data-ttu-id="308e6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="308e6-112">String</span></span>|<span data-ttu-id="308e6-113">O endereço de email de uma instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="308e6-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="308e6-114">name</span><span class="sxs-lookup"><span data-stu-id="308e6-114">name</span></span>|<span data-ttu-id="308e6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="308e6-115">String</span></span>|<span data-ttu-id="308e6-116">O nome de exibição de uma instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="308e6-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="308e6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="308e6-117">JSON representation</span></span>

<span data-ttu-id="308e6-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="308e6-118">Here is a JSON representation of the resource</span></span>

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
