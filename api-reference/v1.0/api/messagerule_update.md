# <a name="update-rule"></a><span data-ttu-id="de0fb-101">Atualizar regra</span><span class="sxs-lookup"><span data-stu-id="de0fb-101">Update rule</span></span>


<span data-ttu-id="de0fb-102">Altere as propriedades graváveis em um objeto [messageRule](../resources/messagerule.md) e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="de0fb-102">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="de0fb-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="de0fb-103">Permissions</span></span>
<span data-ttu-id="de0fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="de0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="de0fb-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de0fb-106">Permission type</span></span>      | <span data-ttu-id="de0fb-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de0fb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de0fb-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de0fb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="de0fb-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de0fb-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="de0fb-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de0fb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de0fb-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de0fb-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="de0fb-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de0fb-112">Application</span></span> | <span data-ttu-id="de0fb-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de0fb-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="de0fb-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de0fb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="de0fb-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="de0fb-115">Optional request headers</span></span>
| <span data-ttu-id="de0fb-116">Nome</span><span class="sxs-lookup"><span data-stu-id="de0fb-116">Name</span></span>       | <span data-ttu-id="de0fb-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="de0fb-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="de0fb-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="de0fb-118">Authorization</span></span>  | <span data-ttu-id="de0fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de0fb-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="de0fb-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de0fb-121">Request body</span></span>
<span data-ttu-id="de0fb-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="de0fb-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de0fb-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de0fb-125">Property</span></span>     | <span data-ttu-id="de0fb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="de0fb-126">Type</span></span>   |<span data-ttu-id="de0fb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="de0fb-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="de0fb-128">actions</span><span class="sxs-lookup"><span data-stu-id="de0fb-128">Actions</span></span> | [<span data-ttu-id="de0fb-129">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="de0fb-129">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="de0fb-130">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="de0fb-130">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="de0fb-131">conditions</span><span class="sxs-lookup"><span data-stu-id="de0fb-131">Conditions</span></span> | [<span data-ttu-id="de0fb-132">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="de0fb-132">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="de0fb-133">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="de0fb-133">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="de0fb-134">displayName</span><span class="sxs-lookup"><span data-stu-id="de0fb-134">displayName</span></span> | <span data-ttu-id="de0fb-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de0fb-135">String</span></span> | <span data-ttu-id="de0fb-136">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="de0fb-136">The name of the new formatting rule.</span></span> |
| <span data-ttu-id="de0fb-137">exceptions</span><span class="sxs-lookup"><span data-stu-id="de0fb-137">exceptions</span></span> | [<span data-ttu-id="de0fb-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="de0fb-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="de0fb-139">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="de0fb-139">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="de0fb-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="de0fb-140">isEnabled</span></span> | <span data-ttu-id="de0fb-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0fb-141">Boolean</span></span> | <span data-ttu-id="de0fb-142">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="de0fb-142">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="de0fb-143">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="de0fb-143">isReadOnly</span></span> | <span data-ttu-id="de0fb-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="de0fb-144">Boolean</span></span> | <span data-ttu-id="de0fb-145">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="de0fb-145">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="de0fb-146">sequence</span><span class="sxs-lookup"><span data-stu-id="de0fb-146">Sequence</span></span> | <span data-ttu-id="de0fb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="de0fb-147">Int32</span></span> | <span data-ttu-id="de0fb-148">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="de0fb-148">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="de0fb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="de0fb-149">Response</span></span>
<span data-ttu-id="de0fb-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [messageRule](../resources/messagerule.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de0fb-150">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de0fb-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de0fb-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de0fb-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de0fb-152">Request</span></span>
<span data-ttu-id="de0fb-153">O exemplo a seguir muda o nome da regra e as ações a serem seguidas para essa regra no [exemplo](messagerule_get.md#example) em [Obter regra](messagerule_get.md), do encaminhamento para um endereço a marcar sua importância como alta.</span><span class="sxs-lookup"><span data-stu-id="de0fb-153">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule_get.md#example) in [Get rule](messagerule_get.md), from forwarding to an address to marking its importance as high.</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')

Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
##### <a name="response"></a><span data-ttu-id="de0fb-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="de0fb-154">Response</span></span>
<span data-ttu-id="de0fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de0fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->