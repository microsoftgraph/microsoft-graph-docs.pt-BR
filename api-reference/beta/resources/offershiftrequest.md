---
title: Tipo de recurso offerShiftRequest
description: Representa o tipo de solicitação de turno para oferecer uma mudança para outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f80e8578422aa00d6af1d2df22a0dfb7472c8c8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721478"
---
# <a name="offershiftrequest-resource-type"></a><span data-ttu-id="498bf-103">Tipo de recurso offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="498bf-103">offerShiftRequest resource type</span></span>

<span data-ttu-id="498bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="498bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="498bf-105">Representa o tipo de solicitação de turno para oferecer uma mudança para outro usuário na equipe.</span><span class="sxs-lookup"><span data-stu-id="498bf-105">Represents type of shift request to offer a shift to another user in the team.</span></span>

## <a name="methods"></a><span data-ttu-id="498bf-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="498bf-106">Methods</span></span>

| <span data-ttu-id="498bf-107">Método</span><span class="sxs-lookup"><span data-stu-id="498bf-107">Method</span></span>       | <span data-ttu-id="498bf-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="498bf-108">Return Type</span></span> | <span data-ttu-id="498bf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="498bf-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="498bf-110">Criar</span><span class="sxs-lookup"><span data-stu-id="498bf-110">Create</span></span>](../api/offershiftrequest-post.md) | [<span data-ttu-id="498bf-111">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="498bf-111">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="498bf-112">Crie uma instância de um objeto offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="498bf-112">Create an instance of an offerShiftRequest object.</span></span> |
| [<span data-ttu-id="498bf-113">Get</span><span class="sxs-lookup"><span data-stu-id="498bf-113">Get</span></span>](../api/offershiftrequest-get.md) | [<span data-ttu-id="498bf-114">offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="498bf-114">offerShiftRequest</span></span>](offershiftrequest.md) | <span data-ttu-id="498bf-115">Ler propriedades e relações do objeto offerShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="498bf-115">Read properties and relationships of offerShiftRequest object.</span></span> |
| [<span data-ttu-id="498bf-116">List</span><span class="sxs-lookup"><span data-stu-id="498bf-116">List</span></span>](../api/offershiftrequest-list.md) | <span data-ttu-id="498bf-117">Coleção [of offerShiftRequest](offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="498bf-117">Collection of [offerShiftRequest](offershiftrequest.md)</span></span> | <span data-ttu-id="498bf-118">Leia propriedades e relações de todos os objetos offerShiftRequest em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="498bf-118">Read properties and relationships of all offerShiftRequest objects in a team.</span></span> |
|[<span data-ttu-id="498bf-119">Aprovar</span><span class="sxs-lookup"><span data-stu-id="498bf-119">Approve</span></span>](../api/offershiftrequest-approve.md)|<span data-ttu-id="498bf-120">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="498bf-120">None</span></span>|<span data-ttu-id="498bf-121">Aprovar uma ofertaShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="498bf-121">Approve an offerShiftRequest.</span></span> |
|[<span data-ttu-id="498bf-122">Declínio</span><span class="sxs-lookup"><span data-stu-id="498bf-122">Decline</span></span>](../api/offershiftrequest-decline.md)|<span data-ttu-id="498bf-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="498bf-123">None</span></span>|<span data-ttu-id="498bf-124">Recusar uma ofertaShiftRequest.</span><span class="sxs-lookup"><span data-stu-id="498bf-124">Decline an offerShiftRequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="498bf-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="498bf-125">Properties</span></span>

| <span data-ttu-id="498bf-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="498bf-126">Property</span></span>     | <span data-ttu-id="498bf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="498bf-127">Type</span></span>        | <span data-ttu-id="498bf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="498bf-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="498bf-129">recipientActionDateTime</span><span class="sxs-lookup"><span data-stu-id="498bf-129">recipientActionDateTime</span></span>|<span data-ttu-id="498bf-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="498bf-130">DateTimeOffset</span></span>|<span data-ttu-id="498bf-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="498bf-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="498bf-132">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="498bf-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="498bf-133">recipientActionMessage</span><span class="sxs-lookup"><span data-stu-id="498bf-133">recipientActionMessage</span></span>|<span data-ttu-id="498bf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="498bf-134">String</span></span>| <span data-ttu-id="498bf-135">Mensagem personalizada enviada pelo destinatário da solicitação de turno de oferta.</span><span class="sxs-lookup"><span data-stu-id="498bf-135">Custom message sent by recipient of the offer shift request.</span></span> |
|<span data-ttu-id="498bf-136">recipientUserId</span><span class="sxs-lookup"><span data-stu-id="498bf-136">recipientUserId</span></span>|<span data-ttu-id="498bf-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="498bf-137">String</span></span>| <span data-ttu-id="498bf-138">ID do usuário do destinatário da solicitação de turno de oferta.</span><span class="sxs-lookup"><span data-stu-id="498bf-138">User id of the recipient of the offer shift request.</span></span>|
|<span data-ttu-id="498bf-139">senderShiftId</span><span class="sxs-lookup"><span data-stu-id="498bf-139">senderShiftId</span></span>|<span data-ttu-id="498bf-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="498bf-140">String</span></span>| <span data-ttu-id="498bf-141">ID do usuário do remetente da solicitação de turno de oferta.</span><span class="sxs-lookup"><span data-stu-id="498bf-141">User id of the sender of the offer shift request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="498bf-142">Relações</span><span class="sxs-lookup"><span data-stu-id="498bf-142">Relationships</span></span>

<span data-ttu-id="498bf-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="498bf-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="498bf-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="498bf-144">JSON representation</span></span>

<span data-ttu-id="498bf-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="498bf-145">The following is a JSON representation of the resource.</span></span>

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


