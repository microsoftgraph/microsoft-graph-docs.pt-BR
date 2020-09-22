---
title: tipo de recurso alertHistoryState
description: Armazena as alterações feitas nos alertas.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: cf8043b4409b29220841e2706649050003b09f34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004275"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="d22a6-103">tipo de recurso alertHistoryState</span><span class="sxs-lookup"><span data-stu-id="d22a6-103">alertHistoryState resource type</span></span>

<span data-ttu-id="d22a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d22a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d22a6-105">Armazena as alterações feitas nos alertas.</span><span class="sxs-lookup"><span data-stu-id="d22a6-105">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="d22a6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d22a6-106">Properties</span></span>

| <span data-ttu-id="d22a6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d22a6-107">Property</span></span>     | <span data-ttu-id="d22a6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d22a6-108">Type</span></span>        | <span data-ttu-id="d22a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d22a6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d22a6-110">appId</span><span class="sxs-lookup"><span data-stu-id="d22a6-110">appId</span></span>|<span data-ttu-id="d22a6-111">String</span><span class="sxs-lookup"><span data-stu-id="d22a6-111">String</span></span>| <span data-ttu-id="d22a6-112">A ID de aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) para o alerta.</span><span class="sxs-lookup"><span data-stu-id="d22a6-112">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="d22a6-113">A appId deve ser extraída do token de autenticação e não inserida manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="d22a6-113">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="d22a6-114">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d22a6-114">assignedTo</span></span>|<span data-ttu-id="d22a6-115">String</span><span class="sxs-lookup"><span data-stu-id="d22a6-115">String</span></span>| <span data-ttu-id="d22a6-116">UPN de usuário ao qual o alerta foi atribuído (Observação: Alert. assignedTo só armazena o último valor/UPN).</span><span class="sxs-lookup"><span data-stu-id="d22a6-116">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="d22a6-117">comentários</span><span class="sxs-lookup"><span data-stu-id="d22a6-117">comments</span></span>|<span data-ttu-id="d22a6-118">String collection</span><span class="sxs-lookup"><span data-stu-id="d22a6-118">String collection</span></span>|<span data-ttu-id="d22a6-119">Comentário inserido pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d22a6-119">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="d22a6-120">comentários</span><span class="sxs-lookup"><span data-stu-id="d22a6-120">feedback</span></span>|<span data-ttu-id="d22a6-121">String</span><span class="sxs-lookup"><span data-stu-id="d22a6-121">String</span></span>| <span data-ttu-id="d22a6-122">Comentários de analista sobre o alerta nesta atualização.</span><span class="sxs-lookup"><span data-stu-id="d22a6-122">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="d22a6-123">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="d22a6-123">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="d22a6-124">status</span><span class="sxs-lookup"><span data-stu-id="d22a6-124">status</span></span>|<span data-ttu-id="d22a6-125">String</span><span class="sxs-lookup"><span data-stu-id="d22a6-125">String</span></span>| <span data-ttu-id="d22a6-126">Valor do status do alerta (se atualizado).</span><span class="sxs-lookup"><span data-stu-id="d22a6-126">Alert status value (if updated).</span></span> <span data-ttu-id="d22a6-127">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="d22a6-127">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="d22a6-128">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d22a6-128">updatedDateTime</span></span>|<span data-ttu-id="d22a6-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d22a6-129">DateTimeOffset</span></span>| <span data-ttu-id="d22a6-130">Data e hora da atualização de alerta.</span><span class="sxs-lookup"><span data-stu-id="d22a6-130">Date and time of the alert update.</span></span> <span data-ttu-id="d22a6-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d22a6-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d22a6-132">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d22a6-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d22a6-133">user</span><span class="sxs-lookup"><span data-stu-id="d22a6-133">user</span></span>|<span data-ttu-id="d22a6-134">String</span><span class="sxs-lookup"><span data-stu-id="d22a6-134">String</span></span>| <span data-ttu-id="d22a6-135">O UPN do usuário conectado que atualizou o alerta (obtido do token de portador-se no modo de autenticação do usuário/delegado).</span><span class="sxs-lookup"><span data-stu-id="d22a6-135">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d22a6-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d22a6-136">JSON representation</span></span>

<span data-ttu-id="d22a6-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d22a6-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

