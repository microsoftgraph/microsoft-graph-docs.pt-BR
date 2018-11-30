---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
ms.openlocfilehash: 00e09b064a083aa72316838c213f9c84e1139a19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039808"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="f684b-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="f684b-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="f684b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f684b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f684b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f684b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f684b-106">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f684b-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="f684b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f684b-107">Properties</span></span>
| <span data-ttu-id="f684b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f684b-108">Property</span></span>     | <span data-ttu-id="f684b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f684b-109">Type</span></span>   |<span data-ttu-id="f684b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f684b-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f684b-111">name</span><span class="sxs-lookup"><span data-stu-id="f684b-111">name</span></span> | <span data-ttu-id="f684b-112">string</span><span class="sxs-lookup"><span data-stu-id="f684b-112">string</span></span> | <span data-ttu-id="f684b-113">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f684b-113">The name of a time zone.</span></span> <span data-ttu-id="f684b-114">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="f684b-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f684b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f684b-115">JSON representation</span></span>

<span data-ttu-id="f684b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f684b-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->