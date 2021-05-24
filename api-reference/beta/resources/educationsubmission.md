---
title: Tipo de recurso educationSubmission
description: Os envios pertencem a uma atribuição. Um envio representa os recursos que um indivíduo (ou grupo) entrega para uma atribuição e a nota/feedback que é retornada.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f468e0715a07320233db1224c3fcee62e0c8fe63
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629438"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="1d16c-104">Tipo de recurso educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-104">educationSubmission resource type</span></span>

<span data-ttu-id="1d16c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d16c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d16c-106">Um envio representa os recursos que um indivíduo (ou grupo) entrega para uma atribuição e os resultados (como notas ou comentários) associados ao envio.</span><span class="sxs-lookup"><span data-stu-id="1d16c-106">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>

<span data-ttu-id="1d16c-107">Os envios pertencem a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="1d16c-107">Submissions are owned by an assignment.</span></span> <span data-ttu-id="1d16c-108">Os envios são criados automaticamente quando uma atribuição é publicada.</span><span class="sxs-lookup"><span data-stu-id="1d16c-108">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="1d16c-109">O envio possui duas listas de recursos.</span><span class="sxs-lookup"><span data-stu-id="1d16c-109">The submission owns two lists of resources.</span></span> <span data-ttu-id="1d16c-110">Os recursos representam a área de trabalho usuário/grupos enquanto os recursos enviados representam os recursos que foram ativamente entregues pelos alunos.</span><span class="sxs-lookup"><span data-stu-id="1d16c-110">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

<span data-ttu-id="1d16c-111">A **propriedade status** é somente leitura e o objeto é movido através do fluxo de trabalho por meio de ações.</span><span class="sxs-lookup"><span data-stu-id="1d16c-111">The **status** property is read-only and the object is moved through the workflow via actions.</span></span> 

<span data-ttu-id="1d16c-112">Se [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) não tiver sido chamado em um **recurso educationSubmission,** a propriedade **resourcesFolderUrl** será `null` .</span><span class="sxs-lookup"><span data-stu-id="1d16c-112">If [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) has not been called on an **educationSubmission** resource, the **resourcesFolderUrl** property is `null`.</span></span>

## <a name="methods"></a><span data-ttu-id="1d16c-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d16c-113">Methods</span></span>

| <span data-ttu-id="1d16c-114">Método</span><span class="sxs-lookup"><span data-stu-id="1d16c-114">Method</span></span>           | <span data-ttu-id="1d16c-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d16c-115">Return Type</span></span>    |<span data-ttu-id="1d16c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d16c-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d16c-117">Obter educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-117">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="1d16c-118">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-118">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="1d16c-119">Leia propriedades e relações de um **objeto educationSubmission.**</span><span class="sxs-lookup"><span data-stu-id="1d16c-119">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="1d16c-120">Listar recursos</span><span class="sxs-lookup"><span data-stu-id="1d16c-120">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="1d16c-121">[Coleção educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="1d16c-121">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="1d16c-122">Obter uma **coleção de objetos educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="1d16c-122">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="1d16c-123">Listar submittedResources</span><span class="sxs-lookup"><span data-stu-id="1d16c-123">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="1d16c-124">[Coleção educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="1d16c-124">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="1d16c-125">Obter uma **coleção de objetos educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="1d16c-125">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="1d16c-126">Listar resultados</span><span class="sxs-lookup"><span data-stu-id="1d16c-126">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="1d16c-127">[Coleção educationOutcome](educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="1d16c-127">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="1d16c-128">Obter uma **coleção de objetos educationOutcome.**</span><span class="sxs-lookup"><span data-stu-id="1d16c-128">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="1d16c-129">return</span><span class="sxs-lookup"><span data-stu-id="1d16c-129">return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="1d16c-130">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-130">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="1d16c-131">Um professor usa o retorno para indicar que as notas/comentários podem ser mostradas ao aluno.</span><span class="sxs-lookup"><span data-stu-id="1d16c-131">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="1d16c-132">Configurar pasta de recursos específicos do envio</span><span class="sxs-lookup"><span data-stu-id="1d16c-132">Set up submission specific resources folder</span></span>](../api/educationsubmission-setupResourcesFolder.md) |[<span data-ttu-id="1d16c-133">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-133">educationSubmission</span></span>](educationsubmission.md) | <span data-ttu-id="1d16c-134">Crie uma SharePoint (em local pré-definido) para carregar arquivos como recursos de envio.</span><span class="sxs-lookup"><span data-stu-id="1d16c-134">Create a SharePoint folder (under pre-defined location) to upload files as submission resources.</span></span> |
|[<span data-ttu-id="1d16c-135">Enviar</span><span class="sxs-lookup"><span data-stu-id="1d16c-135">submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="1d16c-136">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-136">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="1d16c-137">Um aluno usa enviar para entregar a atribuição.</span><span class="sxs-lookup"><span data-stu-id="1d16c-137">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="1d16c-138">Isso copiará os recursos para a **pasta submittedResources** para a classificação e atualiza o status.</span><span class="sxs-lookup"><span data-stu-id="1d16c-138">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="1d16c-139">unsubmit</span><span class="sxs-lookup"><span data-stu-id="1d16c-139">unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="1d16c-140">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1d16c-140">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="1d16c-141">Um aluno usa o cancelamento para mover o estado do envio do envio de volta ao trabalho.</span><span class="sxs-lookup"><span data-stu-id="1d16c-141">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="1d16c-142">Isso copiará os recursos para a **pasta workingResources** para a classificação e atualiza o status.</span><span class="sxs-lookup"><span data-stu-id="1d16c-142">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d16c-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d16c-143">Properties</span></span>
| <span data-ttu-id="1d16c-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d16c-144">Property</span></span>     | <span data-ttu-id="1d16c-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d16c-145">Type</span></span>   |<span data-ttu-id="1d16c-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d16c-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d16c-147">destinatário</span><span class="sxs-lookup"><span data-stu-id="1d16c-147">recipient</span></span>|[<span data-ttu-id="1d16c-148">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="1d16c-148">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="1d16c-149">Who esse envio é atribuído.</span><span class="sxs-lookup"><span data-stu-id="1d16c-149">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="1d16c-150">returnedBy</span><span class="sxs-lookup"><span data-stu-id="1d16c-150">returnedBy</span></span>|[<span data-ttu-id="1d16c-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d16c-151">identitySet</span></span>](identityset.md)|<span data-ttu-id="1d16c-152">Usuário que moveu o status desse envio para retornado.</span><span class="sxs-lookup"><span data-stu-id="1d16c-152">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="1d16c-153">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d16c-153">returnedDateTime</span></span>|<span data-ttu-id="1d16c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d16c-154">DateTimeOffset</span></span>|<span data-ttu-id="1d16c-155">Momento no tempo em que o envio foi retornado.</span><span class="sxs-lookup"><span data-stu-id="1d16c-155">Moment in time when the submission was returned.</span></span> <span data-ttu-id="1d16c-156">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1d16c-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d16c-157">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1d16c-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1d16c-158">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="1d16c-158">resourcesFolderUrl</span></span>|<span data-ttu-id="1d16c-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d16c-159">String</span></span>|<span data-ttu-id="1d16c-160">Pasta onde todos os recursos de arquivo para esse envio precisam ser armazenados.</span><span class="sxs-lookup"><span data-stu-id="1d16c-160">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="1d16c-161">status</span><span class="sxs-lookup"><span data-stu-id="1d16c-161">status</span></span>|<span data-ttu-id="1d16c-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d16c-162">string</span></span>| <span data-ttu-id="1d16c-163">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1d16c-163">Read-Only.</span></span> <span data-ttu-id="1d16c-164">Os valores possíveis são: `working`, `submitted`, `released`, `returned`.</span><span class="sxs-lookup"><span data-stu-id="1d16c-164">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="1d16c-165">submittedBy</span><span class="sxs-lookup"><span data-stu-id="1d16c-165">submittedBy</span></span>|[<span data-ttu-id="1d16c-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d16c-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="1d16c-167">Usuário que moveu o recurso para o estado enviado.</span><span class="sxs-lookup"><span data-stu-id="1d16c-167">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="1d16c-168">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d16c-168">submittedDateTime</span></span>|<span data-ttu-id="1d16c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d16c-169">DateTimeOffset</span></span>|<span data-ttu-id="1d16c-170">Momento no tempo em que o envio foi movido para o estado enviado.</span><span class="sxs-lookup"><span data-stu-id="1d16c-170">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="1d16c-171">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1d16c-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d16c-172">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1d16c-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1d16c-173">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="1d16c-173">unsubmittedBy</span></span>|[<span data-ttu-id="1d16c-174">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d16c-174">identitySet</span></span>](identityset.md)|<span data-ttu-id="1d16c-175">Usuário que moveu o recurso de enviado para o estado de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1d16c-175">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="1d16c-176">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d16c-176">unsubmittedDateTime</span></span>|<span data-ttu-id="1d16c-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d16c-177">DateTimeOffset</span></span>|<span data-ttu-id="1d16c-178">Momento no tempo em que o envio foi movido do envio para o estado de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1d16c-178">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="1d16c-179">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1d16c-179">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d16c-180">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1d16c-180">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d16c-181">Relações</span><span class="sxs-lookup"><span data-stu-id="1d16c-181">Relationships</span></span>
| <span data-ttu-id="1d16c-182">Relação</span><span class="sxs-lookup"><span data-stu-id="1d16c-182">Relationship</span></span> | <span data-ttu-id="1d16c-183">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d16c-183">Type</span></span>   |<span data-ttu-id="1d16c-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d16c-184">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d16c-185">recursos</span><span class="sxs-lookup"><span data-stu-id="1d16c-185">resources</span></span>|<span data-ttu-id="1d16c-186">[Coleção educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="1d16c-186">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="1d16c-187">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1d16c-187">Nullable.</span></span>|
|<span data-ttu-id="1d16c-188">submittedResources</span><span class="sxs-lookup"><span data-stu-id="1d16c-188">submittedResources</span></span>|<span data-ttu-id="1d16c-189">[Coleção educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="1d16c-189">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="1d16c-p109">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1d16c-p109">Read-only. Nullable.</span></span>|
|<span data-ttu-id="1d16c-192">outcomes</span><span class="sxs-lookup"><span data-stu-id="1d16c-192">outcomes</span></span>|<span data-ttu-id="1d16c-193">[Coleção educationOutcome.](educationOutcome.md)</span><span class="sxs-lookup"><span data-stu-id="1d16c-193">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="1d16c-194">Contém notas, comentários e/ou informações rubricas que o professor atribui a esse envio</span><span class="sxs-lookup"><span data-stu-id="1d16c-194">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="1d16c-195">Leitura-Gravação.</span><span class="sxs-lookup"><span data-stu-id="1d16c-195">Read-Write.</span></span> <span data-ttu-id="1d16c-196">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1d16c-196">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d16c-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d16c-197">JSON representation</span></span>

<span data-ttu-id="1d16c-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d16c-198">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


