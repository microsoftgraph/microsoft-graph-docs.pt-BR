---
title: Tipo de recurso offerShiftRequest
description: Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d17ca029d29b2b8f27a923adf4ef019ac002f404
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158720"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="22c6d-103">Tipo de recurso offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="22c6d-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="22c6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22c6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22c6d-105">Representa uma solicitação para oferecer uma mudança para outro usuário na equipe.</span><span class="sxs-lookup"><span data-stu-id="22c6d-105">Represents a request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="22c6d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="22c6d-106">Methods</span></span>

| <span data-ttu-id="22c6d-107">Método</span><span class="sxs-lookup"><span data-stu-id="22c6d-107">Method</span></span>       | <span data-ttu-id="22c6d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22c6d-108">Return Type</span></span> | <span data-ttu-id="22c6d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="22c6d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="22c6d-110">List</span><span class="sxs-lookup"><span data-stu-id="22c6d-110">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="22c6d-111">Coleção de [offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="22c6d-111">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="22c6d-112">Leia as propriedades e os relacionamentos de todos os **objetos offerShiftRequest** em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="22c6d-112">Read the properties and relationships of all **offerShiftRequest** objects in a team.</span></span> |
| [<span data-ttu-id="22c6d-113">Criar</span><span class="sxs-lookup"><span data-stu-id="22c6d-113">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="22c6d-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="22c6d-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="22c6d-115">Crie uma instância de um **objeto offerShiftRequest.**</span><span class="sxs-lookup"><span data-stu-id="22c6d-115">Create an instance of an **offerShiftRequest** object.</span></span> |
| [<span data-ttu-id="22c6d-116">Get</span><span class="sxs-lookup"><span data-stu-id="22c6d-116">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="22c6d-117">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="22c6d-117">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="22c6d-118">Leia as propriedades e os relacionamentos de um **objeto offerShiftRequest.**</span><span class="sxs-lookup"><span data-stu-id="22c6d-118">Read the properties and relationships of an **offerShiftRequest** object.</span></span> |
|[<span data-ttu-id="22c6d-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="22c6d-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="22c6d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22c6d-120">None</span></span>|<span data-ttu-id="22c6d-121">Aprovar uma **ofertaShiftRequest**.</span><span class="sxs-lookup"><span data-stu-id="22c6d-121">Approve an **offerShiftRequest**.</span></span> |
|[<span data-ttu-id="22c6d-122">Recusar</span><span class="sxs-lookup"><span data-stu-id="22c6d-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="22c6d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22c6d-123">None</span></span>|<span data-ttu-id="22c6d-124">Recusar uma **ofertaShiftRequest**.</span><span class="sxs-lookup"><span data-stu-id="22c6d-124">Decline an **offerShiftRequest**.</span></span> |

## <a name="properties"></a><span data-ttu-id="22c6d-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22c6d-125">Properties</span></span>

| <span data-ttu-id="22c6d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22c6d-126">Property</span></span>     | <span data-ttu-id="22c6d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="22c6d-127">Type</span></span>        | <span data-ttu-id="22c6d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="22c6d-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22c6d-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="22c6d-129">recipientActionDateTime</span></span>|<span data-ttu-id="22c6d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22c6d-130">DateTimeOffset</span></span>|<span data-ttu-id="22c6d-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="22c6d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="22c6d-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="22c6d-133">recipientActionMessage</span></span>|<span data-ttu-id="22c6d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22c6d-134">String</span></span>| <span data-ttu-id="22c6d-135">Mensagem personalizada enviada pelo destinatário da solicitação de turno de oferta.</span><span class="sxs-lookup"><span data-stu-id="22c6d-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="22c6d-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="22c6d-136">recipientUserId</span></span>|<span data-ttu-id="22c6d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22c6d-137">String</span></span>| <span data-ttu-id="22c6d-138">ID de usuário do destinatário da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="22c6d-138">User ID of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="22c6d-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="22c6d-139">senderShiftId</span></span>|<span data-ttu-id="22c6d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22c6d-140">String</span></span>| <span data-ttu-id="22c6d-141">ID de usuário do remetente da solicitação de mudança de oferta.</span><span class="sxs-lookup"><span data-stu-id="22c6d-141">User ID of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22c6d-142">Relações</span><span class="sxs-lookup"><span data-stu-id="22c6d-142">Relationships</span></span>

<span data-ttu-id="22c6d-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22c6d-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22c6d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22c6d-144">JSON representation</span></span>

<span data-ttu-id="22c6d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22c6d-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest"
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

