---
title: Tipo de recurso directoryObject
description: Esse recurso representa seu conjunto e os itens de auditoria do diretório
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f980208788731206dc58870635644a1f3edc4c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543223"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="1d228-103">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="1d228-103">directoryAudit resource type</span></span>
<span data-ttu-id="1d228-104">Esse recurso representa seu conjunto e os itens de auditoria do diretório</span><span class="sxs-lookup"><span data-stu-id="1d228-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="1d228-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d228-105">Methods</span></span>

| <span data-ttu-id="1d228-106">Método</span><span class="sxs-lookup"><span data-stu-id="1d228-106">Method</span></span>           | <span data-ttu-id="1d228-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d228-107">Return Type</span></span>    |<span data-ttu-id="1d228-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d228-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d228-109">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="1d228-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="1d228-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="1d228-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="1d228-111">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1d228-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="1d228-112">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="1d228-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="1d228-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="1d228-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="1d228-114">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1d228-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="1d228-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d228-115">Properties</span></span>
| <span data-ttu-id="1d228-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d228-116">Property</span></span>     | <span data-ttu-id="1d228-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d228-117">Type</span></span>   |<span data-ttu-id="1d228-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d228-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d228-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="1d228-119">activityDateTime</span></span>|<span data-ttu-id="1d228-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d228-120">DateTimeOffset</span></span>|<span data-ttu-id="1d228-121">Indica a data e hora que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="1d228-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="1d228-122">O tipo de Timestamp é sempre UTC.</span><span class="sxs-lookup"><span data-stu-id="1d228-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="1d228-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1d228-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1d228-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="1d228-124">activityDisplayName</span></span>|<span data-ttu-id="1d228-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d228-125">String</span></span>|<span data-ttu-id="1d228-126">Indica o nome da atividade ou o nome da operação (ex.:</span><span class="sxs-lookup"><span data-stu-id="1d228-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="1d228-127">"Criar usuário", "Adicionar membro ao grupo").</span><span class="sxs-lookup"><span data-stu-id="1d228-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="1d228-128">Para obter uma lista de atividades registradas, veja [lista de atividades do Azure Ad](https://docs.microsoft.com/pt-BR/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="1d228-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/pt-BR/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="1d228-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="1d228-129">additionalDetails</span></span>|<span data-ttu-id="1d228-130">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1d228-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="1d228-131">Indica detalhes adicionais sobre a atividade.</span><span class="sxs-lookup"><span data-stu-id="1d228-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="1d228-132">category</span><span class="sxs-lookup"><span data-stu-id="1d228-132">category</span></span>|<span data-ttu-id="1d228-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d228-133">String</span></span>|<span data-ttu-id="1d228-134">Indica qual categoria de recurso direcionada pela atividade.</span><span class="sxs-lookup"><span data-stu-id="1d228-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="1d228-135">(Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)</span><span class="sxs-lookup"><span data-stu-id="1d228-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="1d228-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="1d228-136">correlationId</span></span>|<span data-ttu-id="1d228-137">GUID</span><span class="sxs-lookup"><span data-stu-id="1d228-137">GUID</span></span>|<span data-ttu-id="1d228-138">Indica uma ID exclusiva que ajuda correlacionar atividades que englobam vários serviços.</span><span class="sxs-lookup"><span data-stu-id="1d228-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="1d228-139">Pode ser usado para os logs de serviços de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="1d228-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="1d228-140">id</span><span class="sxs-lookup"><span data-stu-id="1d228-140">id</span></span>|<span data-ttu-id="1d228-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d228-141">String</span></span>| <span data-ttu-id="1d228-142">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="1d228-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="1d228-143">Este é um GUID.</span><span class="sxs-lookup"><span data-stu-id="1d228-143">This is a GUID.</span></span>|
|<span data-ttu-id="1d228-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="1d228-144">initiatedBy</span></span>|[<span data-ttu-id="1d228-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="1d228-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="1d228-146">Indica que informações sobre o usuário ou o aplicativo iniciou a atividade.</span><span class="sxs-lookup"><span data-stu-id="1d228-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="1d228-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="1d228-147">loggedByService</span></span>|<span data-ttu-id="1d228-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d228-148">String</span></span>|<span data-ttu-id="1d228-149">Indica informação em que o serviço iniciou a atividade (por exemplo: gerenciamento de senha de autoatendimento, principais diretório, B2C, os usuários convidados, Microsoft Identity Manager, Privileged Identity Management.</span><span class="sxs-lookup"><span data-stu-id="1d228-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="1d228-150">resultado</span><span class="sxs-lookup"><span data-stu-id="1d228-150">result</span></span>|<span data-ttu-id="1d228-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d228-151">string</span></span>| <span data-ttu-id="1d228-152">Indica o resultado da atividade. Valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1d228-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="1d228-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="1d228-153">resultReason</span></span>|<span data-ttu-id="1d228-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d228-154">String</span></span>|<span data-ttu-id="1d228-155">Indica o motivo da falha se o resultado é "tempo esgotado" ou "Falha".</span><span class="sxs-lookup"><span data-stu-id="1d228-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="1d228-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="1d228-156">targetResources</span></span>|<span data-ttu-id="1d228-157">[targetResource](targetresource.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="1d228-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="1d228-158">Indica informação que o recurso foi alterado devido a atividade.</span><span class="sxs-lookup"><span data-stu-id="1d228-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="1d228-159">Tipo de recurso de destino pode ser usuário, dispositivo, diretório, aplicativos, função, grupo, política ou outros.</span><span class="sxs-lookup"><span data-stu-id="1d228-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="1d228-160">Relações</span><span class="sxs-lookup"><span data-stu-id="1d228-160">Relationships</span></span>
<span data-ttu-id="1d228-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d228-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1d228-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d228-162">JSON representation</span></span>

<span data-ttu-id="1d228-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d228-163">Here is a JSON representation of the resource.</span></span>

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
