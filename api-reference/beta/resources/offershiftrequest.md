---
title: tipo de recurso offerShiftRequest
description: Representa o tipo de solicitação de mudança para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c41461848fab45f3d291b175e6c584f98326fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021270"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="eb123-103">tipo de recurso offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="eb123-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="eb123-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb123-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb123-105">Representa o tipo de solicitação de mudança para oferecer uma mudança para outro usuário na equipe.</span><span class="sxs-lookup"><span data-stu-id="eb123-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="eb123-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb123-106">Methods</span></span>

| <span data-ttu-id="eb123-107">Método</span><span class="sxs-lookup"><span data-stu-id="eb123-107">Method</span></span>       | <span data-ttu-id="eb123-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb123-108">Return Type</span></span> | <span data-ttu-id="eb123-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb123-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb123-110">Criar</span><span class="sxs-lookup"><span data-stu-id="eb123-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="eb123-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="eb123-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="eb123-112">Criar uma instância de um objeto offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="eb123-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="eb123-113">Get</span><span class="sxs-lookup"><span data-stu-id="eb123-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="eb123-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="eb123-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="eb123-115">Leia as propriedades e os relacionamentos do objeto offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="eb123-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="eb123-116">Lista</span><span class="sxs-lookup"><span data-stu-id="eb123-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="eb123-117">Coleção de [offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="eb123-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="eb123-118">Leia as propriedades e as relações de todos os objetos offerShiftRequest de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="eb123-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="eb123-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="eb123-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="eb123-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb123-120">None</span></span>|<span data-ttu-id="eb123-121">Aprovar um offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="eb123-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="eb123-122">Aceito</span><span class="sxs-lookup"><span data-stu-id="eb123-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="eb123-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb123-123">None</span></span>|<span data-ttu-id="eb123-124">Recusar um offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="eb123-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb123-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb123-125">Properties</span></span>

| <span data-ttu-id="eb123-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb123-126">Property</span></span>     | <span data-ttu-id="eb123-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb123-127">Type</span></span>        | <span data-ttu-id="eb123-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb123-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb123-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="eb123-129">recipientActionDateTime</span></span>|<span data-ttu-id="eb123-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb123-130">DateTimeOffset</span></span>|<span data-ttu-id="eb123-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eb123-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eb123-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="eb123-133">recipientActionMessage</span></span>|<span data-ttu-id="eb123-134">String</span><span class="sxs-lookup"><span data-stu-id="eb123-134">String</span></span>| <span data-ttu-id="eb123-135">Mensagem personalizada enviada pelo destinatário da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="eb123-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="eb123-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="eb123-136">recipientUserId</span></span>|<span data-ttu-id="eb123-137">String</span><span class="sxs-lookup"><span data-stu-id="eb123-137">String</span></span>| <span data-ttu-id="eb123-138">ID de usuário do destinatário da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="eb123-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="eb123-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="eb123-139">senderShiftId</span></span>|<span data-ttu-id="eb123-140">String</span><span class="sxs-lookup"><span data-stu-id="eb123-140">String</span></span>| <span data-ttu-id="eb123-141">ID de usuário do remetente da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="eb123-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb123-142">Relações</span><span class="sxs-lookup"><span data-stu-id="eb123-142">Relationships</span></span>

<span data-ttu-id="eb123-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb123-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb123-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb123-144">JSON representation</span></span>

<span data-ttu-id="eb123-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb123-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": ""
}-->

```json
{
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


