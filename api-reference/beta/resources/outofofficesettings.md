---
title: Tipo de recurso outOfOfficeSettings
description: Representa informações de acesso telefônico para uma reunião online.
author: elvinyang-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e3e179ec752cfffc4ae4711d9fd0bc541f1506d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796716"
---
# <a name="outofofficesettings-resource-type"></a><span data-ttu-id="04f8e-103">Tipo de recurso outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="04f8e-103">outOfOfficeSettings resource type</span></span>

<span data-ttu-id="04f8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04f8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04f8e-105">Representa as configurações de fora do escritório relacionadas [à presença](presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="04f8e-105">Represents the out of office settings related to the [presence](presence.md) of a user.</span></span>

## <a name="properties"></a><span data-ttu-id="04f8e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04f8e-106">Properties</span></span>

| <span data-ttu-id="04f8e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04f8e-107">Property</span></span>            | <span data-ttu-id="04f8e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="04f8e-108">Type</span></span>    | <span data-ttu-id="04f8e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="04f8e-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="04f8e-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="04f8e-110">message</span></span>           | <span data-ttu-id="04f8e-111">String</span><span class="sxs-lookup"><span data-stu-id="04f8e-111">String</span></span>  | <span data-ttu-id="04f8e-112">A mensagem de saída que o usuário configurou no cliente do Outlook (Respostas Automáticas (Fora do Escritório)) ou no cliente do Teams (Agendamento de saída do escritório).</span><span class="sxs-lookup"><span data-stu-id="04f8e-112">The out of office message that the user configured on Outlook client (Automatic Replies (Out of Office)) or the Teams client (Schedule out of office).</span></span> |
| <span data-ttu-id="04f8e-113">isOutOfOffice</span><span class="sxs-lookup"><span data-stu-id="04f8e-113">isOutOfOffice</span></span>      | <span data-ttu-id="04f8e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f8e-114">Boolean</span></span>  | <span data-ttu-id="04f8e-115">True se:</span><span class="sxs-lookup"><span data-stu-id="04f8e-115">True if either:</span></span></br><ul><li><span data-ttu-id="04f8e-116">Atualmente, ele está na janela de tempo de não escritório configurada no cliente do Outlook ou do Teams.</span><span class="sxs-lookup"><span data-stu-id="04f8e-116">It is currently in the out of office time window configured on the Outlook or Teams client.</span></span></li><li><span data-ttu-id="04f8e-117">Atualmente, há um evento no calendário do usuário marcado como Show as Out of Office</span><span class="sxs-lookup"><span data-stu-id="04f8e-117">There is currently an event on the user's calendar that's marked as Show as Out of Office</span></span></li></ul></br><span data-ttu-id="04f8e-118">Caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="04f8e-118">Otherwise, false.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04f8e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04f8e-119">JSON representation</span></span>

<span data-ttu-id="04f8e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04f8e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.outOfOfficeSettings"
}-->
```json
{
  "message": "String",
  "isOutOfOffice": "Boolean"
}
```
