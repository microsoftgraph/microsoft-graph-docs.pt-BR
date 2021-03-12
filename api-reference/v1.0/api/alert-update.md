---
title: Atualizar alerta
description: Atualize uma propriedade **de alerta editável** em qualquer solução integrada para manter o status de alerta e as atribuições em sincronia entre soluções. Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 92edfc5e312b56170aa1c8924dad6b2b48970839
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721422"
---
# <a name="update-alert"></a><span data-ttu-id="83273-104">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="83273-104">Update alert</span></span>

<span data-ttu-id="83273-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83273-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83273-106">Atualize uma propriedade **de alerta editável** em qualquer solução integrada para manter o status de alerta e as atribuições em sincronia entre soluções.</span><span class="sxs-lookup"><span data-stu-id="83273-106">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="83273-107">Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.</span><span class="sxs-lookup"><span data-stu-id="83273-107">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="83273-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="83273-108">Permissions</span></span>

<span data-ttu-id="83273-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83273-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83273-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83273-111">Permission type</span></span>                        | <span data-ttu-id="83273-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83273-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="83273-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83273-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="83273-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83273-114">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="83273-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83273-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83273-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83273-116">Not supported.</span></span>                      |
| <span data-ttu-id="83273-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83273-117">Application</span></span>                            | <span data-ttu-id="83273-118">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83273-118">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="83273-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83273-119">HTTP request</span></span>

> <span data-ttu-id="83273-120">**Observação:** Você deve incluir a ID **de** alerta como um parâmetro e vendorInformation contendo `provider` o e com este `vendor` método.</span><span class="sxs-lookup"><span data-stu-id="83273-120">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="83273-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83273-121">Request headers</span></span>

| <span data-ttu-id="83273-122">Nome</span><span class="sxs-lookup"><span data-stu-id="83273-122">Name</span></span>          | <span data-ttu-id="83273-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="83273-123">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="83273-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="83273-124">Authorization</span></span> | <span data-ttu-id="83273-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="83273-125">Bearer {code}.</span></span> <span data-ttu-id="83273-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83273-126">Required.</span></span> |
| <span data-ttu-id="83273-127">Preferir</span><span class="sxs-lookup"><span data-stu-id="83273-127">Prefer</span></span>        | <span data-ttu-id="83273-128">return=representation.</span><span class="sxs-lookup"><span data-stu-id="83273-128">return=representation.</span></span> <span data-ttu-id="83273-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="83273-129">Optional.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="83273-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83273-130">Request body</span></span>

<span data-ttu-id="83273-131">No corpo da solicitação, fornece uma representação JSON dos valores para campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="83273-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="83273-132">O corpo **deve** conter a **propriedade vendorInformation** com campos `provider` `vendor` válidos e válidos.</span><span class="sxs-lookup"><span data-stu-id="83273-132">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="83273-133">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="83273-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="83273-134">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="83273-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="83273-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="83273-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="83273-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83273-136">Property</span></span>          | <span data-ttu-id="83273-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="83273-137">Type</span></span>                                                                   | <span data-ttu-id="83273-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="83273-138">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="83273-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="83273-139">assignedTo</span></span>        | <span data-ttu-id="83273-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83273-140">String</span></span>                                                                 | <span data-ttu-id="83273-141">Nome do analista ao que o alerta é atribuído para triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="83273-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="83273-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="83273-142">closedDateTime</span></span>    | <span data-ttu-id="83273-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83273-143">DateTimeOffset</span></span>                                                         | <span data-ttu-id="83273-144">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="83273-144">Time at which the alert was closed.</span></span> <span data-ttu-id="83273-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="83273-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="83273-146">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="83273-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="83273-147">comentários</span><span class="sxs-lookup"><span data-stu-id="83273-147">comments</span></span>          | <span data-ttu-id="83273-148">String collection</span><span class="sxs-lookup"><span data-stu-id="83273-148">String collection</span></span>                                                      | <span data-ttu-id="83273-149">Comentários do analista sobre o alerta (para gerenciamento de alertas do cliente).</span><span class="sxs-lookup"><span data-stu-id="83273-149">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="83273-150">Este método pode atualizar o campo de comentários apenas com os seguintes valores: `Closed in IPC` , `Closed in MCAS` .</span><span class="sxs-lookup"><span data-stu-id="83273-150">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span> |
| <span data-ttu-id="83273-151">comentários</span><span class="sxs-lookup"><span data-stu-id="83273-151">feedback</span></span>          | <span data-ttu-id="83273-152">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="83273-152">alertFeedback</span></span>                                                          | <span data-ttu-id="83273-153">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="83273-153">Analyst feedback on the alert.</span></span> <span data-ttu-id="83273-154">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="83273-154">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="83273-155">status</span><span class="sxs-lookup"><span data-stu-id="83273-155">status</span></span>            | <span data-ttu-id="83273-156">alertStatus</span><span class="sxs-lookup"><span data-stu-id="83273-156">alertStatus</span></span>                                                            | <span data-ttu-id="83273-157">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="83273-157">Alert life cycle status (stage).</span></span> <span data-ttu-id="83273-158">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="83273-158">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="83273-159">tags</span><span class="sxs-lookup"><span data-stu-id="83273-159">tags</span></span>              | <span data-ttu-id="83273-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="83273-160">String collection</span></span>                                                      | <span data-ttu-id="83273-161">Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SAW).</span><span class="sxs-lookup"><span data-stu-id="83273-161">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="83273-162">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="83273-162">vendorInformation</span></span> | [<span data-ttu-id="83273-163">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="83273-163">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="83273-164">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="83273-164">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="83273-165">**Os campos provedor e fornecedor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="83273-165">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="83273-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="83273-166">Response</span></span>

<span data-ttu-id="83273-167">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="83273-167">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="83273-168">Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [de](../resources/alert.md) alerta atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83273-168">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83273-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83273-169">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="83273-170">Exemplo 1: Solicitar sem o header Prefer</span><span class="sxs-lookup"><span data-stu-id="83273-170">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="83273-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83273-171">Request</span></span>

<span data-ttu-id="83273-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83273-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83273-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="83273-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="83273-174">C#</span><span class="sxs-lookup"><span data-stu-id="83273-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83273-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83273-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83273-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83273-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83273-177">Java</span><span class="sxs-lookup"><span data-stu-id="83273-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="83273-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="83273-178">Response</span></span>

<span data-ttu-id="83273-179">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="83273-179">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="83273-180">Exemplo 2: Solicitar com o header Prefer</span><span class="sxs-lookup"><span data-stu-id="83273-180">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="83273-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83273-181">Request</span></span>

<span data-ttu-id="83273-182">O exemplo a seguir mostra uma solicitação que inclui o `Prefer` header de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83273-182">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

#### <a name="response"></a><span data-ttu-id="83273-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="83273-183">Response</span></span>

<span data-ttu-id="83273-184">A seguir, um exemplo da resposta quando o `Prefer: return=representation` header de solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="83273-184">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="83273-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83273-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

