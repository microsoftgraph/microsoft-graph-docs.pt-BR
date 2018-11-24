# <a name="update-alert"></a><span data-ttu-id="aa6ca-101">Atualizar alertas</span><span class="sxs-lookup"><span data-stu-id="aa6ca-101">Update alert</span></span>

<span data-ttu-id="aa6ca-102">Atualize uma propriedade editável **alerta** dentro de qualquer solução integrada para manter o status de alerta e atribuições em sincronia nas soluções.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="aa6ca-103">Esse método atualiza qualquer solução que tem um registro de alerta referenciado ID.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa6ca-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="aa6ca-104">Permissions</span></span>

<span data-ttu-id="aa6ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa6ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa6ca-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa6ca-107">Permission type</span></span>      | <span data-ttu-id="aa6ca-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa6ca-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa6ca-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa6ca-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="aa6ca-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa6ca-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="aa6ca-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa6ca-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aa6ca-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-112">Not supported.</span></span>  |
|<span data-ttu-id="aa6ca-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa6ca-113">Application</span></span> | <span data-ttu-id="aa6ca-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa6ca-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa6ca-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa6ca-115">HTTP request</span></span>

> <span data-ttu-id="aa6ca-116">**Observação:** Você deve incluir o ID de **alerta** como um parâmetro e vendorInformation contendo o `provider` e `vendor` com este método.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="aa6ca-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6ca-117">Request headers</span></span>

| <span data-ttu-id="aa6ca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="aa6ca-118">Name</span></span>       | <span data-ttu-id="aa6ca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa6ca-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aa6ca-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa6ca-120">Authorization</span></span>  | <span data-ttu-id="aa6ca-p103">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="aa6ca-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="aa6ca-123">Prefer</span></span> | <span data-ttu-id="aa6ca-124">retornar = representação</span><span class="sxs-lookup"><span data-stu-id="aa6ca-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa6ca-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6ca-125">Request body</span></span>

<span data-ttu-id="aa6ca-126">No corpo da solicitação, fornece uma representação JSON dos valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="aa6ca-127">O corpo **deve** conter o `vendorInformation` propriedade com válido `provider` e `vendor` campos.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="aa6ca-128">A tabela a seguir lista os campos que podem ser atualizados para um alerta.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-128">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="aa6ca-129">Os valores para propriedades existentes que não estão incluídos no corpo da solicitação não serão alterado.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="aa6ca-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aa6ca-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa6ca-131">Property</span></span>   | <span data-ttu-id="aa6ca-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa6ca-132">Type</span></span> |<span data-ttu-id="aa6ca-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa6ca-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6ca-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="aa6ca-134">assignedTo</span></span>|<span data-ttu-id="aa6ca-135">String</span><span class="sxs-lookup"><span data-stu-id="aa6ca-135">String</span></span>|<span data-ttu-id="aa6ca-136">Nome do analista de alerta é atribuída a triagem, investigação ou correção.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="aa6ca-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa6ca-137">closedDateTime</span></span>|<span data-ttu-id="aa6ca-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa6ca-138">DateTimeOffset</span></span>|<span data-ttu-id="aa6ca-139">Hora em que o alerta foi fechado.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-139">Time at which the alert was closed.</span></span> <span data-ttu-id="aa6ca-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa6ca-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aa6ca-142">comentários</span><span class="sxs-lookup"><span data-stu-id="aa6ca-142">comments</span></span>|<span data-ttu-id="aa6ca-143">String collection</span><span class="sxs-lookup"><span data-stu-id="aa6ca-143">String collection</span></span>|<span data-ttu-id="aa6ca-144">Comentários de analistas no alerta (para gerenciamento de alerta do cliente).</span><span class="sxs-lookup"><span data-stu-id="aa6ca-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="aa6ca-145">comentários</span><span class="sxs-lookup"><span data-stu-id="aa6ca-145">feedback</span></span>|<span data-ttu-id="aa6ca-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="aa6ca-146">alertFeedback</span></span>|<span data-ttu-id="aa6ca-147">Comentários analista no alerta.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="aa6ca-148">Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="aa6ca-149">status</span><span class="sxs-lookup"><span data-stu-id="aa6ca-149">status</span></span>|<span data-ttu-id="aa6ca-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="aa6ca-150">alertStatus</span></span>|<span data-ttu-id="aa6ca-151">Status do ciclo de vida de alerta (estágio).</span><span class="sxs-lookup"><span data-stu-id="aa6ca-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="aa6ca-152">Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="aa6ca-153">marcas</span><span class="sxs-lookup"><span data-stu-id="aa6ca-153">tags</span></span>|<span data-ttu-id="aa6ca-154">String collection</span><span class="sxs-lookup"><span data-stu-id="aa6ca-154">String collection</span></span>|<span data-ttu-id="aa6ca-155">Rótulos podem ser definidos pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SERRA).</span><span class="sxs-lookup"><span data-stu-id="aa6ca-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="aa6ca-156">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="aa6ca-156">vendorInformation</span></span> |[<span data-ttu-id="aa6ca-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="aa6ca-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="aa6ca-158">Tipo complexo que contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="aa6ca-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="aa6ca-159">**Campos de provedor e fornecedor são necessários.**</span><span class="sxs-lookup"><span data-stu-id="aa6ca-159">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="aa6ca-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa6ca-160">Response</span></span>

<span data-ttu-id="aa6ca-161">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-161">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="aa6ca-162">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto atualizado [alerta](../resources/alert.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-162">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="aa6ca-163">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="aa6ca-163">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="aa6ca-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6ca-164">Request</span></span>

<span data-ttu-id="aa6ca-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-165">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa6ca-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa6ca-166">Response</span></span>

<span data-ttu-id="aa6ca-167">O exemplo a seguir é um exemplo de uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-167">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="aa6ca-168">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="aa6ca-168">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="aa6ca-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa6ca-169">Request</span></span>

<span data-ttu-id="aa6ca-170">O exemplo a seguir mostra uma solicitação que inclui o `Prefer` cabeçalho de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-170">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="aa6ca-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa6ca-171">Response</span></span>

<span data-ttu-id="aa6ca-172">A seguir está um exemplo da resposta quando o opcional `Prefer: return=representation` cabeçalho de solicitação é usado.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-172">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="aa6ca-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa6ca-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
