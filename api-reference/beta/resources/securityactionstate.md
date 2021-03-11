---
title: Tipo de recurso securityActionState
description: Representa o histórico de alterações de estado securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6a2fecbc05c9987ee8daec8fa017d728a2d03ed3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722087"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="1bff9-103">Tipo de recurso securityActionState</span><span class="sxs-lookup"><span data-stu-id="1bff9-103">securityActionState resource type</span></span>

<span data-ttu-id="1bff9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bff9-105">Representa o histórico de alterações de estado securityAction.</span><span class="sxs-lookup"><span data-stu-id="1bff9-105">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="1bff9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bff9-106">Properties</span></span>

| <span data-ttu-id="1bff9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bff9-107">Property</span></span>     | <span data-ttu-id="1bff9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bff9-108">Type</span></span>        | <span data-ttu-id="1bff9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bff9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1bff9-110">appId</span><span class="sxs-lookup"><span data-stu-id="1bff9-110">appId</span></span>|<span data-ttu-id="1bff9-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bff9-111">String</span></span>|<span data-ttu-id="1bff9-112">A ID do Aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) à ação.</span><span class="sxs-lookup"><span data-stu-id="1bff9-112">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="1bff9-113">O deve ser extraído do token de auth e não inserido `appId` manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="1bff9-113">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="1bff9-114">status</span><span class="sxs-lookup"><span data-stu-id="1bff9-114">status</span></span>|<span data-ttu-id="1bff9-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bff9-115">String</span></span>| <span data-ttu-id="1bff9-116">Status da securityAction nesta atualização.</span><span class="sxs-lookup"><span data-stu-id="1bff9-116">Status of the securityAction in this update.</span></span> <span data-ttu-id="1bff9-117">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="1bff9-117">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="1bff9-118">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bff9-118">updatedDateTime</span></span>|<span data-ttu-id="1bff9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bff9-119">DateTimeOffset</span></span>| <span data-ttu-id="1bff9-120">Timestamp quando actionState foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="1bff9-120">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="1bff9-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1bff9-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1bff9-122">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1bff9-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1bff9-123">user</span><span class="sxs-lookup"><span data-stu-id="1bff9-123">user</span></span>|<span data-ttu-id="1bff9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bff9-124">String</span></span>|<span data-ttu-id="1bff9-125">O nome principal do usuário do usuário que enviou uma atualização (PATCH) à ação.</span><span class="sxs-lookup"><span data-stu-id="1bff9-125">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="1bff9-126">O deve ser extraído do token de auth e não inserido `user` manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="1bff9-126">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1bff9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bff9-127">JSON representation</span></span>

<span data-ttu-id="1bff9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bff9-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


