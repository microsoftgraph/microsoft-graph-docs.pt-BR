---
title: tipo de recurso de privilegedApproval
description: Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.
ms.openlocfilehash: 3f900ef4a141b2f71c303becd49789b86cefb1b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037031"
---
# <a name="privilegedapproval-resource-type"></a><span data-ttu-id="5b17e-103">tipo de recurso de privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-103">privilegedApproval resource type</span></span>

> <span data-ttu-id="5b17e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b17e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b17e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b17e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b17e-106">Representa uma aprovação solicitada no gerenciamento de identidades privilegiado para entrar em uma função.</span><span class="sxs-lookup"><span data-stu-id="5b17e-106">Represents an approval that is requested in Privileged Identity Management for getting into a role.</span></span>


## <a name="methods"></a><span data-ttu-id="5b17e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5b17e-107">Methods</span></span>

| <span data-ttu-id="5b17e-108">Método</span><span class="sxs-lookup"><span data-stu-id="5b17e-108">Method</span></span>           | <span data-ttu-id="5b17e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b17e-109">Return Type</span></span>    |<span data-ttu-id="5b17e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b17e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b17e-111">Obter privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-111">Get privilegedApproval</span></span>](../api/privilegedapproval-get.md) | [<span data-ttu-id="5b17e-112">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-112">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="5b17e-113">Leia as propriedades e os relacionamentos do objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="5b17e-113">Read properties and relationships of privilegedApproval object.</span></span>|
|[<span data-ttu-id="5b17e-114">Objetos de privilegedApproval List</span><span class="sxs-lookup"><span data-stu-id="5b17e-114">List privilegedApproval objects</span></span>](../api/privilegedapproval-list.md) | <span data-ttu-id="5b17e-115">coleção [privilegedApproval](privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="5b17e-115">[privilegedApproval](privilegedapproval.md) collection</span></span>|<span data-ttu-id="5b17e-116">Obtenha a coleção de privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="5b17e-116">Get the collection of privilegedApproval.</span></span>|
|[<span data-ttu-id="5b17e-117">Criar privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-117">Create privilegedApproval</span></span>](../api/privilegedapproval-post-privilegedapproval.md) | [<span data-ttu-id="5b17e-118">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-118">privilegedApproval</span></span>](privilegedapproval.md)    |<span data-ttu-id="5b17e-119">Crie objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="5b17e-119">Create privilegedApproval object.</span></span> |
|[<span data-ttu-id="5b17e-120">Atualizar privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-120">Update privilegedApproval</span></span>](../api/privilegedapproval-update.md) | [<span data-ttu-id="5b17e-121">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-121">privilegedApproval</span></span>](privilegedapproval.md) |<span data-ttu-id="5b17e-122">Atualize o objeto privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="5b17e-122">Update privilegedApproval object.</span></span> |
|[<span data-ttu-id="5b17e-123">Myrequests</span><span class="sxs-lookup"><span data-stu-id="5b17e-123">Myrequests</span></span>](../api/privilegedapproval-myrequests.md)|[<span data-ttu-id="5b17e-124">privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="5b17e-124">privilegedApproval</span></span>](privilegedapproval.md)|<span data-ttu-id="5b17e-125">Obtenha as solicitações de aprovação do solicitador.</span><span class="sxs-lookup"><span data-stu-id="5b17e-125">Get the requestor's approval requests.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b17e-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b17e-126">Properties</span></span>
| <span data-ttu-id="5b17e-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b17e-127">Property</span></span>     | <span data-ttu-id="5b17e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b17e-128">Type</span></span>   |<span data-ttu-id="5b17e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b17e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b17e-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="5b17e-130">approvalDuration</span></span>|<span data-ttu-id="5b17e-131">Duração</span><span class="sxs-lookup"><span data-stu-id="5b17e-131">Duration</span></span>||
|<span data-ttu-id="5b17e-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="5b17e-132">approvalState</span></span>|<span data-ttu-id="5b17e-133">string</span><span class="sxs-lookup"><span data-stu-id="5b17e-133">string</span></span>| <span data-ttu-id="5b17e-134">Os valores possíveis são: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="5b17e-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="5b17e-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="5b17e-135">approvalType</span></span>|<span data-ttu-id="5b17e-136">String</span><span class="sxs-lookup"><span data-stu-id="5b17e-136">String</span></span>||
|<span data-ttu-id="5b17e-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="5b17e-137">approverReason</span></span>|<span data-ttu-id="5b17e-138">String</span><span class="sxs-lookup"><span data-stu-id="5b17e-138">String</span></span>||
|<span data-ttu-id="5b17e-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5b17e-139">endDateTime</span></span>|<span data-ttu-id="5b17e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b17e-140">DateTimeOffset</span></span>|<span data-ttu-id="5b17e-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5b17e-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5b17e-143">id</span><span class="sxs-lookup"><span data-stu-id="5b17e-143">id</span></span>|<span data-ttu-id="5b17e-144">String</span><span class="sxs-lookup"><span data-stu-id="5b17e-144">String</span></span>| <span data-ttu-id="5b17e-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b17e-145">Read-only.</span></span>|
|<span data-ttu-id="5b17e-146">requestorReason</span><span class="sxs-lookup"><span data-stu-id="5b17e-146">requestorReason</span></span>|<span data-ttu-id="5b17e-147">String</span><span class="sxs-lookup"><span data-stu-id="5b17e-147">String</span></span>||
|<span data-ttu-id="5b17e-148">roleId</span><span class="sxs-lookup"><span data-stu-id="5b17e-148">roleId</span></span>|<span data-ttu-id="5b17e-149">String</span><span class="sxs-lookup"><span data-stu-id="5b17e-149">String</span></span>||
|<span data-ttu-id="5b17e-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5b17e-150">startDateTime</span></span>|<span data-ttu-id="5b17e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b17e-151">DateTimeOffset</span></span>|<span data-ttu-id="5b17e-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5b17e-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5b17e-154">userId</span><span class="sxs-lookup"><span data-stu-id="5b17e-154">userId</span></span>|<span data-ttu-id="5b17e-155">String</span><span class="sxs-lookup"><span data-stu-id="5b17e-155">String</span></span>||

## <a name="relationships"></a><span data-ttu-id="5b17e-156">Relações</span><span class="sxs-lookup"><span data-stu-id="5b17e-156">Relationships</span></span>
| <span data-ttu-id="5b17e-157">Relação</span><span class="sxs-lookup"><span data-stu-id="5b17e-157">Relationship</span></span> | <span data-ttu-id="5b17e-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b17e-158">Type</span></span>   |<span data-ttu-id="5b17e-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b17e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b17e-160">roleInfo</span><span class="sxs-lookup"><span data-stu-id="5b17e-160">roleInfo</span></span>|[<span data-ttu-id="5b17e-161">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="5b17e-161">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="5b17e-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5b17e-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5b17e-164">solicitação</span><span class="sxs-lookup"><span data-stu-id="5b17e-164">request</span></span>|[<span data-ttu-id="5b17e-165">privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b17e-165">privilegedRoleAssignmentRequest</span></span>](privilegedroleassignmentrequest.md)| <span data-ttu-id="5b17e-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b17e-166">Read-only.</span></span> <span data-ttu-id="5b17e-167">A solicitação de atribuição de função para este objeto de aprovação</span><span class="sxs-lookup"><span data-stu-id="5b17e-167">The role assignment request for this approval object</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b17e-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b17e-168">JSON representation</span></span>
<span data-ttu-id="5b17e-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b17e-169">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->