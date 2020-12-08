---
title: tipo de recurso ediscoveryCase
description: as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 12d2901ff6a61213affd14d681c0ec7b6a74470c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597400"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="4c249-103">tipo de recurso ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-103">ediscoveryCase resource type</span></span>

<span data-ttu-id="4c249-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4c249-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c249-105">as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.</span><span class="sxs-lookup"><span data-stu-id="4c249-105">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="4c249-106">Saiba mais sobre casos e [descoberta eletrônica avançada](/microsoft-365/compliance/overview-ediscovery-20).</span><span class="sxs-lookup"><span data-stu-id="4c249-106">Learn more about cases and [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="4c249-107">Methods</span><span class="sxs-lookup"><span data-stu-id="4c249-107">Methods</span></span>

| <span data-ttu-id="4c249-108">Método</span><span class="sxs-lookup"><span data-stu-id="4c249-108">Method</span></span>       | <span data-ttu-id="4c249-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4c249-109">Return Type</span></span> | <span data-ttu-id="4c249-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c249-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4c249-111">Listar ediscoveryCases</span><span class="sxs-lookup"><span data-stu-id="4c249-111">List ediscoveryCases</span></span>](../api/ediscoverycase-list.md)          | <span data-ttu-id="4c249-112">coleção [ediscoveryCase](ediscoverycase.md)</span><span class="sxs-lookup"><span data-stu-id="4c249-112">[ediscoveryCase](ediscoverycase.md) collection</span></span>   | <span data-ttu-id="4c249-113">Obter uma lista de ocorrências de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4c249-113">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="4c249-114">Obter ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-114">Get ediscoveryCase</span></span>](../api/ediscoverycase-get.md)            | [<span data-ttu-id="4c249-115">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-115">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="4c249-116">Leia as propriedades do caso de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4c249-116">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="4c249-117">Criar ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-117">Create ediscoveryCase</span></span>](../api/ediscoverycase-post.md)        | [<span data-ttu-id="4c249-118">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-118">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="4c249-119">Criar um novo **ediscoveryCase** postando na coleção cases.</span><span class="sxs-lookup"><span data-stu-id="4c249-119">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="4c249-120">Atualizar ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-120">Update ediscoveryCase</span></span>](../api/ediscoverycase-update.md)      | [<span data-ttu-id="4c249-121">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-121">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="4c249-122">Atualize uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4c249-122">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="4c249-123">Excluir ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-123">Delete ediscoveryCase</span></span>](../api/ediscoverycase-delete.md)      | <span data-ttu-id="4c249-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c249-124">None</span></span>                                              | <span data-ttu-id="4c249-125">Excluir uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4c249-125">Delete an eDiscovery case.</span></span> |
| [<span data-ttu-id="4c249-126">Fechar ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-126">Close ediscoveryCase</span></span>](../api/ediscoverycase-close.md)        | <span data-ttu-id="4c249-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c249-127">None</span></span>                                              | <span data-ttu-id="4c249-128">Feche uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4c249-128">Close an eDiscovery case.</span></span> |
| [<span data-ttu-id="4c249-129">Reabrir ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="4c249-129">Reopen ediscoveryCase</span></span>](../api/ediscoverycase-reopen.md)      | <span data-ttu-id="4c249-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c249-130">None</span></span>                                              | <span data-ttu-id="4c249-131">Reabra uma ocorrência de descoberta eletrônica fechada.</span><span class="sxs-lookup"><span data-stu-id="4c249-131">Reopen a closed eDiscovery case.</span></span>|
| [<span data-ttu-id="4c249-132">Listar os responsáveis</span><span class="sxs-lookup"><span data-stu-id="4c249-132">List custodians</span></span>](../api/custodian-get.md)   | <span data-ttu-id="4c249-133">coleção [responsáveis](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="4c249-133">[custodian](../resources/custodian.md) collection</span></span> |<span data-ttu-id="4c249-134">Obtenha os recursos do responsáveis da propriedade de navegação responsáveis.</span><span class="sxs-lookup"><span data-stu-id="4c249-134">Get the custodian resources from the custodians navigation property.</span></span>|
| [<span data-ttu-id="4c249-135">Criar responsáveis</span><span class="sxs-lookup"><span data-stu-id="4c249-135">Create custodians</span></span>](../api/ediscoverycase-post-custodians.md)  | [<span data-ttu-id="4c249-136">custódia</span><span class="sxs-lookup"><span data-stu-id="4c249-136">custodian</span></span>](../resources/custodian.md)           |<span data-ttu-id="4c249-137">Criar um novo objeto de responsáveis.</span><span class="sxs-lookup"><span data-stu-id="4c249-137">Create a new custodian object.</span></span>|
| [<span data-ttu-id="4c249-138">Listar reviewSets</span><span class="sxs-lookup"><span data-stu-id="4c249-138">List reviewSets</span></span>](../api/reviewset-list.md)   | <span data-ttu-id="4c249-139">coleção [reviewset](../resources/reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="4c249-139">[reviewSet](../resources/reviewset.md) collection</span></span> | <span data-ttu-id="4c249-140">Obtenha os recursos reviewset da propriedade de navegação reviewSets.</span><span class="sxs-lookup"><span data-stu-id="4c249-140">Get the reviewSet resources from the reviewSets navigation property.</span></span>|
| [<span data-ttu-id="4c249-141">Criar reviewSets</span><span class="sxs-lookup"><span data-stu-id="4c249-141">Create reviewSets</span></span>](../api/reviewset-post.md)  | [<span data-ttu-id="4c249-142">reviewSet</span><span class="sxs-lookup"><span data-stu-id="4c249-142">reviewSet</span></span>](../resources/reviewset.md)           | <span data-ttu-id="4c249-143">Criar um novo objeto reviewset.</span><span class="sxs-lookup"><span data-stu-id="4c249-143">Create a new reviewSet object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c249-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c249-144">Properties</span></span>

| <span data-ttu-id="4c249-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c249-145">Property</span></span>     | <span data-ttu-id="4c249-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c249-146">Type</span></span>        | <span data-ttu-id="4c249-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c249-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c249-148">closedBy</span><span class="sxs-lookup"><span data-stu-id="4c249-148">closedBy</span></span>|[<span data-ttu-id="4c249-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="4c249-149">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="4c249-150">O usuário que fechou o caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-150">The user who closed the case.</span></span>|
|<span data-ttu-id="4c249-151">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c249-151">closedDateTime</span></span>|<span data-ttu-id="4c249-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c249-152">DateTimeOffset</span></span>|<span data-ttu-id="4c249-153">A data e a hora em que o caso foi fechado.</span><span class="sxs-lookup"><span data-stu-id="4c249-153">The date and time when the case was closed.</span></span> <span data-ttu-id="4c249-154">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4c249-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c249-155">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c249-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c249-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="4c249-156">createdBy</span></span>|[<span data-ttu-id="4c249-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="4c249-157">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="4c249-158">O usuário que criou a ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4c249-158">The user who created the case.</span></span>|
|<span data-ttu-id="4c249-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c249-159">createdDateTime</span></span>|<span data-ttu-id="4c249-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c249-160">DateTimeOffset</span></span>|<span data-ttu-id="4c249-161">A data e a hora em que a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="4c249-161">The date and time when the entity was created.</span></span> <span data-ttu-id="4c249-162">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4c249-162">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c249-163">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c249-163">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c249-164">description</span><span class="sxs-lookup"><span data-stu-id="4c249-164">description</span></span>|<span data-ttu-id="4c249-165">String</span><span class="sxs-lookup"><span data-stu-id="4c249-165">String</span></span>|<span data-ttu-id="4c249-166">A descrição do caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-166">The case description.</span></span>|
|<span data-ttu-id="4c249-167">displayName</span><span class="sxs-lookup"><span data-stu-id="4c249-167">displayName</span></span>|<span data-ttu-id="4c249-168">String</span><span class="sxs-lookup"><span data-stu-id="4c249-168">String</span></span>|<span data-ttu-id="4c249-169">O nome do caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-169">The case name.</span></span>|
|<span data-ttu-id="4c249-170">externalId</span><span class="sxs-lookup"><span data-stu-id="4c249-170">externalId</span></span>|<span data-ttu-id="4c249-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c249-171">String</span></span>|<span data-ttu-id="4c249-172">O número do caso externo para referência de cliente.</span><span class="sxs-lookup"><span data-stu-id="4c249-172">The external case number for customer reference.</span></span>|
|<span data-ttu-id="4c249-173">id</span><span class="sxs-lookup"><span data-stu-id="4c249-173">id</span></span>|<span data-ttu-id="4c249-174">String</span><span class="sxs-lookup"><span data-stu-id="4c249-174">String</span></span>| <span data-ttu-id="4c249-175">A ID da ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="4c249-175">The ID for the eDiscovery case.</span></span> <span data-ttu-id="4c249-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c249-176">Read-only.</span></span> |
|<span data-ttu-id="4c249-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4c249-177">lastModifiedBy</span></span>|[<span data-ttu-id="4c249-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="4c249-178">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="4c249-179">O último usuário que modificou a entidade.</span><span class="sxs-lookup"><span data-stu-id="4c249-179">The last user who modified the entity.</span></span>|
|<span data-ttu-id="4c249-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c249-180">lastModifiedDateTime</span></span>|<span data-ttu-id="4c249-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c249-181">DateTimeOffset</span></span>| <span data-ttu-id="4c249-182">A última data e hora em que a ocorrência foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4c249-182">The latest date and time when the case was modified.</span></span> <span data-ttu-id="4c249-183">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4c249-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c249-184">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c249-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c249-185">status</span><span class="sxs-lookup"><span data-stu-id="4c249-185">status</span></span>|<span data-ttu-id="4c249-186">String</span><span class="sxs-lookup"><span data-stu-id="4c249-186">String</span></span>| <span data-ttu-id="4c249-187">O status do caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-187">The case status.</span></span> <span data-ttu-id="4c249-188">Os valores possíveis são:,,, `unknown` `active` `pendingDelete` `closing` `closed` , e `closedWithError` .</span><span class="sxs-lookup"><span data-stu-id="4c249-188">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="4c249-189">Para obter detalhes, consulte a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="4c249-189">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="4c249-190">valores de caseStatus</span><span class="sxs-lookup"><span data-stu-id="4c249-190">caseStatus values</span></span>

|<span data-ttu-id="4c249-191">Member</span><span class="sxs-lookup"><span data-stu-id="4c249-191">Member</span></span>|<span data-ttu-id="4c249-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c249-192">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="4c249-193">desconhecido</span><span class="sxs-lookup"><span data-stu-id="4c249-193">unknown</span></span> | <span data-ttu-id="4c249-194">O status do caso é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="4c249-194">Case status is unknown.</span></span> |
| <span data-ttu-id="4c249-195">active</span><span class="sxs-lookup"><span data-stu-id="4c249-195">active</span></span> | <span data-ttu-id="4c249-196">O caso está ativo.</span><span class="sxs-lookup"><span data-stu-id="4c249-196">Case is active.</span></span> |
| <span data-ttu-id="4c249-197">pendingDelete</span><span class="sxs-lookup"><span data-stu-id="4c249-197">pendingDelete</span></span> | <span data-ttu-id="4c249-198">A ocorrência foi excluída, mas a exclusão não foi totalmente transacionada.</span><span class="sxs-lookup"><span data-stu-id="4c249-198">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="4c249-199">Feche</span><span class="sxs-lookup"><span data-stu-id="4c249-199">closing</span></span> | <span data-ttu-id="4c249-200">O caso foi fechado, mas a operação não foi totalmente transacionada.</span><span class="sxs-lookup"><span data-stu-id="4c249-200">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="4c249-201">sido</span><span class="sxs-lookup"><span data-stu-id="4c249-201">closed</span></span> | <span data-ttu-id="4c249-202">O caso é fechado.</span><span class="sxs-lookup"><span data-stu-id="4c249-202">The case is closed.</span></span> |
| <span data-ttu-id="4c249-203">closedWithError</span><span class="sxs-lookup"><span data-stu-id="4c249-203">closedWithError</span></span> | <span data-ttu-id="4c249-204">O caso está fechado, mas houve erros na liberação de isenções no caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-204">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4c249-205">Relações</span><span class="sxs-lookup"><span data-stu-id="4c249-205">Relationships</span></span>

| <span data-ttu-id="4c249-206">Relação</span><span class="sxs-lookup"><span data-stu-id="4c249-206">Relationship</span></span> | <span data-ttu-id="4c249-207">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c249-207">Type</span></span>        | <span data-ttu-id="4c249-208">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c249-208">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c249-209">responsáveis</span><span class="sxs-lookup"><span data-stu-id="4c249-209">custodians</span></span>|<span data-ttu-id="4c249-210">coleção [responsáveis](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="4c249-210">[custodian](../resources/custodian.md) collection</span></span>| <span data-ttu-id="4c249-211">Pessoas em uma organização que podem ter dados relevantes para o caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-211">People in an organization who may possess data relevant to the case.</span></span> |
|<span data-ttu-id="4c249-212">reviewSets</span><span class="sxs-lookup"><span data-stu-id="4c249-212">reviewSets</span></span>|<span data-ttu-id="4c249-213">coleção [reviewset](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="4c249-213">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="4c249-214">Coleção de conjuntos de análise no caso.</span><span class="sxs-lookup"><span data-stu-id="4c249-214">Collection of review sets in the case.</span></span> <span data-ttu-id="4c249-215">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c249-215">Read-only.</span></span> <span data-ttu-id="4c249-216">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4c249-216">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c249-217">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c249-217">JSON representation</span></span>

<span data-ttu-id="4c249-218">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c249-218">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ediscoveryCase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
