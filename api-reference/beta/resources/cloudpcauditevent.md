---
title: Tipo de recurso cloudPcAuditEvent
description: Representa a entidade de evento de auditoria.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a863ea4128b7383c70bd14f025fcc5ce116dda25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211193"
---
# <a name="cloudpcauditevent-resource-type"></a><span data-ttu-id="f4711-103">Tipo de recurso cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="f4711-103">cloudPcAuditEvent resource type</span></span>

<span data-ttu-id="f4711-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4711-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4711-105">Representa a entidade de evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f4711-105">Represents the audit event entity.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="f4711-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4711-106">Methods</span></span>

|<span data-ttu-id="f4711-107">Método</span><span class="sxs-lookup"><span data-stu-id="f4711-107">Method</span></span>|<span data-ttu-id="f4711-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4711-108">Return type</span></span>|<span data-ttu-id="f4711-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4711-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4711-110">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="f4711-110">List auditEvents</span></span>](../api/virtualendpoint-list-auditevents.md)|<span data-ttu-id="f4711-111">[Coleção cloudPcAuditEvent](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="f4711-111">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) collection</span></span>|<span data-ttu-id="f4711-112">Listar todos os [objetos cloudPcAuditEvent](../resources/cloudpcauditevent.md) em um locatário.</span><span class="sxs-lookup"><span data-stu-id="f4711-112">List all the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects in a tenant.</span></span>|
|[<span data-ttu-id="f4711-113">Obter cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="f4711-113">Get cloudPcAuditEvent</span></span>](../api/cloudpcauditevent-get.md)|[<span data-ttu-id="f4711-114">cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="f4711-114">cloudPcAuditEvent</span></span>](../resources/cloudpcauditevent.md)|<span data-ttu-id="f4711-115">Leia as propriedades e as relações de um [objeto cloudPcAuditEvent.](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="f4711-115">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>|
|[<span data-ttu-id="f4711-116">Função getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="f4711-116">getAuditActivityTypes function</span></span>](../api/cloudpcauditevent-getauditactivitytypes.md)|<span data-ttu-id="f4711-117">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4711-117">String collection</span></span>|<span data-ttu-id="f4711-118">Obter tipos de atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f4711-118">Get audit activity types.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4711-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4711-119">Properties</span></span>

|<span data-ttu-id="f4711-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4711-120">Property</span></span>|<span data-ttu-id="f4711-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4711-121">Type</span></span>|<span data-ttu-id="f4711-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4711-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4711-123">id</span><span class="sxs-lookup"><span data-stu-id="f4711-123">id</span></span>|<span data-ttu-id="f4711-124">String</span><span class="sxs-lookup"><span data-stu-id="f4711-124">String</span></span>|<span data-ttu-id="f4711-125">Chave da entidade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f4711-125">Key of the audit entity.</span></span> <span data-ttu-id="f4711-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-126">Read-only.</span></span>|
|<span data-ttu-id="f4711-127">displayName</span><span class="sxs-lookup"><span data-stu-id="f4711-127">displayName</span></span>|<span data-ttu-id="f4711-128">String</span><span class="sxs-lookup"><span data-stu-id="f4711-128">String</span></span>|<span data-ttu-id="f4711-129">Nome de exibição do evento.</span><span class="sxs-lookup"><span data-stu-id="f4711-129">Event display name.</span></span> <span data-ttu-id="f4711-130">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-130">Read-only.</span></span>|
|<span data-ttu-id="f4711-131">componentName</span><span class="sxs-lookup"><span data-stu-id="f4711-131">componentName</span></span>|<span data-ttu-id="f4711-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4711-132">String</span></span>|<span data-ttu-id="f4711-133">Nome do componente.</span><span class="sxs-lookup"><span data-stu-id="f4711-133">Component name.</span></span> <span data-ttu-id="f4711-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-134">Read-only.</span></span>|
|<span data-ttu-id="f4711-135">actor</span><span class="sxs-lookup"><span data-stu-id="f4711-135">actor</span></span>|[<span data-ttu-id="f4711-136">cloudPcAuditActor</span><span class="sxs-lookup"><span data-stu-id="f4711-136">cloudPcAuditActor</span></span>](../resources/cloudpcauditactor.md)|<span data-ttu-id="f4711-137">Usuário e aplicativo do Azure AD associados ao evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f4711-137">Azure AD user and application associated with the audit event.</span></span> <span data-ttu-id="f4711-138">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-138">Read-only.</span></span>|
|<span data-ttu-id="f4711-139">atividade</span><span class="sxs-lookup"><span data-stu-id="f4711-139">activity</span></span>|<span data-ttu-id="f4711-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4711-140">String</span></span>|<span data-ttu-id="f4711-141">Nome amigável da atividade.</span><span class="sxs-lookup"><span data-stu-id="f4711-141">Friendly name of the activity.</span></span><span data-ttu-id="f4711-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f4711-142"> Optional.</span></span>|
|<span data-ttu-id="f4711-143">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="f4711-143">activityDateTime</span></span>|<span data-ttu-id="f4711-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4711-144">DateTimeOffset</span></span>|<span data-ttu-id="f4711-145">A hora e data em UTC em que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="f4711-145">The date time in UTC when the activity was performed.</span></span><span data-ttu-id="f4711-146">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-146"> Read-only.</span></span>|
|<span data-ttu-id="f4711-147">activityType</span><span class="sxs-lookup"><span data-stu-id="f4711-147">activityType</span></span>|<span data-ttu-id="f4711-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4711-148">String</span></span>|<span data-ttu-id="f4711-149">O tipo de atividade que foi realizada.</span><span class="sxs-lookup"><span data-stu-id="f4711-149">The type of activity that was performed.</span></span><span data-ttu-id="f4711-150">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-150"> Read-only.</span></span>|
|<span data-ttu-id="f4711-151">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="f4711-151">activityOperationType</span></span>|[<span data-ttu-id="f4711-152">cloudPcAuditActivityOperationType</span><span class="sxs-lookup"><span data-stu-id="f4711-152">cloudPcAuditActivityOperationType</span></span>](#cloudpcauditactivityoperationtype-values)|<span data-ttu-id="f4711-153">O tipo de operação HTTP da atividade.</span><span class="sxs-lookup"><span data-stu-id="f4711-153">The HTTP operation type of the activity.</span></span> <span data-ttu-id="f4711-154">Os valores possíveis  `create` `delete` incluem , e `patch` `other` .</span><span class="sxs-lookup"><span data-stu-id="f4711-154">Possible values include `create`, `delete`, `patch` and `other`.</span></span> <span data-ttu-id="f4711-155">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-155">Read-only.</span></span>|
|<span data-ttu-id="f4711-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="f4711-156">activityResult</span></span>|[<span data-ttu-id="f4711-157">cloudPcAuditActivityResult</span><span class="sxs-lookup"><span data-stu-id="f4711-157">cloudPcAuditActivityResult</span></span>](#cloudpcauditactivityresult-values)|<span data-ttu-id="f4711-158">O resultado da atividade.</span><span class="sxs-lookup"><span data-stu-id="f4711-158">The result of the activity.</span></span><span data-ttu-id="f4711-159">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-159"> Read-only.</span></span>|
|<span data-ttu-id="f4711-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="f4711-160">correlationId</span></span>|<span data-ttu-id="f4711-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4711-161">String</span></span>|<span data-ttu-id="f4711-162">O identificador de solicitação do cliente, usado para correlacionar a atividade no sistema.</span><span class="sxs-lookup"><span data-stu-id="f4711-162">The client request identifier, used to correlate activity within the system.</span></span><span data-ttu-id="f4711-163">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-163"> Read-only.</span></span>|
|<span data-ttu-id="f4711-164">recursos</span><span class="sxs-lookup"><span data-stu-id="f4711-164">resources</span></span>|<span data-ttu-id="f4711-165">[Coleção cloudPcAuditResource](../resources/cloudpcauditresource.md)</span><span class="sxs-lookup"><span data-stu-id="f4711-165">[cloudPcAuditResource](../resources/cloudpcauditresource.md) collection</span></span>|<span data-ttu-id="f4711-166">Lista de objetos cloudPcAuditResource.</span><span class="sxs-lookup"><span data-stu-id="f4711-166">List of cloudPcAuditResource objects.</span></span><span data-ttu-id="f4711-167">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-167"> Read-only.</span></span>|
|<span data-ttu-id="f4711-168">category</span><span class="sxs-lookup"><span data-stu-id="f4711-168">category</span></span>|[<span data-ttu-id="f4711-169">cloudPcAuditCategory</span><span class="sxs-lookup"><span data-stu-id="f4711-169">cloudPcAuditCategory</span></span>](#cloudpcauditcategory-values)|<span data-ttu-id="f4711-170">Categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f4711-170">Audit category.</span></span> <span data-ttu-id="f4711-171">Só leitura.</span><span class="sxs-lookup"><span data-stu-id="f4711-171">Read-only.</span></span>|

### <a name="cloudpcauditactivityoperationtype-values"></a><span data-ttu-id="f4711-172">valores cloudPcAuditActivityOperationType</span><span class="sxs-lookup"><span data-stu-id="f4711-172">cloudPcAuditActivityOperationType values</span></span>

|<span data-ttu-id="f4711-173">Member</span><span class="sxs-lookup"><span data-stu-id="f4711-173">Member</span></span>|<span data-ttu-id="f4711-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4711-174">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4711-175">create</span><span class="sxs-lookup"><span data-stu-id="f4711-175">create</span></span>|<span data-ttu-id="f4711-176">Criar operação.</span><span class="sxs-lookup"><span data-stu-id="f4711-176">Create operation.</span></span>|
|<span data-ttu-id="f4711-177">delete</span><span class="sxs-lookup"><span data-stu-id="f4711-177">delete</span></span>|<span data-ttu-id="f4711-178">Excluir operação.</span><span class="sxs-lookup"><span data-stu-id="f4711-178">Delete operation.</span></span>|
|<span data-ttu-id="f4711-179">patch</span><span class="sxs-lookup"><span data-stu-id="f4711-179">patch</span></span>|<span data-ttu-id="f4711-180">Operação patch.</span><span class="sxs-lookup"><span data-stu-id="f4711-180">Patch operation.</span></span>|
|<span data-ttu-id="f4711-181">other</span><span class="sxs-lookup"><span data-stu-id="f4711-181">other</span></span>|<span data-ttu-id="f4711-182">Outra operação.</span><span class="sxs-lookup"><span data-stu-id="f4711-182">Other operation.</span></span>|

### <a name="cloudpcauditactivityresult-values"></a><span data-ttu-id="f4711-183">valores cloudPcAuditActivityResult</span><span class="sxs-lookup"><span data-stu-id="f4711-183">cloudPcAuditActivityResult values</span></span>

|<span data-ttu-id="f4711-184">Member</span><span class="sxs-lookup"><span data-stu-id="f4711-184">Member</span></span>|<span data-ttu-id="f4711-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4711-185">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4711-186">sucesso</span><span class="sxs-lookup"><span data-stu-id="f4711-186">success</span></span>|<span data-ttu-id="f4711-187">Operação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f4711-187">Operation succeeded.</span></span>|
|<span data-ttu-id="f4711-188">clientError</span><span class="sxs-lookup"><span data-stu-id="f4711-188">clientError</span></span>|<span data-ttu-id="f4711-189">A operação falhou com o erro do cliente.</span><span class="sxs-lookup"><span data-stu-id="f4711-189">Operation failed with client error.</span></span>|
|<span data-ttu-id="f4711-190">failure</span><span class="sxs-lookup"><span data-stu-id="f4711-190">failure</span></span>|<span data-ttu-id="f4711-191">Falha na operação.</span><span class="sxs-lookup"><span data-stu-id="f4711-191">Operation failed.</span></span>|
|<span data-ttu-id="f4711-192">timeExceeded</span><span class="sxs-lookup"><span data-stu-id="f4711-192">timeExceeded</span></span>|<span data-ttu-id="f4711-193">A operação falhou com o tempo de tempo.</span><span class="sxs-lookup"><span data-stu-id="f4711-193">Operation failed with timeout.</span></span>|
|<span data-ttu-id="f4711-194">other</span><span class="sxs-lookup"><span data-stu-id="f4711-194">other</span></span>|<span data-ttu-id="f4711-195">Outro resultado.</span><span class="sxs-lookup"><span data-stu-id="f4711-195">Other result.</span></span>|

### <a name="cloudpcauditcategory-values"></a><span data-ttu-id="f4711-196">valores cloudPcAuditCategory</span><span class="sxs-lookup"><span data-stu-id="f4711-196">cloudPcAuditCategory values</span></span>

|<span data-ttu-id="f4711-197">Member</span><span class="sxs-lookup"><span data-stu-id="f4711-197">Member</span></span>|<span data-ttu-id="f4711-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4711-198">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4711-199">cloudPC</span><span class="sxs-lookup"><span data-stu-id="f4711-199">cloudPC</span></span>|<span data-ttu-id="f4711-200">Categoria de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="f4711-200">Cloud PC category.</span></span>|
|<span data-ttu-id="f4711-201">other</span><span class="sxs-lookup"><span data-stu-id="f4711-201">other</span></span> |<span data-ttu-id="f4711-202">Outra categoria.</span><span class="sxs-lookup"><span data-stu-id="f4711-202">Other category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4711-203">Relações</span><span class="sxs-lookup"><span data-stu-id="f4711-203">Relationships</span></span>

<span data-ttu-id="f4711-204">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4711-204">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4711-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4711-205">JSON representation</span></span>

<span data-ttu-id="f4711-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4711-206">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.cloudPcAuditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```
