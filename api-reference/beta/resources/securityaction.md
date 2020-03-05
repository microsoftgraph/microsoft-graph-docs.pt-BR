---
title: tipo de recurso SecurityAction
description: Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente as ações de segurança com o ATP do Windows Defender (em breve) para bloquear as atividades mal-intencionados seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 48c00d99ade3601e051d074272793d6aa0f2c66b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520826"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="4359d-106">tipo de recurso SecurityAction</span><span class="sxs-lookup"><span data-stu-id="4359d-106">securityAction resource type</span></span>

<span data-ttu-id="4359d-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4359d-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4359d-108">Executar uma ação imediata proteger contra ameaças usando a entidade securityActionde Segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4359d-108">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="4359d-109">Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4359d-109">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="4359d-110">Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário.</span><span class="sxs-lookup"><span data-stu-id="4359d-110">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="4359d-111">Experimente as ações de segurança com o [ATP do Windows Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)para bloquear as atividades mal-intencionados em seus pontos de extremidade do Windows usando as propriedades vistas nos alertas ou identificadas durante as investigações.</span><span class="sxs-lookup"><span data-stu-id="4359d-111">Try security actions with [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="4359d-112">**Observação:** ações de segurança no momento apenas dá suporte a permissões do aplicativo compatível.</span><span class="sxs-lookup"><span data-stu-id="4359d-112">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="4359d-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="4359d-113">Methods</span></span>

| <span data-ttu-id="4359d-114">Método</span><span class="sxs-lookup"><span data-stu-id="4359d-114">Method</span></span>       | <span data-ttu-id="4359d-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4359d-115">Return Type</span></span> | <span data-ttu-id="4359d-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4359d-116">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4359d-117">Obter a ação de segurança</span><span class="sxs-lookup"><span data-stu-id="4359d-117">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="4359d-118">SecurityAction</span><span class="sxs-lookup"><span data-stu-id="4359d-118">securityAction</span></span>](securityaction.md) | <span data-ttu-id="4359d-119">Leia as propriedades e as relações do objeto SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="4359d-119">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="4359d-120">Criar ação de segurança</span><span class="sxs-lookup"><span data-stu-id="4359d-120">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="4359d-121">SecurityAction</span><span class="sxs-lookup"><span data-stu-id="4359d-121">securityAction</span></span>](securityaction.md) | <span data-ttu-id="4359d-122">Crie um novo SecurityAction postando na coleção securityActions.</span><span class="sxs-lookup"><span data-stu-id="4359d-122">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="4359d-123">Listar ações de segurança</span><span class="sxs-lookup"><span data-stu-id="4359d-123">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="4359d-124">coleção [SecurityAction](securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="4359d-124">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="4359d-125">Obtenha uma coleção de objetos SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="4359d-125">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="4359d-126">Cancelar ação de segurança</span><span class="sxs-lookup"><span data-stu-id="4359d-126">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="4359d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4359d-127">None</span></span>|<span data-ttu-id="4359d-128">Cancela uma operação de segurança.</span><span class="sxs-lookup"><span data-stu-id="4359d-128">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="4359d-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4359d-129">Properties</span></span>

| <span data-ttu-id="4359d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4359d-130">Property</span></span>     | <span data-ttu-id="4359d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4359d-131">Type</span></span>        | <span data-ttu-id="4359d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4359d-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4359d-133">actionReason</span><span class="sxs-lookup"><span data-stu-id="4359d-133">actionReason</span></span>|<span data-ttu-id="4359d-134">String</span><span class="sxs-lookup"><span data-stu-id="4359d-134">String</span></span>|<span data-ttu-id="4359d-135">Motivo para invocar esta ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-135">Reason for invoking this action.</span></span>|
|<span data-ttu-id="4359d-136">appId</span><span class="sxs-lookup"><span data-stu-id="4359d-136">appId</span></span>|<span data-ttu-id="4359d-137">String</span><span class="sxs-lookup"><span data-stu-id="4359d-137">String</span></span>|<span data-ttu-id="4359d-138">A ID de aplicativo do aplicativo de chamada que enviou (POST) a ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-138">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="4359d-139">A appId deve ser extraída do token de autenticação e não inserida manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="4359d-139">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="4359d-140">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="4359d-140">azureTenantId</span></span>|<span data-ttu-id="4359d-141">String</span><span class="sxs-lookup"><span data-stu-id="4359d-141">String</span></span>|<span data-ttu-id="4359d-142">ID do locatário do Azure da entidade para determinar a qual locatário a entidade pertence (suporte a várias locação).</span><span class="sxs-lookup"><span data-stu-id="4359d-142">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="4359d-143">O azureTenantId deve ser extraído do token de autenticação e não é inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="4359d-143">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="4359d-144">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4359d-144">completedDateTime</span></span>|<span data-ttu-id="4359d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4359d-145">DateTimeOffset</span></span>|<span data-ttu-id="4359d-146">Carimbo de data/hora em que a ação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="4359d-146">Timestamp when the action was completed.</span></span> <span data-ttu-id="4359d-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4359d-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4359d-148">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4359d-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4359d-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4359d-149">createdDateTime</span></span>|<span data-ttu-id="4359d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4359d-150">DateTimeOffset</span></span>|<span data-ttu-id="4359d-151">Carimbo de data/hora em que a ação é criada.</span><span class="sxs-lookup"><span data-stu-id="4359d-151">Timestamp when the action is created.</span></span> <span data-ttu-id="4359d-152">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4359d-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4359d-153">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4359d-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4359d-154">errorInfo</span><span class="sxs-lookup"><span data-stu-id="4359d-154">errorInfo</span></span>|[<span data-ttu-id="4359d-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4359d-155">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="4359d-156">Informações de erro quando a ação falha.</span><span class="sxs-lookup"><span data-stu-id="4359d-156">Error info when the action fails.</span></span>|
|<span data-ttu-id="4359d-157">id</span><span class="sxs-lookup"><span data-stu-id="4359d-157">id</span></span>|<span data-ttu-id="4359d-158">String</span><span class="sxs-lookup"><span data-stu-id="4359d-158">String</span></span>| <span data-ttu-id="4359d-159">Criado pelo sistema quando a ação é ingerida.</span><span class="sxs-lookup"><span data-stu-id="4359d-159">Created by the system when the action is ingested.</span></span> <span data-ttu-id="4359d-160">GUID gerado/identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="4359d-160">Generated GUID/unique identifier.</span></span> <span data-ttu-id="4359d-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4359d-161">Read-only.</span></span>|
|<span data-ttu-id="4359d-162">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4359d-162">lastActionDateTime</span></span>|<span data-ttu-id="4359d-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4359d-163">DateTimeOffset</span></span>| <span data-ttu-id="4359d-164">Carimbo de data/hora da última atualização da ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-164">Timestamp when this action was last updated.</span></span> <span data-ttu-id="4359d-165">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4359d-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4359d-166">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4359d-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4359d-167">nome</span><span class="sxs-lookup"><span data-stu-id="4359d-167">name</span></span>|<span data-ttu-id="4359d-168">String</span><span class="sxs-lookup"><span data-stu-id="4359d-168">String</span></span>| <span data-ttu-id="4359d-169">Nome da ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-169">Action name.</span></span>|
|<span data-ttu-id="4359d-170">parameters</span><span class="sxs-lookup"><span data-stu-id="4359d-170">parameters</span></span>|<span data-ttu-id="4359d-171">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4359d-171">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="4359d-172">Coleção de parâmetros (pares chave-valor) necessário para invocar a ação, por exemplo, URL ou FileHash para bloquear, etc.).</span><span class="sxs-lookup"><span data-stu-id="4359d-172">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="4359d-173">**Required**</span><span class="sxs-lookup"><span data-stu-id="4359d-173">**Required**</span></span>|
|<span data-ttu-id="4359d-174">determina</span><span class="sxs-lookup"><span data-stu-id="4359d-174">states</span></span>|<span data-ttu-id="4359d-175">coleção [securityActionState](securityactionstate.md)</span><span class="sxs-lookup"><span data-stu-id="4359d-175">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="4359d-176">Coleção de securityActionState para manter o histórico de uma ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-176">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="4359d-177">status</span><span class="sxs-lookup"><span data-stu-id="4359d-177">status</span></span>|<span data-ttu-id="4359d-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4359d-178">string</span></span>| <span data-ttu-id="4359d-179">Status da ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-179">Status of the action.</span></span> <span data-ttu-id="4359d-180">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="4359d-180">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="4359d-181">user</span><span class="sxs-lookup"><span data-stu-id="4359d-181">user</span></span>|<span data-ttu-id="4359d-182">String</span><span class="sxs-lookup"><span data-stu-id="4359d-182">String</span></span>| <span data-ttu-id="4359d-183">O nome principal de usuário do usuário conectado que enviou (POST) a ação.</span><span class="sxs-lookup"><span data-stu-id="4359d-183">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="4359d-184">O usuário deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="4359d-184">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="4359d-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="4359d-185">vendorInformation</span></span>|[<span data-ttu-id="4359d-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="4359d-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="4359d-187">Tipo complexo que contém detalhes sobre o fornecedor de produtos/serviços de segurança, o provedor e o subprovedor (por exemplo, fornecedor = Microsoft; Provider = Windows Defender ATP; subprovider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="4359d-187">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4359d-188">Relações</span><span class="sxs-lookup"><span data-stu-id="4359d-188">Relationships</span></span>

<span data-ttu-id="4359d-189">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4359d-189">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4359d-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4359d-190">JSON representation</span></span>

<span data-ttu-id="4359d-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4359d-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
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