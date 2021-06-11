---
title: Tipo de recurso outOfOfficeSettings
description: Representa as informações de acesso ao telefone para uma reunião online.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13f826babea1e6f9448d1ecb9b8100baaf962b20
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896631"
---
# <a name="outofofficesettings-resource-type"></a><span data-ttu-id="dfa9c-103">Tipo de recurso outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="dfa9c-103">outOfOfficeSettings resource type</span></span>

<span data-ttu-id="dfa9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfa9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa9c-105">Representa as configurações fora do escritório relacionadas à [presença](presence.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dfa9c-105">Represents the out of office settings related to the [presence](presence.md) of a user.</span></span>

## <a name="properties"></a><span data-ttu-id="dfa9c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfa9c-106">Properties</span></span>

| <span data-ttu-id="dfa9c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfa9c-107">Property</span></span>            | <span data-ttu-id="dfa9c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfa9c-108">Type</span></span>    | <span data-ttu-id="dfa9c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfa9c-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="dfa9c-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="dfa9c-110">message</span></span>           | <span data-ttu-id="dfa9c-111">String</span><span class="sxs-lookup"><span data-stu-id="dfa9c-111">String</span></span>  | <span data-ttu-id="dfa9c-112">A mensagem fora do escritório que o usuário configurou no cliente Outlook (Respostas Automáticas (Sem Office)) ou o cliente Teams (Agendar sem escritório).</span><span class="sxs-lookup"><span data-stu-id="dfa9c-112">The out of office message that the user configured on Outlook client (Automatic Replies (Out of Office)) or the Teams client (Schedule out of office).</span></span> |
| <span data-ttu-id="dfa9c-113">isOutOfOffice</span><span class="sxs-lookup"><span data-stu-id="dfa9c-113">isOutOfOffice</span></span>      | <span data-ttu-id="dfa9c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfa9c-114">Boolean</span></span>  | <span data-ttu-id="dfa9c-115">True se:</span><span class="sxs-lookup"><span data-stu-id="dfa9c-115">True if either:</span></span></br><ul><li><span data-ttu-id="dfa9c-116">Atualmente, ele está na janela de tempo fora do escritório configurada no Outlook ou Teams cliente.</span><span class="sxs-lookup"><span data-stu-id="dfa9c-116">It is currently in the out of office time window configured on the Outlook or Teams client.</span></span></li><li><span data-ttu-id="dfa9c-117">Atualmente, há um evento no calendário do usuário marcado como Show as Out of Office</span><span class="sxs-lookup"><span data-stu-id="dfa9c-117">There is currently an event on the user's calendar that's marked as Show as Out of Office</span></span></li></ul></br><span data-ttu-id="dfa9c-118">Caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="dfa9c-118">Otherwise, false.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dfa9c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfa9c-119">JSON representation</span></span>

<span data-ttu-id="dfa9c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfa9c-120">The following is a JSON representation of the resource.</span></span>

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
