---
title: Tipo de recurso alertHistoryState
description: Armazena alterações feitas em alertas.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2bc1c1a58f6f7f073b6803adbee07b4b2990a0e1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722164"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="d30e3-103">Tipo de recurso alertHistoryState</span><span class="sxs-lookup"><span data-stu-id="d30e3-103">alertHistoryState resource type</span></span>

<span data-ttu-id="d30e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d30e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30e3-105">Armazena alterações feitas em alertas.</span><span class="sxs-lookup"><span data-stu-id="d30e3-105">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="d30e3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d30e3-106">Properties</span></span>

| <span data-ttu-id="d30e3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d30e3-107">Property</span></span>     | <span data-ttu-id="d30e3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d30e3-108">Type</span></span>        | <span data-ttu-id="d30e3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d30e3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d30e3-110">appId</span><span class="sxs-lookup"><span data-stu-id="d30e3-110">appId</span></span>|<span data-ttu-id="d30e3-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d30e3-111">String</span></span>| <span data-ttu-id="d30e3-112">A ID do Aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) ao alerta.</span><span class="sxs-lookup"><span data-stu-id="d30e3-112">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="d30e3-113">O appId deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="d30e3-113">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="d30e3-114">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d30e3-114">assignedTo</span></span>|<span data-ttu-id="d30e3-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d30e3-115">String</span></span>| <span data-ttu-id="d30e3-116">UPN do usuário ao que o alerta foi atribuído (observação: alert.assignedTo armazena apenas o último valor/UPN).</span><span class="sxs-lookup"><span data-stu-id="d30e3-116">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="d30e3-117">comentários</span><span class="sxs-lookup"><span data-stu-id="d30e3-117">comments</span></span>|<span data-ttu-id="d30e3-118">String collection</span><span class="sxs-lookup"><span data-stu-id="d30e3-118">String collection</span></span>|<span data-ttu-id="d30e3-119">Comentário inserido pelo usuário inserido.</span><span class="sxs-lookup"><span data-stu-id="d30e3-119">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="d30e3-120">comentários</span><span class="sxs-lookup"><span data-stu-id="d30e3-120">feedback</span></span>|<span data-ttu-id="d30e3-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d30e3-121">String</span></span>| <span data-ttu-id="d30e3-122">Comentários do analista sobre o alerta nesta atualização.</span><span class="sxs-lookup"><span data-stu-id="d30e3-122">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="d30e3-123">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="d30e3-123">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="d30e3-124">status</span><span class="sxs-lookup"><span data-stu-id="d30e3-124">status</span></span>|<span data-ttu-id="d30e3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d30e3-125">String</span></span>| <span data-ttu-id="d30e3-126">Valor de status do alerta (se atualizado).</span><span class="sxs-lookup"><span data-stu-id="d30e3-126">Alert status value (if updated).</span></span> <span data-ttu-id="d30e3-127">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="d30e3-127">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="d30e3-128">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d30e3-128">updatedDateTime</span></span>|<span data-ttu-id="d30e3-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30e3-129">DateTimeOffset</span></span>| <span data-ttu-id="d30e3-130">Data e hora da atualização de alerta.</span><span class="sxs-lookup"><span data-stu-id="d30e3-130">Date and time of the alert update.</span></span> <span data-ttu-id="d30e3-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d30e3-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d30e3-132">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d30e3-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d30e3-133">user</span><span class="sxs-lookup"><span data-stu-id="d30e3-133">user</span></span>|<span data-ttu-id="d30e3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d30e3-134">String</span></span>| <span data-ttu-id="d30e3-135">UPN do usuário que atualizou o alerta (retirado do token do portador - se no modo de auth delegado/do usuário).</span><span class="sxs-lookup"><span data-stu-id="d30e3-135">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d30e3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d30e3-136">JSON representation</span></span>

<span data-ttu-id="d30e3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d30e3-137">The following is a JSON representation of the resource.</span></span>

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

