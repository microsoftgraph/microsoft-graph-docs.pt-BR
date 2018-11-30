---
title: Atualizar alertas
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 9f8040220c64310a04293d43c0c31704c3f49261
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2018
ms.locfileid: "27041224"
---
# <a name="update-alert"></a><span data-ttu-id="98720-104">Atualizar alertas</span><span class="sxs-lookup"><span data-stu-id="98720-104">Update alert</span></span>

 > <span data-ttu-id="98720-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="98720-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98720-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98720-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98720-107">Atualize uma propriedade editável **alerta** dentro de qualquer solução integrada para manter o status de alerta e atribuições em sincronia nas soluções.</span><span class="sxs-lookup"><span data-stu-id="98720-107">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="98720-108">Esse método atualiza qualquer solução que tem um registro de alerta referenciado ID.</span><span class="sxs-lookup"><span data-stu-id="98720-108">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="98720-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="98720-109">Permissions</span></span>

<span data-ttu-id="98720-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98720-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98720-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98720-112">Permission type</span></span>      | <span data-ttu-id="98720-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98720-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98720-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98720-114">Delegated (work or school account)</span></span> |   <span data-ttu-id="98720-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98720-115">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="98720-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98720-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="98720-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98720-117">Not supported.</span></span>  |
|<span data-ttu-id="98720-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98720-118">Application</span></span> | <span data-ttu-id="98720-119">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98720-119">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98720-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98720-120">HTTP request</span></span>

> <span data-ttu-id="98720-121">**Observação:** Você deve incluir o ID de **alerta** como um parâmetro e vendorInformation contendo o `provider` e `vendor` com este método.</span><span class="sxs-lookup"><span data-stu-id="98720-121">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="98720-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98720-122">Request headers</span></span>

| <span data-ttu-id="98720-123">Nome</span><span class="sxs-lookup"><span data-stu-id="98720-123">Name</span></span>       | <span data-ttu-id="98720-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="98720-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="98720-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="98720-125">Authorization</span></span>  | <span data-ttu-id="98720-p105">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98720-p105">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="98720-128">Preferir</span><span class="sxs-lookup"><span data-stu-id="98720-128">Prefer</span></span> | <span data-ttu-id="98720-129">retornar = representação</span><span class="sxs-lookup"><span data-stu-id="98720-129">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="98720-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98720-130">Request body</span></span>

<span data-ttu-id="98720-131">No corpo da solicitação, fornece uma representação JSON dos valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="98720-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="98720-132">O corpo **deve** conter o `vendorInformation` propriedade com válido `provider` e `vendor` campos.</span><span class="sxs-lookup"><span data-stu-id="98720-132">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="98720-133">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="98720-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="98720-134">Os valores para propriedades existentes que não estão incluídos no corpo da solicitação não serão alterado.</span><span class="sxs-lookup"><span data-stu-id="98720-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="98720-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="98720-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="98720-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98720-136">Property</span></span>   | <span data-ttu-id="98720-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="98720-137">Type</span></span> |<span data-ttu-id="98720-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="98720-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98720-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="98720-139">assignedTo</span></span>|<span data-ttu-id="98720-140">String</span><span class="sxs-lookup"><span data-stu-id="98720-140">String</span></span>|<span data-ttu-id="98720-141">Nome do analista de alerta é atribuída a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="98720-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="98720-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="98720-142">closedDateTime</span></span>|<span data-ttu-id="98720-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98720-143">DateTimeOffset</span></span>|<span data-ttu-id="98720-144">Hora em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="98720-144">Time at which the alert was closed.</span></span> <span data-ttu-id="98720-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="98720-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="98720-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="98720-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="98720-147">comentários</span><span class="sxs-lookup"><span data-stu-id="98720-147">comments</span></span>|<span data-ttu-id="98720-148">String collection</span><span class="sxs-lookup"><span data-stu-id="98720-148">String collection</span></span>|<span data-ttu-id="98720-149">Comentários de analistas no alerta (para gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="98720-149">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="98720-150">comentários</span><span class="sxs-lookup"><span data-stu-id="98720-150">feedback</span></span>|<span data-ttu-id="98720-151">enumeração alertFeedback</span><span class="sxs-lookup"><span data-stu-id="98720-151">alertFeedback enum</span></span>|<span data-ttu-id="98720-152">Comentários analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="98720-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="98720-153">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="98720-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="98720-154">status</span><span class="sxs-lookup"><span data-stu-id="98720-154">status</span></span>|<span data-ttu-id="98720-155">enumeração alertStatus</span><span class="sxs-lookup"><span data-stu-id="98720-155">alertStatus enum</span></span>|<span data-ttu-id="98720-156">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="98720-156">Alert lifecycle status (stage).</span></span> <span data-ttu-id="98720-157">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="98720-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="98720-158">marcas</span><span class="sxs-lookup"><span data-stu-id="98720-158">tags</span></span>|<span data-ttu-id="98720-159">String collection</span><span class="sxs-lookup"><span data-stu-id="98720-159">String collection</span></span>|<span data-ttu-id="98720-160">Rótulos podem ser definidos pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SERRA).</span><span class="sxs-lookup"><span data-stu-id="98720-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="98720-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="98720-161">vendorInformation</span></span> |[<span data-ttu-id="98720-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="98720-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="98720-163">Tipo complexo que contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="98720-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="98720-164">**Campos de provedor e fornecedor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="98720-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="98720-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="98720-165">Response</span></span>

<span data-ttu-id="98720-166">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98720-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="98720-167">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto atualizado [alerta](../resources/alert.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98720-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="98720-168">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="98720-168">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="98720-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98720-169">Request</span></span>

<span data-ttu-id="98720-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98720-170">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a><span data-ttu-id="98720-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="98720-171">Response</span></span>

<span data-ttu-id="98720-172">O exemplo a seguir é um exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="98720-172">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="98720-173">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="98720-173">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="98720-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98720-174">Request</span></span>

<span data-ttu-id="98720-175">O exemplo a seguir mostra uma solicitação que inclui o `Prefer` cabeçalho de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98720-175">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a><span data-ttu-id="98720-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="98720-176">Response</span></span>

<span data-ttu-id="98720-177">A seguir está um exemplo da resposta quando o opcional `Prefer: return=representation` cabeçalho de solicitação é usado.</span><span class="sxs-lookup"><span data-stu-id="98720-177">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="98720-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98720-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
