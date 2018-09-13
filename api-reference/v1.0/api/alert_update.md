# <a name="update-alert"></a><span data-ttu-id="f2c62-101">Update alert</span><span class="sxs-lookup"><span data-stu-id="f2c62-101">Update alert</span></span>

<span data-ttu-id="f2c62-102">Atualiza uma propriedade editável **alert** dentro de qualquer solução integrada para manter o status do alerta e as tarefas atribuídas em sincronia em todas soluções.</span><span class="sxs-lookup"><span data-stu-id="f2c62-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="f2c62-103">Este método atualiza qualquer solução que tenha um registro do alerta referenciado pelo ID.</span><span class="sxs-lookup"><span data-stu-id="f2c62-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c62-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2c62-104">Permissions</span></span>

<span data-ttu-id="f2c62-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2c62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2c62-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2c62-107">Permission type</span></span>      | <span data-ttu-id="f2c62-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2c62-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c62-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2c62-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="f2c62-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c62-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="f2c62-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2c62-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f2c62-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2c62-112">Not supported.</span></span>  |
|<span data-ttu-id="f2c62-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c62-113">Application</span></span> | <span data-ttu-id="f2c62-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c62-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2c62-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c62-115">HTTP request</span></span>

> <span data-ttu-id="f2c62-116">**Observação:** Você deve incluir o ID do **alerta** como parâmetro e vendorInformation contendo `provider` e `vendor` neste método.</span><span class="sxs-lookup"><span data-stu-id="f2c62-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="f2c62-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c62-117">Request headers</span></span>

| <span data-ttu-id="f2c62-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f2c62-118">Name</span></span>       | <span data-ttu-id="f2c62-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c62-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f2c62-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2c62-120">Authorization</span></span>  | <span data-ttu-id="f2c62-p103">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2c62-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="f2c62-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="f2c62-123">Prefer</span></span> | <span data-ttu-id="f2c62-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="f2c62-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2c62-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c62-125">Request body</span></span>

<span data-ttu-id="f2c62-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f2c62-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f2c62-127">O corpo **deve** conter a propriedade `vendorInformation` com os campos `provider` e `vendor` válidos.</span><span class="sxs-lookup"><span data-stu-id="f2c62-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="f2c62-128">A tabela a seguir lista os campos que podem ser atualizados em um alerta.</span><span class="sxs-lookup"><span data-stu-id="f2c62-128">The following table lists the authentication settings that can be changed for an authentication provider.</span></span> <span data-ttu-id="f2c62-129">Os valores para propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados.</span><span class="sxs-lookup"><span data-stu-id="f2c62-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="f2c62-130">Para alcançar um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f2c62-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f2c62-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2c62-131">Property</span></span>   | <span data-ttu-id="f2c62-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2c62-132">Type</span></span> |<span data-ttu-id="f2c62-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c62-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2c62-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="f2c62-134">assignedTo</span></span>|<span data-ttu-id="f2c62-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2c62-135">String</span></span>|<span data-ttu-id="f2c62-136">Nome do analista para quem foi atribuída a triagem, investigação ou correção do alerta.</span><span class="sxs-lookup"><span data-stu-id="f2c62-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="f2c62-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2c62-137">closedDateTime</span></span>|<span data-ttu-id="f2c62-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2c62-138">DateTimeOffset</span></span>|<span data-ttu-id="f2c62-139">Hora em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="f2c62-139">Time at which the alert was closed.</span></span> <span data-ttu-id="f2c62-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f2c62-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2c62-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f2c62-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f2c62-142">comments</span><span class="sxs-lookup"><span data-stu-id="f2c62-142">comments</span></span>|<span data-ttu-id="f2c62-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2c62-143">String collection</span></span>|<span data-ttu-id="f2c62-144">Comentários do analista sobre o alerta (para gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="f2c62-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="f2c62-145">feedback</span><span class="sxs-lookup"><span data-stu-id="f2c62-145">Feedback</span></span>|<span data-ttu-id="f2c62-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="f2c62-146">alertFeedback</span></span>|<span data-ttu-id="f2c62-147">Feedback do analista sobre o alerta.</span><span class="sxs-lookup"><span data-stu-id="f2c62-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="f2c62-148">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="f2c62-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="f2c62-149">status</span><span class="sxs-lookup"><span data-stu-id="f2c62-149">status</span></span>|<span data-ttu-id="f2c62-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="f2c62-150">alertStatus</span></span>|<span data-ttu-id="f2c62-151">Status do ciclo de vida do alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="f2c62-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="f2c62-152">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="f2c62-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="f2c62-153">tags</span><span class="sxs-lookup"><span data-stu-id="f2c62-153">tags</span></span>|<span data-ttu-id="f2c62-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2c62-154">String collection</span></span>|<span data-ttu-id="f2c62-155">Rótulos definidos pelo usuário que podem ser aplicados a um alerta e servir como condições de filtro (por exemplo, "HVA", "SAW").</span><span class="sxs-lookup"><span data-stu-id="f2c62-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="f2c62-156">vendorInformation \*</span><span class="sxs-lookup"><span data-stu-id="f2c62-156">vendorInformation \*</span></span>|[<span data-ttu-id="f2c62-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f2c62-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="f2c62-158">Tipo complexo contendo detalhes sobre o produto de segurança/provedor de serviço (por exemplo, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="f2c62-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="f2c62-159">**Os campos provider e vendor são obrigatórios.**</span><span class="sxs-lookup"><span data-stu-id="f2c62-159">**Provider and vendor fields are required.**</span></span>|
<span data-ttu-id="f2c62-160">(\* Indica um campo obrigatório.)</span><span class="sxs-lookup"><span data-stu-id="f2c62-160">(\* Indicates a mandatory field.)</span></span>

## <a name="response"></a><span data-ttu-id="f2c62-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c62-161">Response</span></span>

<span data-ttu-id="f2c62-162">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2c62-162">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f2c62-163">Se o cabeçalho opcional da solicitação for usado, o método retornará um código de resposta `200 OK` e o objeto [alert](../resources/alert.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c62-163">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="f2c62-164">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="f2c62-164">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="f2c62-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c62-165">Request</span></span>

<span data-ttu-id="f2c62-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2c62-166">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2c62-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c62-167">Response</span></span>

<span data-ttu-id="f2c62-168">Este é um exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f2c62-168">The following is an example of a response to a  event.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="f2c62-169">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="f2c62-169">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="f2c62-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c62-170">Request</span></span>

<span data-ttu-id="f2c62-171">O exemplo a seguir mostra uma solicitação que inclui o cabeçalho de solicitação `Prefer`.</span><span class="sxs-lookup"><span data-stu-id="f2c62-171">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="f2c62-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c62-172">Response</span></span>

<span data-ttu-id="f2c62-173">A seguir está um exemplo da resposta quando o cabeçalho de solicitação opcional `Prefer: return=representation` é usado.</span><span class="sxs-lookup"><span data-stu-id="f2c62-173">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="f2c62-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2c62-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
