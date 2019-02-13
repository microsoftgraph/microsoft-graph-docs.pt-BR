---
title: Atualizar alerta
description: Atualize uma propriedade editável de alerta em qualquer solução integrada para manter o status de alerta e atribuições em sincronia nas soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b1fec6bfca2ce116bc35c4a7c8a115418b15012
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967323"
---
# <a name="update-alert"></a><span data-ttu-id="a849d-103">Atualizar alerta</span><span class="sxs-lookup"><span data-stu-id="a849d-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a849d-104">Atualize uma propriedade editável **alerta** dentro de qualquer solução integrada para manter o status de alerta e atribuições em sincronia nas soluções.</span><span class="sxs-lookup"><span data-stu-id="a849d-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="a849d-105">Esse método atualiza qualquer solução que tem um registro de alerta referenciado ID.</span><span class="sxs-lookup"><span data-stu-id="a849d-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a849d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a849d-106">Permissions</span></span>

<span data-ttu-id="a849d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a849d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a849d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a849d-109">Permission type</span></span>      | <span data-ttu-id="a849d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a849d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a849d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a849d-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="a849d-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a849d-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="a849d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a849d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a849d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a849d-114">Not supported.</span></span>  |
|<span data-ttu-id="a849d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a849d-115">Application</span></span> | <span data-ttu-id="a849d-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a849d-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a849d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a849d-117">HTTP request</span></span>

> <span data-ttu-id="a849d-118">**Observação:** Você deve incluir o ID de **alerta** como um parâmetro e vendorInformation contendo o `provider` e `vendor` com este método.</span><span class="sxs-lookup"><span data-stu-id="a849d-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="a849d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a849d-119">Request headers</span></span>

| <span data-ttu-id="a849d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a849d-120">Name</span></span>       | <span data-ttu-id="a849d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a849d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a849d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a849d-122">Authorization</span></span>  | <span data-ttu-id="a849d-p103">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a849d-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="a849d-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="a849d-125">Prefer</span></span> | <span data-ttu-id="a849d-126">retornar = representação</span><span class="sxs-lookup"><span data-stu-id="a849d-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="a849d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a849d-127">Request body</span></span>

<span data-ttu-id="a849d-128">No corpo da solicitação, fornece uma representação JSON dos valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a849d-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a849d-129">O corpo **deve** conter o `vendorInformation` propriedade com válido `provider` e `vendor` campos.</span><span class="sxs-lookup"><span data-stu-id="a849d-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="a849d-130">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="a849d-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="a849d-131">Os valores para propriedades existentes que não estão incluídos no corpo da solicitação não serão alterado.</span><span class="sxs-lookup"><span data-stu-id="a849d-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="a849d-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a849d-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a849d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a849d-133">Property</span></span>   | <span data-ttu-id="a849d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a849d-134">Type</span></span> |<span data-ttu-id="a849d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a849d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a849d-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a849d-136">assignedTo</span></span>|<span data-ttu-id="a849d-137">String</span><span class="sxs-lookup"><span data-stu-id="a849d-137">String</span></span>|<span data-ttu-id="a849d-138">Nome do analista de alerta é atribuída a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="a849d-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="a849d-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="a849d-139">closedDateTime</span></span>|<span data-ttu-id="a849d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a849d-140">DateTimeOffset</span></span>|<span data-ttu-id="a849d-141">Tempo em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="a849d-141">Time at which the alert was closed.</span></span> <span data-ttu-id="a849d-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a849d-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a849d-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a849d-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a849d-144">comentários</span><span class="sxs-lookup"><span data-stu-id="a849d-144">comments</span></span>|<span data-ttu-id="a849d-145">String collection</span><span class="sxs-lookup"><span data-stu-id="a849d-145">String collection</span></span>|<span data-ttu-id="a849d-146">Comentários de analistas no alerta (para gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="a849d-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="a849d-147">comentários</span><span class="sxs-lookup"><span data-stu-id="a849d-147">feedback</span></span>|<span data-ttu-id="a849d-148">enumeração alertFeedback</span><span class="sxs-lookup"><span data-stu-id="a849d-148">alertFeedback enum</span></span>|<span data-ttu-id="a849d-149">Comentários do analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="a849d-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="a849d-150">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="a849d-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="a849d-151">status</span><span class="sxs-lookup"><span data-stu-id="a849d-151">status</span></span>|<span data-ttu-id="a849d-152">enumeração alertStatus</span><span class="sxs-lookup"><span data-stu-id="a849d-152">alertStatus enum</span></span>|<span data-ttu-id="a849d-153">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="a849d-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="a849d-154">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="a849d-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="a849d-155">marcações</span><span class="sxs-lookup"><span data-stu-id="a849d-155">tags</span></span>|<span data-ttu-id="a849d-156">String collection</span><span class="sxs-lookup"><span data-stu-id="a849d-156">String collection</span></span>|<span data-ttu-id="a849d-157">Rótulos podem ser definidos pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SERRA).</span><span class="sxs-lookup"><span data-stu-id="a849d-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="a849d-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="a849d-158">vendorInformation</span></span> |[<span data-ttu-id="a849d-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="a849d-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="a849d-160">Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="a849d-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="a849d-161">**Campos de provedor e fornecedor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="a849d-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="a849d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a849d-162">Response</span></span>

<span data-ttu-id="a849d-163">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a849d-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="a849d-164">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto atualizado [alerta](../resources/alert.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a849d-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a849d-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a849d-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="a849d-166">Exemplo 1: Solicitação sem cabeçalho Prefer</span><span class="sxs-lookup"><span data-stu-id="a849d-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a849d-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a849d-167">Request</span></span>

<span data-ttu-id="a849d-168">A seguir está um exemplo da solicitação sem o `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a849d-168">The following is an example of the request without the `Prefer` header.</span></span>
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

#### <a name="response"></a><span data-ttu-id="a849d-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a849d-169">Response</span></span>

<span data-ttu-id="a849d-170">Veja a seguir o exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="a849d-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="a849d-171">Exemplo 2: Solicitação com Prefer cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a849d-171">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a849d-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a849d-172">Request</span></span>

<span data-ttu-id="a849d-173">O exemplo a seguir mostra uma solicitação que inclui o `Prefer` cabeçalho de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a849d-173">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a849d-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="a849d-174">Response</span></span>

<span data-ttu-id="a849d-175">A seguir está um exemplo da resposta quando o opcional `Prefer: return=representation` cabeçalho de solicitação é usado.</span><span class="sxs-lookup"><span data-stu-id="a849d-175">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="a849d-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a849d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
