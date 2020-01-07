---
title: tipo de recurso offerShiftRequest
description: Representa o tipo de solicitação de mudança para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2b12dd9df816ad7fecbf6c520f0fff579087428
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952290"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="7df81-103">tipo de recurso offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="7df81-103">offerShiftRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7df81-104">Representa o tipo de solicitação de mudança para oferecer uma mudança para outro usuário na equipe.</span><span class="sxs-lookup"><span data-stu-id="7df81-104">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="7df81-105">Methods</span><span class="sxs-lookup"><span data-stu-id="7df81-105">Methods</span></span>

| <span data-ttu-id="7df81-106">Método</span><span class="sxs-lookup"><span data-stu-id="7df81-106">Method</span></span>       | <span data-ttu-id="7df81-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7df81-107">Return Type</span></span> | <span data-ttu-id="7df81-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7df81-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7df81-109">Criar</span><span class="sxs-lookup"><span data-stu-id="7df81-109">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="7df81-110">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="7df81-110">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="7df81-111">Criar uma instância de um objeto offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="7df81-111">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="7df81-112">Get</span><span class="sxs-lookup"><span data-stu-id="7df81-112">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="7df81-113">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="7df81-113">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="7df81-114">Leia as propriedades e os relacionamentos do objeto offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="7df81-114">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="7df81-115">List</span><span class="sxs-lookup"><span data-stu-id="7df81-115">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="7df81-116">Coleção de [offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="7df81-116">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="7df81-117">Leia as propriedades e as relações de todos os objetos offerShiftRequest de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="7df81-117">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="7df81-118">Aprovar</span><span class="sxs-lookup"><span data-stu-id="7df81-118">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="7df81-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7df81-119">None</span></span>|<span data-ttu-id="7df81-120">Aprovar um offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="7df81-120">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="7df81-121">Aceito</span><span class="sxs-lookup"><span data-stu-id="7df81-121">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="7df81-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7df81-122">None</span></span>|<span data-ttu-id="7df81-123">Recusar um offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="7df81-123">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="7df81-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7df81-124">Properties</span></span>

| <span data-ttu-id="7df81-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7df81-125">Property</span></span>     | <span data-ttu-id="7df81-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="7df81-126">Type</span></span>        | <span data-ttu-id="7df81-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="7df81-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7df81-128">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7df81-128">recipientActionDateTime</span></span>|<span data-ttu-id="7df81-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df81-129">DateTimeOffset</span></span>|<span data-ttu-id="7df81-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7df81-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7df81-132">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="7df81-132">recipientActionMessage</span></span>|<span data-ttu-id="7df81-133">String</span><span class="sxs-lookup"><span data-stu-id="7df81-133">String</span></span>| <span data-ttu-id="7df81-134">Mensagem personalizada enviada pelo destinatário da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="7df81-134">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="7df81-135">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="7df81-135">recipientUserId</span></span>|<span data-ttu-id="7df81-136">String</span><span class="sxs-lookup"><span data-stu-id="7df81-136">String</span></span>| <span data-ttu-id="7df81-137">ID de usuário do destinatário da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="7df81-137">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="7df81-138">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="7df81-138">senderShiftId</span></span>|<span data-ttu-id="7df81-139">String</span><span class="sxs-lookup"><span data-stu-id="7df81-139">String</span></span>| <span data-ttu-id="7df81-140">ID de usuário do remetente da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="7df81-140">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df81-141">Relações</span><span class="sxs-lookup"><span data-stu-id="7df81-141">Relationships</span></span>

<span data-ttu-id="7df81-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7df81-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7df81-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7df81-143">JSON representation</span></span>

<span data-ttu-id="7df81-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7df81-144">The following is a JSON representation of the resource.</span></span>

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
