---
title: tipo de recurso alertHistoryState
description: Armazena as alterações feitas nos alertas.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461037"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="94eea-103">tipo de recurso alertHistoryState</span><span class="sxs-lookup"><span data-stu-id="94eea-103">alertHistoryState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94eea-104">Armazena as alterações feitas nos alertas.</span><span class="sxs-lookup"><span data-stu-id="94eea-104">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="94eea-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94eea-105">Properties</span></span>

| <span data-ttu-id="94eea-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94eea-106">Property</span></span>     | <span data-ttu-id="94eea-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="94eea-107">Type</span></span>        | <span data-ttu-id="94eea-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="94eea-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94eea-109">appId</span><span class="sxs-lookup"><span data-stu-id="94eea-109">appId</span></span>|<span data-ttu-id="94eea-110">String</span><span class="sxs-lookup"><span data-stu-id="94eea-110">String</span></span>| <span data-ttu-id="94eea-111">A ID de aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) para o alerta.</span><span class="sxs-lookup"><span data-stu-id="94eea-111">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="94eea-112">A appId deve ser extraída do token de autenticação e não inserida manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="94eea-112">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="94eea-113">assignedTo</span><span class="sxs-lookup"><span data-stu-id="94eea-113">assignedTo</span></span>|<span data-ttu-id="94eea-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94eea-114">String</span></span>| <span data-ttu-id="94eea-115">UPN de usuário ao qual o alerta foi atribuído (Observação: Alert. assignedTo só armazena o último valor/UPN).</span><span class="sxs-lookup"><span data-stu-id="94eea-115">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="94eea-116">comentários</span><span class="sxs-lookup"><span data-stu-id="94eea-116">comments</span></span>|<span data-ttu-id="94eea-117">String collection</span><span class="sxs-lookup"><span data-stu-id="94eea-117">String collection</span></span>|<span data-ttu-id="94eea-118">Comentário inserido pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="94eea-118">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="94eea-119">comentários</span><span class="sxs-lookup"><span data-stu-id="94eea-119">feedback</span></span>|<span data-ttu-id="94eea-120">String</span><span class="sxs-lookup"><span data-stu-id="94eea-120">String</span></span>| <span data-ttu-id="94eea-121">Comentários de analista sobre o alerta nesta atualização.</span><span class="sxs-lookup"><span data-stu-id="94eea-121">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="94eea-122">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="94eea-122">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="94eea-123">status</span><span class="sxs-lookup"><span data-stu-id="94eea-123">status</span></span>|<span data-ttu-id="94eea-124">String</span><span class="sxs-lookup"><span data-stu-id="94eea-124">String</span></span>| <span data-ttu-id="94eea-125">Valor do status do alerta (se atualizado).</span><span class="sxs-lookup"><span data-stu-id="94eea-125">Alert status value (if updated).</span></span> <span data-ttu-id="94eea-126">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="94eea-126">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="94eea-127">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="94eea-127">updatedDateTime</span></span>|<span data-ttu-id="94eea-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94eea-128">DateTimeOffset</span></span>| <span data-ttu-id="94eea-129">Data e hora da atualização de alerta.</span><span class="sxs-lookup"><span data-stu-id="94eea-129">Date and time of the alert update.</span></span> <span data-ttu-id="94eea-130">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="94eea-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94eea-131">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="94eea-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="94eea-132">user</span><span class="sxs-lookup"><span data-stu-id="94eea-132">user</span></span>|<span data-ttu-id="94eea-133">String</span><span class="sxs-lookup"><span data-stu-id="94eea-133">String</span></span>| <span data-ttu-id="94eea-134">O UPN do usuário conectado que atualizou o alerta (obtido do token de portador-se no modo de autenticação do usuário/delegado).</span><span class="sxs-lookup"><span data-stu-id="94eea-134">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94eea-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94eea-135">JSON representation</span></span>

<span data-ttu-id="94eea-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94eea-136">The following is a JSON representation of the resource.</span></span>

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