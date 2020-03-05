---
title: Atualizar alerta
description: Atualize uma propriedade de alerta editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 963440a7d8d2c6035660a1cc831b474dbab68ee0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441610"
---
# <a name="update-alert"></a><span data-ttu-id="29ebe-103">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="29ebe-103">Update alert</span></span>

<span data-ttu-id="29ebe-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29ebe-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ebe-105">Atualize uma propriedade de **alerta** editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.</span><span class="sxs-lookup"><span data-stu-id="29ebe-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="29ebe-106">Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.</span><span class="sxs-lookup"><span data-stu-id="29ebe-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="29ebe-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29ebe-107">Permissions</span></span>

<span data-ttu-id="29ebe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29ebe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29ebe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29ebe-110">Permission type</span></span>      | <span data-ttu-id="29ebe-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29ebe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29ebe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29ebe-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="29ebe-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29ebe-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="29ebe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29ebe-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="29ebe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29ebe-115">Not supported.</span></span>  |
|<span data-ttu-id="29ebe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29ebe-116">Application</span></span> | <span data-ttu-id="29ebe-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29ebe-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29ebe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29ebe-118">HTTP request</span></span>

> <span data-ttu-id="29ebe-119">**Observação:** Você deve incluir a ID do **alerta** como um parâmetro e vendorInformation contendo `provider` o `vendor` e com esse método.</span><span class="sxs-lookup"><span data-stu-id="29ebe-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="29ebe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29ebe-120">Request headers</span></span>

| <span data-ttu-id="29ebe-121">Nome</span><span class="sxs-lookup"><span data-stu-id="29ebe-121">Name</span></span>       | <span data-ttu-id="29ebe-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="29ebe-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="29ebe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29ebe-123">Authorization</span></span>  | <span data-ttu-id="29ebe-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="29ebe-124">Bearer {code}.</span></span> <span data-ttu-id="29ebe-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29ebe-125">Required.</span></span>|
|<span data-ttu-id="29ebe-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="29ebe-126">Prefer</span></span> | <span data-ttu-id="29ebe-127">Return = representação.</span><span class="sxs-lookup"><span data-stu-id="29ebe-127">return=representation.</span></span> <span data-ttu-id="29ebe-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="29ebe-128">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29ebe-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29ebe-129">Request body</span></span>

<span data-ttu-id="29ebe-130">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="29ebe-130">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="29ebe-131">O corpo **deve** conter a propriedade **vendorInformation** com os `provider` campos `vendor` válidos e.</span><span class="sxs-lookup"><span data-stu-id="29ebe-131">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="29ebe-132">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="29ebe-132">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="29ebe-133">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="29ebe-133">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="29ebe-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="29ebe-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="29ebe-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29ebe-135">Property</span></span>   | <span data-ttu-id="29ebe-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="29ebe-136">Type</span></span> |<span data-ttu-id="29ebe-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="29ebe-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29ebe-138">assignedTo</span><span class="sxs-lookup"><span data-stu-id="29ebe-138">assignedTo</span></span>|<span data-ttu-id="29ebe-139">String</span><span class="sxs-lookup"><span data-stu-id="29ebe-139">String</span></span>|<span data-ttu-id="29ebe-140">Nome do analista ao qual o alerta é atribuído para a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="29ebe-140">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="29ebe-141">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="29ebe-141">closedDateTime</span></span>|<span data-ttu-id="29ebe-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29ebe-142">DateTimeOffset</span></span>|<span data-ttu-id="29ebe-143">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="29ebe-143">Time at which the alert was closed.</span></span> <span data-ttu-id="29ebe-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="29ebe-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29ebe-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29ebe-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29ebe-146">comentários</span><span class="sxs-lookup"><span data-stu-id="29ebe-146">comments</span></span>|<span data-ttu-id="29ebe-147">String collection</span><span class="sxs-lookup"><span data-stu-id="29ebe-147">String collection</span></span>|<span data-ttu-id="29ebe-148">Comentários de analista sobre o alerta (para o gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="29ebe-148">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="29ebe-149">Este método pode atualizar o campo Comments com os seguintes valores apenas `Closed in IPC`: `Closed in MCAS`,.</span><span class="sxs-lookup"><span data-stu-id="29ebe-149">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span>|
|<span data-ttu-id="29ebe-150">comentários</span><span class="sxs-lookup"><span data-stu-id="29ebe-150">feedback</span></span>|<span data-ttu-id="29ebe-151">Enumeração alertFeedback</span><span class="sxs-lookup"><span data-stu-id="29ebe-151">alertFeedback enum</span></span>|<span data-ttu-id="29ebe-152">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="29ebe-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="29ebe-153">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="29ebe-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="29ebe-154">status</span><span class="sxs-lookup"><span data-stu-id="29ebe-154">status</span></span>|<span data-ttu-id="29ebe-155">Enumeração alertStatus</span><span class="sxs-lookup"><span data-stu-id="29ebe-155">alertStatus enum</span></span>|<span data-ttu-id="29ebe-156">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="29ebe-156">Alert life cycle status (stage).</span></span> <span data-ttu-id="29ebe-157">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="29ebe-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="29ebe-158">tags</span><span class="sxs-lookup"><span data-stu-id="29ebe-158">tags</span></span>|<span data-ttu-id="29ebe-159">String collection</span><span class="sxs-lookup"><span data-stu-id="29ebe-159">String collection</span></span>|<span data-ttu-id="29ebe-160">Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "vimos).</span><span class="sxs-lookup"><span data-stu-id="29ebe-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="29ebe-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="29ebe-161">vendorInformation</span></span> |[<span data-ttu-id="29ebe-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="29ebe-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="29ebe-163">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="29ebe-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="29ebe-164">**Os campos Provider e Vendor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="29ebe-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="29ebe-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ebe-165">Response</span></span>

<span data-ttu-id="29ebe-166">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29ebe-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="29ebe-167">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [Alert](../resources/alert.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29ebe-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29ebe-168">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29ebe-168">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="29ebe-169">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="29ebe-169">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="29ebe-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29ebe-170">Request</span></span>

<span data-ttu-id="29ebe-171">Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="29ebe-171">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="29ebe-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="29ebe-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="29ebe-173">C#</span><span class="sxs-lookup"><span data-stu-id="29ebe-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29ebe-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29ebe-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29ebe-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29ebe-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="29ebe-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ebe-176">Response</span></span>

<span data-ttu-id="29ebe-177">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="29ebe-177">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="29ebe-178">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="29ebe-178">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="29ebe-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29ebe-179">Request</span></span>

<span data-ttu-id="29ebe-180">O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29ebe-180">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="29ebe-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ebe-181">Response</span></span>

<span data-ttu-id="29ebe-182">Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="29ebe-182">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="29ebe-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29ebe-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
