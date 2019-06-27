---
title: Atualizar alerta
description: Atualize uma propriedade de alerta editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3ad81e698c43e8863d3081d6995fc29b1b9a9dc3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258538"
---
# <a name="update-alert"></a><span data-ttu-id="61153-103">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="61153-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61153-104">Atualize uma propriedade de **alerta** editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.</span><span class="sxs-lookup"><span data-stu-id="61153-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="61153-105">Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.</span><span class="sxs-lookup"><span data-stu-id="61153-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="61153-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61153-106">Permissions</span></span>

<span data-ttu-id="61153-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61153-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61153-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61153-109">Permission type</span></span>      | <span data-ttu-id="61153-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61153-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61153-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61153-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="61153-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61153-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="61153-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61153-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="61153-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61153-114">Not supported.</span></span>  |
|<span data-ttu-id="61153-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61153-115">Application</span></span> | <span data-ttu-id="61153-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61153-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61153-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61153-117">HTTP request</span></span>

> <span data-ttu-id="61153-118">**Observação:** Você deve incluir a ID do **alerta** como um parâmetro e vendorInformation contendo `provider` o `vendor` e com esse método.</span><span class="sxs-lookup"><span data-stu-id="61153-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="61153-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61153-119">Request headers</span></span>

| <span data-ttu-id="61153-120">Nome</span><span class="sxs-lookup"><span data-stu-id="61153-120">Name</span></span>       | <span data-ttu-id="61153-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="61153-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="61153-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61153-122">Authorization</span></span>  | <span data-ttu-id="61153-123">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="61153-123">Bearer {code}.</span></span> <span data-ttu-id="61153-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61153-124">Required.</span></span>|
|<span data-ttu-id="61153-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="61153-125">Prefer</span></span> | <span data-ttu-id="61153-126">Return = representação</span><span class="sxs-lookup"><span data-stu-id="61153-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="61153-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61153-127">Request body</span></span>

<span data-ttu-id="61153-128">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="61153-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="61153-129">O corpo **deve** conter a `vendorInformation` Propriedade com os `provider` campos `vendor` válidos e.</span><span class="sxs-lookup"><span data-stu-id="61153-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="61153-130">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="61153-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="61153-131">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="61153-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="61153-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="61153-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="61153-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61153-133">Property</span></span>   | <span data-ttu-id="61153-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="61153-134">Type</span></span> |<span data-ttu-id="61153-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="61153-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61153-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="61153-136">assignedTo</span></span>|<span data-ttu-id="61153-137">String</span><span class="sxs-lookup"><span data-stu-id="61153-137">String</span></span>|<span data-ttu-id="61153-138">Nome do analista ao qual o alerta é atribuído para a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="61153-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="61153-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="61153-139">closedDateTime</span></span>|<span data-ttu-id="61153-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61153-140">DateTimeOffset</span></span>|<span data-ttu-id="61153-141">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="61153-141">Time at which the alert was closed.</span></span> <span data-ttu-id="61153-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="61153-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61153-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="61153-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="61153-144">comentários</span><span class="sxs-lookup"><span data-stu-id="61153-144">comments</span></span>|<span data-ttu-id="61153-145">String collection</span><span class="sxs-lookup"><span data-stu-id="61153-145">String collection</span></span>|<span data-ttu-id="61153-146">Comentários de analista sobre o alerta (para o gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="61153-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="61153-147">comentários</span><span class="sxs-lookup"><span data-stu-id="61153-147">feedback</span></span>|<span data-ttu-id="61153-148">Enumeração alertFeedback</span><span class="sxs-lookup"><span data-stu-id="61153-148">alertFeedback enum</span></span>|<span data-ttu-id="61153-149">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="61153-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="61153-150">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="61153-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="61153-151">status</span><span class="sxs-lookup"><span data-stu-id="61153-151">status</span></span>|<span data-ttu-id="61153-152">Enumeração alertStatus</span><span class="sxs-lookup"><span data-stu-id="61153-152">alertStatus enum</span></span>|<span data-ttu-id="61153-153">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="61153-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="61153-154">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="61153-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="61153-155">marcações</span><span class="sxs-lookup"><span data-stu-id="61153-155">tags</span></span>|<span data-ttu-id="61153-156">String collection</span><span class="sxs-lookup"><span data-stu-id="61153-156">String collection</span></span>|<span data-ttu-id="61153-157">Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "vimos).</span><span class="sxs-lookup"><span data-stu-id="61153-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="61153-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="61153-158">vendorInformation</span></span> |[<span data-ttu-id="61153-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="61153-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="61153-160">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="61153-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="61153-161">**Os campos Provider e Vendor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="61153-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="61153-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="61153-162">Response</span></span>

<span data-ttu-id="61153-163">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="61153-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="61153-164">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [Alert](../resources/alert.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61153-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61153-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61153-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="61153-166">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="61153-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="61153-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61153-167">Request</span></span>

<span data-ttu-id="61153-168">Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="61153-168">The following is an example of the request without the `Prefer` header.</span></span>
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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="61153-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="61153-169">Response</span></span>

<span data-ttu-id="61153-170">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="61153-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="61153-171">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="61153-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="61153-172">C#</span><span class="sxs-lookup"><span data-stu-id="61153-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61153-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="61153-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_alert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="61153-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="61153-174">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_alert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="61153-175">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="61153-175">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="61153-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61153-176">Request</span></span>

<span data-ttu-id="61153-177">O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61153-177">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="61153-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="61153-178">Response</span></span>

<span data-ttu-id="61153-179">Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="61153-179">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="61153-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61153-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
