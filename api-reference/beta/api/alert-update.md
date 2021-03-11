---
title: Atualizar alerta
description: Atualize uma propriedade de alerta editável em qualquer solução integrada para manter o status de alerta e as atribuições em sincronia entre soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7a3adeaa6dc576182318cec5b096beced660ef5f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719973"
---
# <a name="update-alert"></a><span data-ttu-id="93f2f-103">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="93f2f-103">Update alert</span></span>

<span data-ttu-id="93f2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f2f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f2f-105">Atualize uma propriedade **de alerta editável** em qualquer solução integrada para manter o status de alerta e as atribuições em sincronia entre soluções.</span><span class="sxs-lookup"><span data-stu-id="93f2f-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="93f2f-106">Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.</span><span class="sxs-lookup"><span data-stu-id="93f2f-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="93f2f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="93f2f-107">Permissions</span></span>

<span data-ttu-id="93f2f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f2f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93f2f-110">Permission type</span></span>      | <span data-ttu-id="93f2f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93f2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f2f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93f2f-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="93f2f-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f2f-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="93f2f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93f2f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="93f2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93f2f-115">Not supported.</span></span>  |
|<span data-ttu-id="93f2f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93f2f-116">Application</span></span> | <span data-ttu-id="93f2f-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f2f-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93f2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93f2f-118">HTTP request</span></span>

> <span data-ttu-id="93f2f-119">**Observação:** Você deve incluir a ID **de** alerta como um parâmetro e vendorInformation contendo `provider` o e com este `vendor` método.</span><span class="sxs-lookup"><span data-stu-id="93f2f-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="93f2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93f2f-120">Request headers</span></span>

| <span data-ttu-id="93f2f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="93f2f-121">Name</span></span>       | <span data-ttu-id="93f2f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f2f-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="93f2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93f2f-123">Authorization</span></span>  | <span data-ttu-id="93f2f-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="93f2f-124">Bearer {code}.</span></span> <span data-ttu-id="93f2f-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93f2f-125">Required.</span></span>|
|<span data-ttu-id="93f2f-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="93f2f-126">Prefer</span></span> | <span data-ttu-id="93f2f-127">return=representation.</span><span class="sxs-lookup"><span data-stu-id="93f2f-127">return=representation.</span></span> <span data-ttu-id="93f2f-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="93f2f-128">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93f2f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93f2f-129">Request body</span></span>

<span data-ttu-id="93f2f-130">No corpo da solicitação, fornece uma representação JSON dos valores para campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="93f2f-130">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="93f2f-131">O corpo **deve** conter a **propriedade vendorInformation** com campos `provider` `vendor` válidos e válidos.</span><span class="sxs-lookup"><span data-stu-id="93f2f-131">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="93f2f-132">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="93f2f-132">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="93f2f-133">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="93f2f-133">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="93f2f-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="93f2f-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="93f2f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93f2f-135">Property</span></span>   | <span data-ttu-id="93f2f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="93f2f-136">Type</span></span> |<span data-ttu-id="93f2f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="93f2f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93f2f-138">assignedTo</span><span class="sxs-lookup"><span data-stu-id="93f2f-138">assignedTo</span></span>|<span data-ttu-id="93f2f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93f2f-139">String</span></span>|<span data-ttu-id="93f2f-140">Nome do analista ao que o alerta é atribuído para triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="93f2f-140">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="93f2f-141">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="93f2f-141">closedDateTime</span></span>|<span data-ttu-id="93f2f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93f2f-142">DateTimeOffset</span></span>|<span data-ttu-id="93f2f-143">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="93f2f-143">Time at which the alert was closed.</span></span> <span data-ttu-id="93f2f-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="93f2f-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93f2f-145">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="93f2f-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="93f2f-146">comentários</span><span class="sxs-lookup"><span data-stu-id="93f2f-146">comments</span></span>|<span data-ttu-id="93f2f-147">String collection</span><span class="sxs-lookup"><span data-stu-id="93f2f-147">String collection</span></span>|<span data-ttu-id="93f2f-148">Comentários do analista sobre o alerta (para gerenciamento de alertas do cliente).</span><span class="sxs-lookup"><span data-stu-id="93f2f-148">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="93f2f-149">Este método pode atualizar o campo de comentários apenas com os seguintes valores: `Closed in IPC` , `Closed in MCAS` .</span><span class="sxs-lookup"><span data-stu-id="93f2f-149">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span>|
|<span data-ttu-id="93f2f-150">comentários</span><span class="sxs-lookup"><span data-stu-id="93f2f-150">feedback</span></span>|<span data-ttu-id="93f2f-151">alertFeedback enum</span><span class="sxs-lookup"><span data-stu-id="93f2f-151">alertFeedback enum</span></span>|<span data-ttu-id="93f2f-152">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="93f2f-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="93f2f-153">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="93f2f-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="93f2f-154">status</span><span class="sxs-lookup"><span data-stu-id="93f2f-154">status</span></span>|<span data-ttu-id="93f2f-155">número alertStatus</span><span class="sxs-lookup"><span data-stu-id="93f2f-155">alertStatus enum</span></span>|<span data-ttu-id="93f2f-156">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="93f2f-156">Alert life cycle status (stage).</span></span> <span data-ttu-id="93f2f-157">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="93f2f-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="93f2f-158">tags</span><span class="sxs-lookup"><span data-stu-id="93f2f-158">tags</span></span>|<span data-ttu-id="93f2f-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93f2f-159">String collection</span></span>|<span data-ttu-id="93f2f-160">Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SAW).</span><span class="sxs-lookup"><span data-stu-id="93f2f-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="93f2f-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="93f2f-161">vendorInformation</span></span> |[<span data-ttu-id="93f2f-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="93f2f-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="93f2f-163">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="93f2f-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="93f2f-164">**Os campos provedor e fornecedor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="93f2f-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="93f2f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f2f-165">Response</span></span>

<span data-ttu-id="93f2f-166">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="93f2f-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="93f2f-167">Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [de](../resources/alert.md) alerta atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93f2f-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93f2f-168">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93f2f-168">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="93f2f-169">Exemplo 1: Solicitar sem o header Prefer</span><span class="sxs-lookup"><span data-stu-id="93f2f-169">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="93f2f-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93f2f-170">Request</span></span>

<span data-ttu-id="93f2f-171">A seguir, um exemplo da solicitação sem `Prefer` o header.</span><span class="sxs-lookup"><span data-stu-id="93f2f-171">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="93f2f-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="93f2f-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="93f2f-173">C#</span><span class="sxs-lookup"><span data-stu-id="93f2f-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93f2f-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93f2f-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93f2f-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93f2f-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93f2f-176">Java</span><span class="sxs-lookup"><span data-stu-id="93f2f-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="93f2f-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f2f-177">Response</span></span>

<span data-ttu-id="93f2f-178">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="93f2f-178">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="93f2f-179">Exemplo 2: Solicitar com o header Prefer</span><span class="sxs-lookup"><span data-stu-id="93f2f-179">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="93f2f-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93f2f-180">Request</span></span>

<span data-ttu-id="93f2f-181">O exemplo a seguir mostra uma solicitação que inclui o `Prefer` header de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93f2f-181">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="93f2f-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="93f2f-182">Response</span></span>

<span data-ttu-id="93f2f-183">A seguir, um exemplo da resposta quando o `Prefer: return=representation` header de solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="93f2f-183">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="93f2f-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93f2f-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


