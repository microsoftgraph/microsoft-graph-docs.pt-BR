---
title: Tipo de recurso directoryObject
description: Representa os itens de auditoria de diretório e sua coleção.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54badc0fb411a79ac854c2a34f708cd7d29133a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029481"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="9452b-103">Tipo de recurso directoryObject</span><span class="sxs-lookup"><span data-stu-id="9452b-103">directoryAudit resource type</span></span>

<span data-ttu-id="9452b-104">Representa os itens de auditoria de diretório e sua coleção.</span><span class="sxs-lookup"><span data-stu-id="9452b-104">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="9452b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9452b-105">Methods</span></span>

| <span data-ttu-id="9452b-106">Método</span><span class="sxs-lookup"><span data-stu-id="9452b-106">Method</span></span>           | <span data-ttu-id="9452b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9452b-107">Return Type</span></span>    |<span data-ttu-id="9452b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9452b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9452b-109">Lista directoryAudits</span><span class="sxs-lookup"><span data-stu-id="9452b-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="9452b-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9452b-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="9452b-111">Liste os itens de auditoria de diretório no conjunto de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9452b-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="9452b-112">Obter directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9452b-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="9452b-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9452b-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="9452b-114">Obter um item de auditoria do diretório específico e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9452b-114">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="9452b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9452b-115">Properties</span></span>

| <span data-ttu-id="9452b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9452b-116">Property</span></span>     | <span data-ttu-id="9452b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="9452b-117">Type</span></span>   |<span data-ttu-id="9452b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="9452b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9452b-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="9452b-119">activityDateTime</span></span>|<span data-ttu-id="9452b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9452b-120">DateTimeOffset</span></span>|<span data-ttu-id="9452b-121">Indica a data e hora que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="9452b-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="9452b-122">O tipo de Timestamp é sempre UTC.</span><span class="sxs-lookup"><span data-stu-id="9452b-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="9452b-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9452b-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9452b-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="9452b-124">activityDisplayName</span></span>|<span data-ttu-id="9452b-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9452b-125">String</span></span>|<span data-ttu-id="9452b-126">Indica o nome da atividade ou o nome da operação (exemplos: "criar usuário" e "Adicionar membro ao grupo").</span><span class="sxs-lookup"><span data-stu-id="9452b-126">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="9452b-127">Para obter uma lista completa, confira [lista de atividades do Azure ad](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="9452b-127">For full list, see [Azure AD activity list](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="9452b-128">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="9452b-128">additionalDetails</span></span>|<span data-ttu-id="9452b-129">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9452b-129">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="9452b-130">Indica detalhes adicionais sobre a atividade.</span><span class="sxs-lookup"><span data-stu-id="9452b-130">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="9452b-131">category</span><span class="sxs-lookup"><span data-stu-id="9452b-131">category</span></span>|<span data-ttu-id="9452b-132">String</span><span class="sxs-lookup"><span data-stu-id="9452b-132">String</span></span>|<span data-ttu-id="9452b-133">Indica qual categoria de recurso direcionada pela atividade.</span><span class="sxs-lookup"><span data-stu-id="9452b-133">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="9452b-134">(Por exemplo: gerenciamento de usuário, grupo gerenciamento etc..)</span><span class="sxs-lookup"><span data-stu-id="9452b-134">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="9452b-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="9452b-135">correlationId</span></span>|<span data-ttu-id="9452b-136">GUID</span><span class="sxs-lookup"><span data-stu-id="9452b-136">GUID</span></span>|<span data-ttu-id="9452b-137">Indica uma ID exclusiva que ajuda correlacionar atividades que englobam vários serviços.</span><span class="sxs-lookup"><span data-stu-id="9452b-137">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="9452b-138">Pode ser usado para os logs de serviços de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="9452b-138">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="9452b-139">id</span><span class="sxs-lookup"><span data-stu-id="9452b-139">id</span></span>|<span data-ttu-id="9452b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9452b-140">String</span></span>| <span data-ttu-id="9452b-141">Indica que a ID exclusiva para a atividade.</span><span class="sxs-lookup"><span data-stu-id="9452b-141">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="9452b-142">Este é um GUID.</span><span class="sxs-lookup"><span data-stu-id="9452b-142">This is a GUID.</span></span>|
|<span data-ttu-id="9452b-143">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="9452b-143">initiatedBy</span></span>|[<span data-ttu-id="9452b-144">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="9452b-144">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="9452b-145">Indica que informações sobre o usuário ou o aplicativo iniciou a atividade.</span><span class="sxs-lookup"><span data-stu-id="9452b-145">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="9452b-146">loggedByService</span><span class="sxs-lookup"><span data-stu-id="9452b-146">loggedByService</span></span>|<span data-ttu-id="9452b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9452b-147">String</span></span>|<span data-ttu-id="9452b-148">Indica informação em que o serviço iniciou a atividade (por exemplo: gerenciamento de senha de autoatendimento, principais diretório, B2C, os usuários convidados, Microsoft Identity Manager, Privileged Identity Management.</span><span class="sxs-lookup"><span data-stu-id="9452b-148">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="9452b-149">resultado</span><span class="sxs-lookup"><span data-stu-id="9452b-149">result</span></span>|<span data-ttu-id="9452b-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9452b-150">string</span></span>| <span data-ttu-id="9452b-151">Indica o resultado da atividade. Valores possíveis são: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9452b-151">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="9452b-152">resultReason</span><span class="sxs-lookup"><span data-stu-id="9452b-152">resultReason</span></span>|<span data-ttu-id="9452b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9452b-153">String</span></span>|<span data-ttu-id="9452b-154">Descreve a causa dos resultados de "falha" ou "tempo limite".</span><span class="sxs-lookup"><span data-stu-id="9452b-154">Describes cause of "failure" or "timeout" results.</span></span>|
|<span data-ttu-id="9452b-155">targetResources</span><span class="sxs-lookup"><span data-stu-id="9452b-155">targetResources</span></span>|<span data-ttu-id="9452b-156">[targetResource](targetresource.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="9452b-156">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="9452b-157">Indica informação que o recurso foi alterado devido a atividade.</span><span class="sxs-lookup"><span data-stu-id="9452b-157">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="9452b-158">Tipo de recurso de destino pode ser usuário, dispositivo, diretório, aplicativos, função, grupo, política ou outros.</span><span class="sxs-lookup"><span data-stu-id="9452b-158">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="9452b-159">Relações</span><span class="sxs-lookup"><span data-stu-id="9452b-159">Relationships</span></span>

<span data-ttu-id="9452b-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9452b-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9452b-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9452b-161">JSON representation</span></span>

<span data-ttu-id="9452b-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9452b-162">Here is a JSON representation of the resource.</span></span>

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
