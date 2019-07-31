---
title: tipo de recurso securityActionState
description: Representa o histórico das alterações de estado SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e3efd29e156b6e0346574c74fad2a30a39ec7131
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008506"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="d59f6-103">tipo de recurso securityActionState</span><span class="sxs-lookup"><span data-stu-id="d59f6-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d59f6-104">Representa o histórico das alterações de estado SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="d59f6-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="d59f6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d59f6-105">Properties</span></span>

| <span data-ttu-id="d59f6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d59f6-106">Property</span></span>     | <span data-ttu-id="d59f6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d59f6-107">Type</span></span>        | <span data-ttu-id="d59f6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d59f6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d59f6-109">appId</span><span class="sxs-lookup"><span data-stu-id="d59f6-109">appId</span></span>|<span data-ttu-id="d59f6-110">String</span><span class="sxs-lookup"><span data-stu-id="d59f6-110">String</span></span>|<span data-ttu-id="d59f6-111">A ID de aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) à ação.</span><span class="sxs-lookup"><span data-stu-id="d59f6-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="d59f6-112">O `appId` deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="d59f6-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="d59f6-113">status</span><span class="sxs-lookup"><span data-stu-id="d59f6-113">status</span></span>|<span data-ttu-id="d59f6-114">String</span><span class="sxs-lookup"><span data-stu-id="d59f6-114">String</span></span>| <span data-ttu-id="d59f6-115">Status do SecurityAction nesta atualização.</span><span class="sxs-lookup"><span data-stu-id="d59f6-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="d59f6-116">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="d59f6-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="d59f6-117">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d59f6-117">updatedDateTime</span></span>|<span data-ttu-id="d59f6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59f6-118">DateTimeOffset</span></span>| <span data-ttu-id="d59f6-119">Carimbo de data/hora em que ActionState foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="d59f6-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="d59f6-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d59f6-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d59f6-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d59f6-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d59f6-122">user</span><span class="sxs-lookup"><span data-stu-id="d59f6-122">user</span></span>|<span data-ttu-id="d59f6-123">String</span><span class="sxs-lookup"><span data-stu-id="d59f6-123">String</span></span>|<span data-ttu-id="d59f6-124">O nome principal de usuário do usuário conectado que enviou uma atualização (PATCH) à ação.</span><span class="sxs-lookup"><span data-stu-id="d59f6-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="d59f6-125">O `user` deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="d59f6-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d59f6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d59f6-126">JSON representation</span></span>

<span data-ttu-id="d59f6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d59f6-127">The following is a JSON representation of the resource.</span></span>

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
