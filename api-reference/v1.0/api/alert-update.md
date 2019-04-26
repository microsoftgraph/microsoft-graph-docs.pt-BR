---
title: Atualizar alerta
description: Atualize uma propriedade de **alerta** editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções. Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 42bc945dde726466439802350796d628ee438e22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551503"
---
# <a name="update-alert"></a><span data-ttu-id="e0655-104">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="e0655-104">Update alert</span></span>

<span data-ttu-id="e0655-105">Atualize uma propriedade de **alerta** editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.</span><span class="sxs-lookup"><span data-stu-id="e0655-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="e0655-106">Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.</span><span class="sxs-lookup"><span data-stu-id="e0655-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0655-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0655-107">Permissions</span></span>

<span data-ttu-id="e0655-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0655-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0655-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0655-110">Permission type</span></span>                        | <span data-ttu-id="e0655-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0655-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="e0655-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0655-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0655-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0655-113">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="e0655-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0655-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0655-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0655-115">Not supported.</span></span>                      |
| <span data-ttu-id="e0655-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0655-116">Application</span></span>                            | <span data-ttu-id="e0655-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0655-117">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="e0655-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0655-118">HTTP request</span></span>

> <span data-ttu-id="e0655-119">**Observação:** Você deve incluir a ID do **alerta** como um parâmetro e vendorInformation contendo `provider` o `vendor` e com esse método.</span><span class="sxs-lookup"><span data-stu-id="e0655-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="e0655-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0655-120">Request headers</span></span>

| <span data-ttu-id="e0655-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e0655-121">Name</span></span>          | <span data-ttu-id="e0655-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0655-122">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="e0655-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0655-123">Authorization</span></span> | <span data-ttu-id="e0655-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="e0655-124">Bearer {code}.</span></span> <span data-ttu-id="e0655-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0655-125">Required.</span></span> |
| <span data-ttu-id="e0655-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="e0655-126">Prefer</span></span>        | <span data-ttu-id="e0655-127">Return = representação</span><span class="sxs-lookup"><span data-stu-id="e0655-127">return=representation</span></span>    |

## <a name="request-body"></a><span data-ttu-id="e0655-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0655-128">Request body</span></span>

<span data-ttu-id="e0655-129">No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e0655-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e0655-130">O corpo **deve** conter a `vendorInformation` Propriedade com os `provider` campos `vendor` válidos e.</span><span class="sxs-lookup"><span data-stu-id="e0655-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="e0655-131">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="e0655-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="e0655-132">Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="e0655-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="e0655-133">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e0655-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0655-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0655-134">Property</span></span>          | <span data-ttu-id="e0655-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0655-135">Type</span></span>                                                                   | <span data-ttu-id="e0655-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0655-136">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="e0655-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="e0655-137">assignedTo</span></span>        | <span data-ttu-id="e0655-138">String</span><span class="sxs-lookup"><span data-stu-id="e0655-138">String</span></span>                                                                 | <span data-ttu-id="e0655-139">Nome do analista ao qual o alerta é atribuído para a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="e0655-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="e0655-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0655-140">closedDateTime</span></span>    | <span data-ttu-id="e0655-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0655-141">DateTimeOffset</span></span>                                                         | <span data-ttu-id="e0655-142">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="e0655-142">Time at which the alert was closed.</span></span> <span data-ttu-id="e0655-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e0655-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0655-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e0655-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="e0655-145">comentários</span><span class="sxs-lookup"><span data-stu-id="e0655-145">comments</span></span>          | <span data-ttu-id="e0655-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0655-146">String collection</span></span>                                                      | <span data-ttu-id="e0655-147">Comentários de analista sobre o alerta (para o gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="e0655-147">Analyst comments on the alert (for customer alert management).</span></span> |
| <span data-ttu-id="e0655-148">comentários</span><span class="sxs-lookup"><span data-stu-id="e0655-148">feedback</span></span>          | <span data-ttu-id="e0655-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="e0655-149">alertFeedback</span></span>                                                          | <span data-ttu-id="e0655-150">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="e0655-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="e0655-151">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="e0655-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="e0655-152">status</span><span class="sxs-lookup"><span data-stu-id="e0655-152">status</span></span>            | <span data-ttu-id="e0655-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="e0655-153">alertStatus</span></span>                                                            | <span data-ttu-id="e0655-154">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="e0655-154">Alert life cycle status (stage).</span></span> <span data-ttu-id="e0655-155">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="e0655-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="e0655-156">tags</span><span class="sxs-lookup"><span data-stu-id="e0655-156">tags</span></span>              | <span data-ttu-id="e0655-157">String collection</span><span class="sxs-lookup"><span data-stu-id="e0655-157">String collection</span></span>                                                      | <span data-ttu-id="e0655-158">Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "vimos).</span><span class="sxs-lookup"><span data-stu-id="e0655-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="e0655-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="e0655-159">vendorInformation</span></span> | [<span data-ttu-id="e0655-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="e0655-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="e0655-161">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="e0655-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="e0655-162">**Os campos Provider e Vendor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="e0655-162">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="e0655-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0655-163">Response</span></span>

<span data-ttu-id="e0655-164">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e0655-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="e0655-165">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [Alert](../resources/alert.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0655-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0655-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0655-166">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="e0655-167">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="e0655-167">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="e0655-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0655-168">Request</span></span>

<span data-ttu-id="e0655-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0655-169">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="e0655-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0655-170">Response</span></span>

<span data-ttu-id="e0655-171">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="e0655-171">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="e0655-172">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="e0655-172">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="e0655-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0655-173">Request</span></span>

<span data-ttu-id="e0655-174">O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0655-174">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="e0655-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0655-175">Response</span></span>

<span data-ttu-id="e0655-176">Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.</span><span class="sxs-lookup"><span data-stu-id="e0655-176">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="e0655-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0655-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
