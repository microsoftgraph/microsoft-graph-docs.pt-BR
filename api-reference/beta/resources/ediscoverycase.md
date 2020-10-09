---
title: tipo de recurso ediscoveryCase
description: as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 8fac6cfa8de0533c936c9d8d03a6173f06d0886f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404788"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="7c544-103">tipo de recurso ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="7c544-103">ediscoveryCase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c544-104">as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.</span><span class="sxs-lookup"><span data-stu-id="7c544-104">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="7c544-105">Saiba mais sobre casos e [descoberta eletrônica avançada](/microsoft-365/compliance/overview-ediscovery-20).</span><span class="sxs-lookup"><span data-stu-id="7c544-105">Learn more about cases and [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="7c544-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7c544-106">Methods</span></span>

| <span data-ttu-id="7c544-107">Método</span><span class="sxs-lookup"><span data-stu-id="7c544-107">Method</span></span>       | <span data-ttu-id="7c544-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7c544-108">Return Type</span></span> | <span data-ttu-id="7c544-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c544-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7c544-110">List</span><span class="sxs-lookup"><span data-stu-id="7c544-110">List</span></span>](../api/ediscoverycase-list.md) | <span data-ttu-id="7c544-111">coleção [ediscoveryCase](ediscoverycase.md)</span><span class="sxs-lookup"><span data-stu-id="7c544-111">[ediscoveryCase](ediscoverycase.md) collection</span></span> | <span data-ttu-id="7c544-112">Obter uma lista de ocorrências de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="7c544-112">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="7c544-113">Get</span><span class="sxs-lookup"><span data-stu-id="7c544-113">Get</span></span>](../api/ediscoverycase-get.md) | [<span data-ttu-id="7c544-114">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="7c544-114">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="7c544-115">Leia as propriedades do caso de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="7c544-115">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="7c544-116">Create</span><span class="sxs-lookup"><span data-stu-id="7c544-116">Create</span></span>](../api/ediscoverycase-post.md) | [<span data-ttu-id="7c544-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="7c544-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="7c544-118">Criar um novo **ediscoveryCase** postando na coleção cases.</span><span class="sxs-lookup"><span data-stu-id="7c544-118">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="7c544-119">Update</span><span class="sxs-lookup"><span data-stu-id="7c544-119">Update</span></span>](../api/ediscoverycase-update.md) | [<span data-ttu-id="7c544-120">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="7c544-120">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="7c544-121">Atualize uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="7c544-121">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="7c544-122">Delete</span><span class="sxs-lookup"><span data-stu-id="7c544-122">Delete</span></span>](../api/ediscoverycase-delete.md) | <span data-ttu-id="7c544-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c544-123">None</span></span> | <span data-ttu-id="7c544-124">Excluir uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="7c544-124">Delete an eDiscovery case.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c544-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c544-125">Properties</span></span>

| <span data-ttu-id="7c544-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c544-126">Property</span></span>     | <span data-ttu-id="7c544-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c544-127">Type</span></span>        | <span data-ttu-id="7c544-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c544-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c544-129">closedBy</span><span class="sxs-lookup"><span data-stu-id="7c544-129">closedBy</span></span>|[<span data-ttu-id="7c544-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="7c544-130">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="7c544-131">O usuário que fechou o caso.</span><span class="sxs-lookup"><span data-stu-id="7c544-131">The user who closed the case.</span></span>|
|<span data-ttu-id="7c544-132">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c544-132">closedDateTime</span></span>|<span data-ttu-id="7c544-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c544-133">DateTimeOffset</span></span>|<span data-ttu-id="7c544-134">A data e a hora em que o caso foi fechado.</span><span class="sxs-lookup"><span data-stu-id="7c544-134">The date and time when the case was closed.</span></span> <span data-ttu-id="7c544-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7c544-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c544-136">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7c544-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7c544-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="7c544-137">createdBy</span></span>|[<span data-ttu-id="7c544-138">identitySet</span><span class="sxs-lookup"><span data-stu-id="7c544-138">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="7c544-139">O usuário que criou a ocorrência.</span><span class="sxs-lookup"><span data-stu-id="7c544-139">The user who created the case.</span></span>|
|<span data-ttu-id="7c544-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c544-140">createdDateTime</span></span>|<span data-ttu-id="7c544-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c544-141">DateTimeOffset</span></span>|<span data-ttu-id="7c544-142">A data e a hora em que a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="7c544-142">The date and time when the entity was created.</span></span> <span data-ttu-id="7c544-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7c544-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c544-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7c544-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7c544-145">description</span><span class="sxs-lookup"><span data-stu-id="7c544-145">description</span></span>|<span data-ttu-id="7c544-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c544-146">String</span></span>|<span data-ttu-id="7c544-147">A descrição do caso.</span><span class="sxs-lookup"><span data-stu-id="7c544-147">The case description.</span></span>|
|<span data-ttu-id="7c544-148">displayName</span><span class="sxs-lookup"><span data-stu-id="7c544-148">displayName</span></span>|<span data-ttu-id="7c544-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c544-149">String</span></span>|<span data-ttu-id="7c544-150">O nome do caso.</span><span class="sxs-lookup"><span data-stu-id="7c544-150">The case name.</span></span>|
|<span data-ttu-id="7c544-151">externalId</span><span class="sxs-lookup"><span data-stu-id="7c544-151">externalId</span></span>|<span data-ttu-id="7c544-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c544-152">String</span></span>|<span data-ttu-id="7c544-153">O número do caso externo para referência de cliente.</span><span class="sxs-lookup"><span data-stu-id="7c544-153">The external case number for customer reference.</span></span>|
|<span data-ttu-id="7c544-154">id</span><span class="sxs-lookup"><span data-stu-id="7c544-154">id</span></span>|<span data-ttu-id="7c544-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c544-155">String</span></span>| <span data-ttu-id="7c544-156">A ID da ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="7c544-156">The ID for the eDiscovery case.</span></span> <span data-ttu-id="7c544-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c544-157">Read-only.</span></span> |
|<span data-ttu-id="7c544-158">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7c544-158">lastModifiedBy</span></span>|[<span data-ttu-id="7c544-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="7c544-159">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="7c544-160">O último usuário que modificou a entidade.</span><span class="sxs-lookup"><span data-stu-id="7c544-160">The last user who modified the entity.</span></span>|
|<span data-ttu-id="7c544-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c544-161">lastModifiedDateTime</span></span>|<span data-ttu-id="7c544-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c544-162">DateTimeOffset</span></span>| <span data-ttu-id="7c544-163">A última data e hora em que a ocorrência foi modificada.</span><span class="sxs-lookup"><span data-stu-id="7c544-163">The latest date and time when the case was modified.</span></span> <span data-ttu-id="7c544-164">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7c544-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c544-165">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7c544-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7c544-166">status</span><span class="sxs-lookup"><span data-stu-id="7c544-166">status</span></span>|<span data-ttu-id="7c544-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c544-167">String</span></span>| <span data-ttu-id="7c544-168">O status do caso.</span><span class="sxs-lookup"><span data-stu-id="7c544-168">The case status.</span></span> <span data-ttu-id="7c544-169">Os valores possíveis são:,,, `unknown` `active` `pendingDelete` `closing` `closed` , e `closedWithError` .</span><span class="sxs-lookup"><span data-stu-id="7c544-169">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="7c544-170">Para obter detalhes, consulte a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7c544-170">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="7c544-171">valores de caseStatus</span><span class="sxs-lookup"><span data-stu-id="7c544-171">caseStatus values</span></span>

|<span data-ttu-id="7c544-172">Member</span><span class="sxs-lookup"><span data-stu-id="7c544-172">Member</span></span>|<span data-ttu-id="7c544-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c544-173">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="7c544-174">desconhecido</span><span class="sxs-lookup"><span data-stu-id="7c544-174">unknown</span></span> | <span data-ttu-id="7c544-175">O status do caso é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7c544-175">Case status is unknown.</span></span> |
| <span data-ttu-id="7c544-176">active</span><span class="sxs-lookup"><span data-stu-id="7c544-176">active</span></span> | <span data-ttu-id="7c544-177">O caso está ativo.</span><span class="sxs-lookup"><span data-stu-id="7c544-177">Case is active.</span></span> |
| <span data-ttu-id="7c544-178">pendingDelete</span><span class="sxs-lookup"><span data-stu-id="7c544-178">pendingDelete</span></span> | <span data-ttu-id="7c544-179">A ocorrência foi excluída, mas a exclusão não foi totalmente transacionada.</span><span class="sxs-lookup"><span data-stu-id="7c544-179">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="7c544-180">Feche</span><span class="sxs-lookup"><span data-stu-id="7c544-180">closing</span></span> | <span data-ttu-id="7c544-181">O caso foi fechado, mas a operação não foi totalmente transacionada.</span><span class="sxs-lookup"><span data-stu-id="7c544-181">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="7c544-182">sido</span><span class="sxs-lookup"><span data-stu-id="7c544-182">closed</span></span> | <span data-ttu-id="7c544-183">O caso é fechado.</span><span class="sxs-lookup"><span data-stu-id="7c544-183">The case is closed.</span></span> |
| <span data-ttu-id="7c544-184">closedWithError</span><span class="sxs-lookup"><span data-stu-id="7c544-184">closedWithError</span></span> | <span data-ttu-id="7c544-185">O caso está fechado, mas houve erros na liberação de isenções no caso.</span><span class="sxs-lookup"><span data-stu-id="7c544-185">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7c544-186">Relações</span><span class="sxs-lookup"><span data-stu-id="7c544-186">Relationships</span></span>

| <span data-ttu-id="7c544-187">Relação</span><span class="sxs-lookup"><span data-stu-id="7c544-187">Relationship</span></span> | <span data-ttu-id="7c544-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c544-188">Type</span></span>        | <span data-ttu-id="7c544-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c544-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c544-190">Revisar conjuntos</span><span class="sxs-lookup"><span data-stu-id="7c544-190">Review sets</span></span>|<span data-ttu-id="7c544-191">coleção [reviewset](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="7c544-191">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="7c544-192">Coleção de conjuntos de análise no caso.</span><span class="sxs-lookup"><span data-stu-id="7c544-192">Collection of review sets in the case.</span></span> <span data-ttu-id="7c544-193">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c544-193">Read-only.</span></span> <span data-ttu-id="7c544-194">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7c544-194">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c544-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c544-195">JSON representation</span></span>

<span data-ttu-id="7c544-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c544-196">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "closedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "closedDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
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