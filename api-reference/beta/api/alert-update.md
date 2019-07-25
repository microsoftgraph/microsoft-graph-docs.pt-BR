---
title: Atualizar alerta
description: Atualize uma propriedade de alerta editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 47c5499a49ce6e9f4bae7962a0a30e26a7290ed2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855369"
---
# <a name="update-alert"></a><span data-ttu-id="ac310-103">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="ac310-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac310-104">Atualize uma propriedade de **alerta** editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.</span><span class="sxs-lookup"><span data-stu-id="ac310-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="ac310-105">Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.</span><span class="sxs-lookup"><span data-stu-id="ac310-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac310-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac310-106">Permissions</span></span>

<span data-ttu-id="ac310-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac310-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac310-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac310-109">Permission type</span></span>      | <span data-ttu-id="ac310-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac310-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac310-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac310-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="ac310-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac310-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="ac310-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac310-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ac310-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac310-114">Not supported.</span></span>  |
|<span data-ttu-id="ac310-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac310-115">Application</span></span> | <span data-ttu-id="ac310-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac310-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac310-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac310-117">HTTP request</span></span>

> <span data-ttu-id="ac310-118">**Observação:** Você deve incluir a ID do **alerta** como um parâmetro e vendorInformation contendo `provider` o `vendor` e com esse método.</span><span class="sxs-lookup"><span data-stu-id="ac310-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="ac310-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac310-119">Request headers</span></span>

| <span data-ttu-id="ac310-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ac310-120">Name</span></span>       | <span data-ttu-id="ac310-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac310-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac310-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac310-122">Authorization</span></span>  | <span data-ttu-id="ac310-123">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="ac310-123">Bearer {code}.</span></span> <span data-ttu-id="ac310-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac310-124">Required.</span></span>|
|<span data-ttu-id="ac310-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="ac310-125">Prefer</span></span> | <span data-ttu-id="ac310-126">Return = representação</span><span class="sxs-lookup"><span data-stu-id="ac310-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac310-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac310-127">Request body</span></span>

<span data-ttu-id="ac310-128">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ac310-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ac310-129">O corpo **deve** conter a `vendorInformation` Propriedade com os `provider` campos `vendor` válidos e.</span><span class="sxs-lookup"><span data-stu-id="ac310-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="ac310-130">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="ac310-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="ac310-131">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="ac310-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="ac310-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ac310-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ac310-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac310-133">Property</span></span>   | <span data-ttu-id="ac310-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac310-134">Type</span></span> |<span data-ttu-id="ac310-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac310-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac310-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="ac310-136">assignedTo</span></span>|<span data-ttu-id="ac310-137">String</span><span class="sxs-lookup"><span data-stu-id="ac310-137">String</span></span>|<span data-ttu-id="ac310-138">Nome do analista ao qual o alerta é atribuído para a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="ac310-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="ac310-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac310-139">closedDateTime</span></span>|<span data-ttu-id="ac310-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac310-140">DateTimeOffset</span></span>|<span data-ttu-id="ac310-141">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="ac310-141">Time at which the alert was closed.</span></span> <span data-ttu-id="ac310-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ac310-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac310-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ac310-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ac310-144">comentários</span><span class="sxs-lookup"><span data-stu-id="ac310-144">comments</span></span>|<span data-ttu-id="ac310-145">String collection</span><span class="sxs-lookup"><span data-stu-id="ac310-145">String collection</span></span>|<span data-ttu-id="ac310-146">Comentários de analista sobre o alerta (para o gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="ac310-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="ac310-147">comentários</span><span class="sxs-lookup"><span data-stu-id="ac310-147">feedback</span></span>|<span data-ttu-id="ac310-148">Enumeração alertFeedback</span><span class="sxs-lookup"><span data-stu-id="ac310-148">alertFeedback enum</span></span>|<span data-ttu-id="ac310-149">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="ac310-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="ac310-150">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="ac310-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="ac310-151">status</span><span class="sxs-lookup"><span data-stu-id="ac310-151">status</span></span>|<span data-ttu-id="ac310-152">Enumeração alertStatus</span><span class="sxs-lookup"><span data-stu-id="ac310-152">alertStatus enum</span></span>|<span data-ttu-id="ac310-153">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="ac310-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="ac310-154">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="ac310-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="ac310-155">marcações</span><span class="sxs-lookup"><span data-stu-id="ac310-155">tags</span></span>|<span data-ttu-id="ac310-156">String collection</span><span class="sxs-lookup"><span data-stu-id="ac310-156">String collection</span></span>|<span data-ttu-id="ac310-157">Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "vimos).</span><span class="sxs-lookup"><span data-stu-id="ac310-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="ac310-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="ac310-158">vendorInformation</span></span> |[<span data-ttu-id="ac310-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="ac310-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="ac310-160">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="ac310-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="ac310-161">**Os campos Provider e Vendor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="ac310-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="ac310-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac310-162">Response</span></span>

<span data-ttu-id="ac310-163">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac310-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="ac310-164">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [Alert](../resources/alert.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac310-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac310-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ac310-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="ac310-166">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="ac310-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="ac310-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac310-167">Request</span></span>

<span data-ttu-id="ac310-168">Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="ac310-168">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ac310-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac310-169">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac310-170">C#</span><span class="sxs-lookup"><span data-stu-id="ac310-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac310-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="ac310-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac310-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ac310-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ac310-173">Java</span><span class="sxs-lookup"><span data-stu-id="ac310-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="ac310-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac310-174">Response</span></span>

<span data-ttu-id="ac310-175">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ac310-175">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="ac310-176">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="ac310-176">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="ac310-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac310-177">Request</span></span>

<span data-ttu-id="ac310-178">O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac310-178">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="ac310-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac310-179">Response</span></span>

<span data-ttu-id="ac310-180">Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="ac310-180">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="ac310-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac310-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
