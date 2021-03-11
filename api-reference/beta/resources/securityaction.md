---
title: Tipo de recurso securityAction
description: Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o ATP do Windows Defender (em breve) para bloquear as atividades mal-intencionados seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c1adeb6ee5ab3b3ad2165e854b2812e39b8df5ab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720624"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="5708a-106">Tipo de recurso securityAction</span><span class="sxs-lookup"><span data-stu-id="5708a-106">securityAction resource type</span></span>

<span data-ttu-id="5708a-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5708a-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5708a-108">Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5708a-108">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="5708a-109">Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5708a-109">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="5708a-110">Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário.</span><span class="sxs-lookup"><span data-stu-id="5708a-110">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="5708a-111">Experimente as ações de segurança com o [ATP do Windows Defender](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)para bloquear as atividades mal-intencionados em seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.</span><span class="sxs-lookup"><span data-stu-id="5708a-111">Try security actions with [Windows Defender ATP](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="5708a-112">**Observação:** ações de segurança no momento apenas dá suporte a permissões do aplicativo compatível.</span><span class="sxs-lookup"><span data-stu-id="5708a-112">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="5708a-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="5708a-113">Methods</span></span>

| <span data-ttu-id="5708a-114">Método</span><span class="sxs-lookup"><span data-stu-id="5708a-114">Method</span></span>       | <span data-ttu-id="5708a-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5708a-115">Return Type</span></span> | <span data-ttu-id="5708a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5708a-116">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5708a-117">Obter a ação de segurança</span><span class="sxs-lookup"><span data-stu-id="5708a-117">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="5708a-118">securityAction</span><span class="sxs-lookup"><span data-stu-id="5708a-118">securityAction</span></span>](securityaction.md) | <span data-ttu-id="5708a-119">Ler propriedades e relações do objeto securityAction.</span><span class="sxs-lookup"><span data-stu-id="5708a-119">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="5708a-120">Criar ação de segurança</span><span class="sxs-lookup"><span data-stu-id="5708a-120">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="5708a-121">securityAction</span><span class="sxs-lookup"><span data-stu-id="5708a-121">securityAction</span></span>](securityaction.md) | <span data-ttu-id="5708a-122">Crie uma nova securityAction postando na coleção securityActions.</span><span class="sxs-lookup"><span data-stu-id="5708a-122">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="5708a-123">Listar ações de segurança</span><span class="sxs-lookup"><span data-stu-id="5708a-123">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="5708a-124">[Coleção securityAction](securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="5708a-124">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="5708a-125">Obter uma coleção de objetos securityAction.</span><span class="sxs-lookup"><span data-stu-id="5708a-125">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="5708a-126">Cancelar ação de segurança</span><span class="sxs-lookup"><span data-stu-id="5708a-126">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="5708a-127">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="5708a-127">None</span></span>|<span data-ttu-id="5708a-128">Cancele uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="5708a-128">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="5708a-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5708a-129">Properties</span></span>

| <span data-ttu-id="5708a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5708a-130">Property</span></span>     | <span data-ttu-id="5708a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5708a-131">Type</span></span>        | <span data-ttu-id="5708a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5708a-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5708a-133">actionReason</span><span class="sxs-lookup"><span data-stu-id="5708a-133">actionReason</span></span>|<span data-ttu-id="5708a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5708a-134">String</span></span>|<span data-ttu-id="5708a-135">Motivo para invocar essa ação.</span><span class="sxs-lookup"><span data-stu-id="5708a-135">Reason for invoking this action.</span></span>|
|<span data-ttu-id="5708a-136">appId</span><span class="sxs-lookup"><span data-stu-id="5708a-136">appId</span></span>|<span data-ttu-id="5708a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5708a-137">String</span></span>|<span data-ttu-id="5708a-138">A ID do Aplicativo do aplicativo de chamada que enviou (POST) a ação.</span><span class="sxs-lookup"><span data-stu-id="5708a-138">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="5708a-139">O appId deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="5708a-139">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="5708a-140">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="5708a-140">azureTenantId</span></span>|<span data-ttu-id="5708a-141">String</span><span class="sxs-lookup"><span data-stu-id="5708a-141">String</span></span>|<span data-ttu-id="5708a-142">ID do locatário do Azure da entidade para determinar a qual locatário a entidade pertence (suporte a vários locatários).</span><span class="sxs-lookup"><span data-stu-id="5708a-142">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="5708a-143">O azureTenantId deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="5708a-143">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="5708a-144">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="5708a-144">completedDateTime</span></span>|<span data-ttu-id="5708a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5708a-145">DateTimeOffset</span></span>|<span data-ttu-id="5708a-146">Timestamp quando a ação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="5708a-146">Timestamp when the action was completed.</span></span> <span data-ttu-id="5708a-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5708a-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5708a-148">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5708a-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5708a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5708a-149">createdDateTime</span></span>|<span data-ttu-id="5708a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5708a-150">DateTimeOffset</span></span>|<span data-ttu-id="5708a-151">Timestamp quando a ação é criada.</span><span class="sxs-lookup"><span data-stu-id="5708a-151">Timestamp when the action is created.</span></span> <span data-ttu-id="5708a-152">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5708a-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5708a-153">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5708a-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5708a-154">errorInfo</span><span class="sxs-lookup"><span data-stu-id="5708a-154">errorInfo</span></span>|[<span data-ttu-id="5708a-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5708a-155">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="5708a-156">Informações de erro quando a ação falhar.</span><span class="sxs-lookup"><span data-stu-id="5708a-156">Error info when the action fails.</span></span>|
|<span data-ttu-id="5708a-157">id</span><span class="sxs-lookup"><span data-stu-id="5708a-157">id</span></span>|<span data-ttu-id="5708a-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5708a-158">String</span></span>| <span data-ttu-id="5708a-159">Criado pelo sistema quando a ação é ingerida.</span><span class="sxs-lookup"><span data-stu-id="5708a-159">Created by the system when the action is ingested.</span></span> <span data-ttu-id="5708a-160">GUID gerado/identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="5708a-160">Generated GUID/unique identifier.</span></span> <span data-ttu-id="5708a-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5708a-161">Read-only.</span></span>|
|<span data-ttu-id="5708a-162">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="5708a-162">lastActionDateTime</span></span>|<span data-ttu-id="5708a-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5708a-163">DateTimeOffset</span></span>| <span data-ttu-id="5708a-164">Timestamp quando essa ação foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5708a-164">Timestamp when this action was last updated.</span></span> <span data-ttu-id="5708a-165">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5708a-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5708a-166">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5708a-166">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5708a-167">nome</span><span class="sxs-lookup"><span data-stu-id="5708a-167">name</span></span>|<span data-ttu-id="5708a-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5708a-168">String</span></span>| <span data-ttu-id="5708a-169">Nome da ação.</span><span class="sxs-lookup"><span data-stu-id="5708a-169">Action name.</span></span>|
|<span data-ttu-id="5708a-170">parameters</span><span class="sxs-lookup"><span data-stu-id="5708a-170">parameters</span></span>|<span data-ttu-id="5708a-171">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5708a-171">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="5708a-172">Coleção de parâmetros (pares de valores-chave) necessários para invocar a ação, por exemplo, URL ou fileHash para bloquear, etc.).</span><span class="sxs-lookup"><span data-stu-id="5708a-172">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="5708a-173">**Required**</span><span class="sxs-lookup"><span data-stu-id="5708a-173">**Required**</span></span>|
|<span data-ttu-id="5708a-174">states</span><span class="sxs-lookup"><span data-stu-id="5708a-174">states</span></span>|<span data-ttu-id="5708a-175">[Coleção securityActionState](securityactionstate.md)</span><span class="sxs-lookup"><span data-stu-id="5708a-175">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="5708a-176">Coleção de securityActionState para manter o histórico de uma ação.</span><span class="sxs-lookup"><span data-stu-id="5708a-176">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="5708a-177">status</span><span class="sxs-lookup"><span data-stu-id="5708a-177">status</span></span>|<span data-ttu-id="5708a-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5708a-178">string</span></span>| <span data-ttu-id="5708a-179">Status da ação.</span><span class="sxs-lookup"><span data-stu-id="5708a-179">Status of the action.</span></span> <span data-ttu-id="5708a-180">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="5708a-180">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="5708a-181">user</span><span class="sxs-lookup"><span data-stu-id="5708a-181">user</span></span>|<span data-ttu-id="5708a-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5708a-182">String</span></span>| <span data-ttu-id="5708a-183">O nome principal do usuário do usuário que enviou (POST) a ação.</span><span class="sxs-lookup"><span data-stu-id="5708a-183">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="5708a-184">O usuário deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="5708a-184">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="5708a-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="5708a-185">vendorInformation</span></span>|[<span data-ttu-id="5708a-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="5708a-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="5708a-187">Tipo complexo que contém detalhes sobre o fornecedor, provedor e sub-provedor de produtos/serviços de segurança (por exemplo, vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="5708a-187">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5708a-188">Relações</span><span class="sxs-lookup"><span data-stu-id="5708a-188">Relationships</span></span>

<span data-ttu-id="5708a-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5708a-189">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5708a-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5708a-190">JSON representation</span></span>

<span data-ttu-id="5708a-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5708a-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->