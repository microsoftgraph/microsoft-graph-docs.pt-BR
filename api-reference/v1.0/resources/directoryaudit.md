---
title: Tipo de recurso directoryObject
description: Representa os itens de auditoria de diretório e sua coleção.
author: SarahBar
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86d2482c974c839597ebb8bc6a5b298f854d07b6
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845306"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="95b55-103">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="95b55-103">directoryAudit resource type</span></span>

<span data-ttu-id="95b55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95b55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95b55-105">Representa os itens de auditoria de diretório e sua coleção.</span><span class="sxs-lookup"><span data-stu-id="95b55-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="95b55-106">Methods</span><span class="sxs-lookup"><span data-stu-id="95b55-106">Methods</span></span>

| <span data-ttu-id="95b55-107">Método</span><span class="sxs-lookup"><span data-stu-id="95b55-107">Method</span></span>           | <span data-ttu-id="95b55-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95b55-108">Return Type</span></span>    |<span data-ttu-id="95b55-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b55-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95b55-110">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="95b55-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="95b55-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="95b55-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="95b55-112">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="95b55-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="95b55-113">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="95b55-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="95b55-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="95b55-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="95b55-115">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="95b55-115">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="95b55-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95b55-116">Properties</span></span>

| <span data-ttu-id="95b55-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95b55-117">Property</span></span>            | <span data-ttu-id="95b55-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="95b55-118">Type</span></span>                                                | <span data-ttu-id="95b55-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b55-119">Description</span></span>                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="95b55-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="95b55-120">activityDateTime</span></span>    | <span data-ttu-id="95b55-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b55-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="95b55-122">Indica a data e hora que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="95b55-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="95b55-123">O tipo de Timestamp é sempre UTC.</span><span class="sxs-lookup"><span data-stu-id="95b55-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="95b55-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="95b55-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>                                                                                          |
| <span data-ttu-id="95b55-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="95b55-125">activityDisplayName</span></span> | <span data-ttu-id="95b55-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b55-126">String</span></span>                                              | <span data-ttu-id="95b55-127">Indica o nome da atividade ou o nome da operação (exemplos: "criar usuário" e "Adicionar membro ao grupo").</span><span class="sxs-lookup"><span data-stu-id="95b55-127">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="95b55-128">Para obter uma lista completa, confira [lista de atividades do Azure ad](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="95b55-128">For full list, see [Azure AD activity list](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="95b55-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="95b55-129">additionalDetails</span></span>   | <span data-ttu-id="95b55-130">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="95b55-130">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="95b55-131">Indica detalhes adicionais sobre a atividade.</span><span class="sxs-lookup"><span data-stu-id="95b55-131">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                                      |
| <span data-ttu-id="95b55-132">category</span><span class="sxs-lookup"><span data-stu-id="95b55-132">category</span></span>            | <span data-ttu-id="95b55-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b55-133">String</span></span>                                              | <span data-ttu-id="95b55-134">Indica qual categoria de recurso direcionada pela atividade.</span><span class="sxs-lookup"><span data-stu-id="95b55-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="95b55-135">(Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)</span><span class="sxs-lookup"><span data-stu-id="95b55-135">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                                          |
| <span data-ttu-id="95b55-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="95b55-136">correlationId</span></span>       | <span data-ttu-id="95b55-137">GUID</span><span class="sxs-lookup"><span data-stu-id="95b55-137">GUID</span></span>                                                | <span data-ttu-id="95b55-138">Indica uma ID exclusiva que ajuda correlacionar atividades que englobam vários serviços.</span><span class="sxs-lookup"><span data-stu-id="95b55-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="95b55-139">Pode ser usado para os logs de serviços de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="95b55-139">Can be used to trace logs across services.</span></span>                                                                                                                                                |
| <span data-ttu-id="95b55-140">id</span><span class="sxs-lookup"><span data-stu-id="95b55-140">id</span></span>                  | <span data-ttu-id="95b55-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b55-141">String</span></span>                                              | <span data-ttu-id="95b55-142">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="95b55-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="95b55-143">Este é um GUID.</span><span class="sxs-lookup"><span data-stu-id="95b55-143">This is a GUID.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="95b55-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="95b55-144">initiatedBy</span></span>         | [<span data-ttu-id="95b55-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="95b55-145">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="95b55-146">Indica que informações sobre o usuário ou o aplicativo iniciou a atividade.</span><span class="sxs-lookup"><span data-stu-id="95b55-146">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                                |
| <span data-ttu-id="95b55-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="95b55-147">loggedByService</span></span>     | <span data-ttu-id="95b55-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b55-148">String</span></span>                                              | <span data-ttu-id="95b55-149">Indica informação em que o serviço iniciou a atividade (por exemplo: gerenciamento de senha de autoatendimento, principais diretório, B2C, os usuários convidados, Microsoft Identity Manager, Privileged Identity Management.</span><span class="sxs-lookup"><span data-stu-id="95b55-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                                      |
| <span data-ttu-id="95b55-150">resultado</span><span class="sxs-lookup"><span data-stu-id="95b55-150">result</span></span>              | <span data-ttu-id="95b55-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b55-151">string</span></span>                                              | <span data-ttu-id="95b55-152">Indica o resultado da atividade. Valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="95b55-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                                   |
| <span data-ttu-id="95b55-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="95b55-153">resultReason</span></span>        | <span data-ttu-id="95b55-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b55-154">String</span></span>                                              | <span data-ttu-id="95b55-155">Descreve a causa dos resultados de "falha" ou "tempo limite".</span><span class="sxs-lookup"><span data-stu-id="95b55-155">Describes cause of "failure" or "timeout" results.</span></span>                                                                                                                                                                                                                                 |
| <span data-ttu-id="95b55-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="95b55-156">targetResources</span></span>     | <span data-ttu-id="95b55-157">[targetResource](targetresource.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="95b55-157">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="95b55-158">Indica informação que o recurso foi alterado devido a atividade.</span><span class="sxs-lookup"><span data-stu-id="95b55-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="95b55-159">Tipo de recurso de destino pode ser usuário, dispositivo, diretório, aplicativos, função, grupo, política ou outros.</span><span class="sxs-lookup"><span data-stu-id="95b55-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>                                                                                                                   |

## <a name="relationships"></a><span data-ttu-id="95b55-160">Relações</span><span class="sxs-lookup"><span data-stu-id="95b55-160">Relationships</span></span>

<span data-ttu-id="95b55-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95b55-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95b55-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95b55-162">JSON representation</span></span>

<span data-ttu-id="95b55-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95b55-163">Here is a JSON representation of the resource.</span></span>

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
