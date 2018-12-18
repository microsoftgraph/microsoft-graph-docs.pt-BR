---
title: tipo de recurso de directoryAudit
description: Esse recurso representa os itens de auditoria de diretório e sua coleção
author: lleonard-msft
ms.openlocfilehash: 5cbfc1320f721afd71ed3f196bb94a5c716d2c5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312786"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="e6dc8-103">tipo de recurso de directoryAudit</span><span class="sxs-lookup"><span data-stu-id="e6dc8-103">directoryAudit resource type</span></span>
<span data-ttu-id="e6dc8-104">Esse recurso representa os itens de auditoria de diretório e sua coleção</span><span class="sxs-lookup"><span data-stu-id="e6dc8-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="e6dc8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6dc8-105">Methods</span></span>

| <span data-ttu-id="e6dc8-106">Método</span><span class="sxs-lookup"><span data-stu-id="e6dc8-106">Method</span></span>           | <span data-ttu-id="e6dc8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6dc8-107">Return Type</span></span>    |<span data-ttu-id="e6dc8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dc8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6dc8-109">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="e6dc8-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="e6dc8-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="e6dc8-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="e6dc8-111">Listam os itens de auditoria de diretório na coleção e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="e6dc8-112">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="e6dc8-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="e6dc8-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="e6dc8-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="e6dc8-114">Obtenha um item de auditoria de diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="e6dc8-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6dc8-115">Properties</span></span>
| <span data-ttu-id="e6dc8-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6dc8-116">Property</span></span>     | <span data-ttu-id="e6dc8-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6dc8-117">Type</span></span>   |<span data-ttu-id="e6dc8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dc8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6dc8-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="e6dc8-119">activityDateTime</span></span>|<span data-ttu-id="e6dc8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6dc8-120">DateTimeOffset</span></span>|<span data-ttu-id="e6dc8-121">Indica a data e hora que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="e6dc8-122">O tipo de carimbo de hora é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="e6dc8-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e6dc8-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e6dc8-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6dc8-124">activityDisplayName</span></span>|<span data-ttu-id="e6dc8-125">String</span><span class="sxs-lookup"><span data-stu-id="e6dc8-125">String</span></span>|<span data-ttu-id="e6dc8-126">Indica o nome da atividade ou o nome da operação (ex.:</span><span class="sxs-lookup"><span data-stu-id="e6dc8-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="e6dc8-127">"Criar usuário", "Adicionar membro ao grupo").</span><span class="sxs-lookup"><span data-stu-id="e6dc8-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="e6dc8-128">Para obter uma lista de atividades conectado, consulte [lista de atividades do Windows Azure Ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="e6dc8-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="e6dc8-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="e6dc8-129">additionalDetails</span></span>|<span data-ttu-id="e6dc8-130">coleção [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc8-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="e6dc8-131">Indica detalhes adicionais sobre a atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="e6dc8-132">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="e6dc8-132">category</span></span>|<span data-ttu-id="e6dc8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dc8-133">String</span></span>|<span data-ttu-id="e6dc8-134">Indica qual categoria de recurso que está programada pela atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="e6dc8-135">(Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)</span><span class="sxs-lookup"><span data-stu-id="e6dc8-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="e6dc8-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="e6dc8-136">correlationId</span></span>|<span data-ttu-id="e6dc8-137">GUID</span><span class="sxs-lookup"><span data-stu-id="e6dc8-137">GUID</span></span>|<span data-ttu-id="e6dc8-138">Indica uma identificação exclusiva que ajuda a correlacionar atividades que se estendem por vários serviços.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="e6dc8-139">Podem ser usadas para logs de rastreamento em serviços.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="e6dc8-140">id</span><span class="sxs-lookup"><span data-stu-id="e6dc8-140">id</span></span>|<span data-ttu-id="e6dc8-141">String</span><span class="sxs-lookup"><span data-stu-id="e6dc8-141">String</span></span>| <span data-ttu-id="e6dc8-142">Indica a ID exclusiva da atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="e6dc8-143">Este é um GUID.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-143">This is a GUID.</span></span>|
|<span data-ttu-id="e6dc8-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="e6dc8-144">initiatedBy</span></span>|[<span data-ttu-id="e6dc8-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="e6dc8-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="e6dc8-146">Indica informações sobre o usuário ou aplicativo iniciado a atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="e6dc8-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="e6dc8-147">loggedByService</span></span>|<span data-ttu-id="e6dc8-148">String</span><span class="sxs-lookup"><span data-stu-id="e6dc8-148">String</span></span>|<span data-ttu-id="e6dc8-149">Indica informações no qual o serviço iniciou a atividade (por exemplo: gerenciamento de senha pessoal, Core diretório, B2C, usuários convidados, Microsoft Identity Manager, privilegiado gerenciamento de identidade.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="e6dc8-150">result</span><span class="sxs-lookup"><span data-stu-id="e6dc8-150">result</span></span>|<span data-ttu-id="e6dc8-151">string</span><span class="sxs-lookup"><span data-stu-id="e6dc8-151">string</span></span>| <span data-ttu-id="e6dc8-152">Indica o resultado da atividade. Os valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="e6dc8-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="e6dc8-153">resultReason</span></span>|<span data-ttu-id="e6dc8-154">String</span><span class="sxs-lookup"><span data-stu-id="e6dc8-154">String</span></span>|<span data-ttu-id="e6dc8-155">Indica o motivo da falha se o resultado é "Falha" ou "timeout".</span><span class="sxs-lookup"><span data-stu-id="e6dc8-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="e6dc8-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="e6dc8-156">targetResources</span></span>|<span data-ttu-id="e6dc8-157">coleção [targetResource](targetresource.md)</span><span class="sxs-lookup"><span data-stu-id="e6dc8-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="e6dc8-158">Indica informações no qual o recurso foi alterado devido a atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="e6dc8-159">Tipo de recurso de destino pode ser um usuário, dispositivo, diretório, App, função, grupo, política ou outros.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="e6dc8-160">Relações</span><span class="sxs-lookup"><span data-stu-id="e6dc8-160">Relationships</span></span>
<span data-ttu-id="e6dc8-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6dc8-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6dc8-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6dc8-162">JSON representation</span></span>

<span data-ttu-id="e6dc8-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6dc8-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->