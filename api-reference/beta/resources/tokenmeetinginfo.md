---
title: tipo de recurso de tokenMeetingInfo
description: O tipo de tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9a618906df450ce58f7428a76367e896b315591a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806976"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="7cba3-103">tipo de recurso de tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="7cba3-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="7cba3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7cba3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cba3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7cba3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7cba3-106">O tipo de tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="7cba3-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="7cba3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7cba3-107">Properties</span></span>

| <span data-ttu-id="7cba3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cba3-108">Property</span></span>                     | <span data-ttu-id="7cba3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cba3-109">Type</span></span>    | <span data-ttu-id="7cba3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cba3-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="7cba3-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="7cba3-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="7cba3-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="7cba3-112">Boolean</span></span> | <span data-ttu-id="7cba3-113">Indica se uma conversa pode continuar depois que deixa o host da conversa.</span><span class="sxs-lookup"><span data-stu-id="7cba3-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="7cba3-114">token</span><span class="sxs-lookup"><span data-stu-id="7cba3-114">token</span></span>                        | <span data-ttu-id="7cba3-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cba3-115">String</span></span>  | <span data-ttu-id="7cba3-116">O token de ingresso/ativar a reunião.</span><span class="sxs-lookup"><span data-stu-id="7cba3-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="7cba3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7cba3-117">JSON representation</span></span>

<span data-ttu-id="7cba3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7cba3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="7cba3-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cba3-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
