---
title: tipo de recurso securityActionState
description: Representa o histórico das alterações de estado SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ba22a03f4d4a6d03b0093ed28b8c54a7c095d037
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988860"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="062cf-103">tipo de recurso securityActionState</span><span class="sxs-lookup"><span data-stu-id="062cf-103">securityActionState resource type</span></span>

<span data-ttu-id="062cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="062cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="062cf-105">Representa o histórico das alterações de estado SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="062cf-105">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="062cf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="062cf-106">Properties</span></span>

| <span data-ttu-id="062cf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="062cf-107">Property</span></span>     | <span data-ttu-id="062cf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="062cf-108">Type</span></span>        | <span data-ttu-id="062cf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="062cf-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="062cf-110">appId</span><span class="sxs-lookup"><span data-stu-id="062cf-110">appId</span></span>|<span data-ttu-id="062cf-111">String</span><span class="sxs-lookup"><span data-stu-id="062cf-111">String</span></span>|<span data-ttu-id="062cf-112">A ID de aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) à ação.</span><span class="sxs-lookup"><span data-stu-id="062cf-112">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="062cf-113">O `appId` deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="062cf-113">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="062cf-114">status</span><span class="sxs-lookup"><span data-stu-id="062cf-114">status</span></span>|<span data-ttu-id="062cf-115">String</span><span class="sxs-lookup"><span data-stu-id="062cf-115">String</span></span>| <span data-ttu-id="062cf-116">Status do SecurityAction nesta atualização.</span><span class="sxs-lookup"><span data-stu-id="062cf-116">Status of the securityAction in this update.</span></span> <span data-ttu-id="062cf-117">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="062cf-117">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="062cf-118">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="062cf-118">updatedDateTime</span></span>|<span data-ttu-id="062cf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="062cf-119">DateTimeOffset</span></span>| <span data-ttu-id="062cf-120">Carimbo de data/hora em que ActionState foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="062cf-120">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="062cf-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="062cf-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="062cf-122">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="062cf-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="062cf-123">user</span><span class="sxs-lookup"><span data-stu-id="062cf-123">user</span></span>|<span data-ttu-id="062cf-124">String</span><span class="sxs-lookup"><span data-stu-id="062cf-124">String</span></span>|<span data-ttu-id="062cf-125">O nome principal de usuário do usuário conectado que enviou uma atualização (PATCH) à ação.</span><span class="sxs-lookup"><span data-stu-id="062cf-125">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="062cf-126">O `user` deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="062cf-126">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="062cf-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="062cf-127">JSON representation</span></span>

<span data-ttu-id="062cf-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="062cf-128">The following is a JSON representation of the resource.</span></span>

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


