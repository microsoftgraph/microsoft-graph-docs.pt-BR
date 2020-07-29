---
title: tipo de recurso ediscoveryCase
description: as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 930d04449f24d05d8c9225869506bfc1ed2720aa
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509963"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="ab2ec-103">tipo de recurso ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="ab2ec-103">ediscoveryCase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2ec-104">as ocorrências de descoberta eletrônica são contêineres que contêm responsáveis, isenções, coleções, conjuntos de revisão e exportações.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-104">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="ab2ec-105">Saiba mais sobre casos e [descoberta eletrônica avançada](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span><span class="sxs-lookup"><span data-stu-id="ab2ec-105">Learn more about cases and [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="ab2ec-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab2ec-106">Methods</span></span>

| <span data-ttu-id="ab2ec-107">Método</span><span class="sxs-lookup"><span data-stu-id="ab2ec-107">Method</span></span>       | <span data-ttu-id="ab2ec-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab2ec-108">Return Type</span></span> | <span data-ttu-id="ab2ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2ec-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ab2ec-110">Listar</span><span class="sxs-lookup"><span data-stu-id="ab2ec-110">List</span></span>](../api/ediscoverycase-list.md) | <span data-ttu-id="ab2ec-111">coleção [ediscoveryCase](ediscoverycase.md)</span><span class="sxs-lookup"><span data-stu-id="ab2ec-111">[ediscoveryCase](ediscoverycase.md) collection</span></span> | <span data-ttu-id="ab2ec-112">Obter uma lista de ocorrências de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-112">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="ab2ec-113">Get</span><span class="sxs-lookup"><span data-stu-id="ab2ec-113">Get</span></span>](../api/ediscoverycase-get.md) | [<span data-ttu-id="ab2ec-114">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="ab2ec-114">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="ab2ec-115">Leia as propriedades do caso de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-115">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="ab2ec-116">Create</span><span class="sxs-lookup"><span data-stu-id="ab2ec-116">Create</span></span>](../api/ediscoverycase-post.md) | [<span data-ttu-id="ab2ec-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="ab2ec-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="ab2ec-118">Criar um novo **ediscoveryCase** postando na coleção cases.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-118">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="ab2ec-119">Update</span><span class="sxs-lookup"><span data-stu-id="ab2ec-119">Update</span></span>](../api/ediscoverycase-update.md) | [<span data-ttu-id="ab2ec-120">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="ab2ec-120">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="ab2ec-121">Atualize uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-121">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="ab2ec-122">Delete</span><span class="sxs-lookup"><span data-stu-id="ab2ec-122">Delete</span></span>](../api/ediscoverycase-delete.md) | <span data-ttu-id="ab2ec-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab2ec-123">None</span></span> | <span data-ttu-id="ab2ec-124">Excluir uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-124">Delete an eDiscovery case.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab2ec-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab2ec-125">Properties</span></span>

| <span data-ttu-id="ab2ec-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab2ec-126">Property</span></span>     | <span data-ttu-id="ab2ec-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab2ec-127">Type</span></span>        | <span data-ttu-id="ab2ec-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2ec-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab2ec-129">closedBy</span><span class="sxs-lookup"><span data-stu-id="ab2ec-129">closedBy</span></span>|[<span data-ttu-id="ab2ec-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab2ec-130">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="ab2ec-131">O usuário que fechou o caso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-131">The user who closed the case.</span></span>|
|<span data-ttu-id="ab2ec-132">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2ec-132">closedDateTime</span></span>|<span data-ttu-id="ab2ec-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2ec-133">DateTimeOffset</span></span>|<span data-ttu-id="ab2ec-134">A data e a hora em que o caso foi fechado.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-134">The date and time when the case was closed.</span></span> <span data-ttu-id="ab2ec-135">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab2ec-136">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ab2ec-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ab2ec-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="ab2ec-137">createdBy</span></span>|[<span data-ttu-id="ab2ec-138">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab2ec-138">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="ab2ec-139">O usuário que criou a ocorrência.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-139">The user who created the case.</span></span>|
|<span data-ttu-id="ab2ec-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2ec-140">createdDateTime</span></span>|<span data-ttu-id="ab2ec-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2ec-141">DateTimeOffset</span></span>|<span data-ttu-id="ab2ec-142">A data e a hora em que a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-142">The date and time when the entity was created.</span></span> <span data-ttu-id="ab2ec-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab2ec-144">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ab2ec-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ab2ec-145">description</span><span class="sxs-lookup"><span data-stu-id="ab2ec-145">description</span></span>|<span data-ttu-id="ab2ec-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab2ec-146">String</span></span>|<span data-ttu-id="ab2ec-147">A descrição do caso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-147">The case description.</span></span>|
|<span data-ttu-id="ab2ec-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ab2ec-148">displayName</span></span>|<span data-ttu-id="ab2ec-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab2ec-149">String</span></span>|<span data-ttu-id="ab2ec-150">O nome do caso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-150">The case name.</span></span>|
|<span data-ttu-id="ab2ec-151">externalId</span><span class="sxs-lookup"><span data-stu-id="ab2ec-151">externalId</span></span>|<span data-ttu-id="ab2ec-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab2ec-152">String</span></span>|<span data-ttu-id="ab2ec-153">O número do caso externo para referência de cliente.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-153">The external case number for customer reference.</span></span>|
|<span data-ttu-id="ab2ec-154">id</span><span class="sxs-lookup"><span data-stu-id="ab2ec-154">id</span></span>|<span data-ttu-id="ab2ec-155">String</span><span class="sxs-lookup"><span data-stu-id="ab2ec-155">String</span></span>| <span data-ttu-id="ab2ec-156">A ID da ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-156">The ID for the eDiscovery case.</span></span> <span data-ttu-id="ab2ec-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-157">Read-only.</span></span> |
|<span data-ttu-id="ab2ec-158">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ab2ec-158">lastModifiedBy</span></span>|[<span data-ttu-id="ab2ec-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab2ec-159">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="ab2ec-160">O último usuário que modificou a entidade.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-160">The last user who modified the entity.</span></span>|
|<span data-ttu-id="ab2ec-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2ec-161">lastModifiedDateTime</span></span>|<span data-ttu-id="ab2ec-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2ec-162">DateTimeOffset</span></span>| <span data-ttu-id="ab2ec-163">A última data e hora em que a ocorrência foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-163">The latest date and time when the case was modified.</span></span> <span data-ttu-id="ab2ec-164">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab2ec-165">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ab2ec-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ab2ec-166">status</span><span class="sxs-lookup"><span data-stu-id="ab2ec-166">status</span></span>|<span data-ttu-id="ab2ec-167">String</span><span class="sxs-lookup"><span data-stu-id="ab2ec-167">String</span></span>| <span data-ttu-id="ab2ec-168">O status do caso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-168">The case status.</span></span> <span data-ttu-id="ab2ec-169">Os valores possíveis são:,,, `unknown` `active` `pendingDelete` `closing` `closed` , e `closedWithError` .</span><span class="sxs-lookup"><span data-stu-id="ab2ec-169">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="ab2ec-170">Para obter detalhes, consulte a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-170">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="ab2ec-171">valores de caseStatus</span><span class="sxs-lookup"><span data-stu-id="ab2ec-171">caseStatus values</span></span>

|<span data-ttu-id="ab2ec-172">Member</span><span class="sxs-lookup"><span data-stu-id="ab2ec-172">Member</span></span>|<span data-ttu-id="ab2ec-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2ec-173">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="ab2ec-174">desconhecido</span><span class="sxs-lookup"><span data-stu-id="ab2ec-174">unknown</span></span> | <span data-ttu-id="ab2ec-175">O status do caso é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-175">Case status is unknown.</span></span> |
| <span data-ttu-id="ab2ec-176">active</span><span class="sxs-lookup"><span data-stu-id="ab2ec-176">active</span></span> | <span data-ttu-id="ab2ec-177">O caso está ativo.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-177">Case is active.</span></span> |
| <span data-ttu-id="ab2ec-178">pendingDelete</span><span class="sxs-lookup"><span data-stu-id="ab2ec-178">pendingDelete</span></span> | <span data-ttu-id="ab2ec-179">A ocorrência foi excluída, mas a exclusão não foi totalmente transacionada.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-179">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="ab2ec-180">Feche</span><span class="sxs-lookup"><span data-stu-id="ab2ec-180">closing</span></span> | <span data-ttu-id="ab2ec-181">O caso foi fechado, mas a operação não foi totalmente transacionada.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-181">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="ab2ec-182">sido</span><span class="sxs-lookup"><span data-stu-id="ab2ec-182">closed</span></span> | <span data-ttu-id="ab2ec-183">O caso é fechado.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-183">The case is closed.</span></span> |
| <span data-ttu-id="ab2ec-184">closedWithError</span><span class="sxs-lookup"><span data-stu-id="ab2ec-184">closedWithError</span></span> | <span data-ttu-id="ab2ec-185">O caso está fechado, mas houve erros na liberação de isenções no caso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-185">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ab2ec-186">Relações</span><span class="sxs-lookup"><span data-stu-id="ab2ec-186">Relationships</span></span>

| <span data-ttu-id="ab2ec-187">Relação</span><span class="sxs-lookup"><span data-stu-id="ab2ec-187">Relationship</span></span> | <span data-ttu-id="ab2ec-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab2ec-188">Type</span></span>        | <span data-ttu-id="ab2ec-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2ec-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab2ec-190">Revisar conjuntos</span><span class="sxs-lookup"><span data-stu-id="ab2ec-190">Review sets</span></span>|<span data-ttu-id="ab2ec-191">coleção [reviewset](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="ab2ec-191">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="ab2ec-192">Coleção de conjuntos de análise no caso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-192">Collection of review sets in the case.</span></span> <span data-ttu-id="ab2ec-193">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-193">Read-only.</span></span> <span data-ttu-id="ab2ec-194">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-194">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab2ec-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab2ec-195">JSON representation</span></span>

<span data-ttu-id="ab2ec-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab2ec-196">The following is a JSON representation of the resource.</span></span>

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
