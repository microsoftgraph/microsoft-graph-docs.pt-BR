# <a name="create-rule"></a><span data-ttu-id="b5484-101">Criar regra</span><span class="sxs-lookup"><span data-stu-id="b5484-101">Create rule</span></span>


<span data-ttu-id="b5484-102">Crie um objeto [messageRule](../resources/messagerule.md) especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="b5484-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="b5484-103">O Outlook realizará essas ações se uma mensagem recebida na Caixa de Entrada do usuário atender às condições especificadas.</span><span class="sxs-lookup"><span data-stu-id="b5484-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5484-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5484-104">Permissions</span></span>
<span data-ttu-id="b5484-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5484-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5484-107">Permission type</span></span>      | <span data-ttu-id="b5484-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5484-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5484-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5484-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b5484-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5484-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b5484-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5484-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5484-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5484-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b5484-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5484-113">Application</span></span> | <span data-ttu-id="b5484-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5484-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="b5484-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5484-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="b5484-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5484-116">Request headers</span></span>
| <span data-ttu-id="b5484-117">Nome</span><span class="sxs-lookup"><span data-stu-id="b5484-117">Name</span></span>       | <span data-ttu-id="b5484-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5484-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5484-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5484-119">Authorization</span></span>  | <span data-ttu-id="b5484-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5484-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b5484-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5484-122">Request body</span></span>
<span data-ttu-id="b5484-123">No corpo da solicitação, forneça os parâmetros que são aplicáveis à sua regra.</span><span class="sxs-lookup"><span data-stu-id="b5484-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="b5484-124">A seguir estão os parâmetros de corpo que normalmente são usados ao criar regras.</span><span class="sxs-lookup"><span data-stu-id="b5484-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="b5484-125">É possível especificar outras propriedades **messageRule** graváveis conforme apropriado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5484-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

### <a name="request-parameters"></a><span data-ttu-id="b5484-126">Parâmetros da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5484-126">Request parameters</span></span>
| <span data-ttu-id="b5484-127">Nome</span><span class="sxs-lookup"><span data-stu-id="b5484-127">Name</span></span>       | <span data-ttu-id="b5484-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5484-128">Type</span></span>|<span data-ttu-id="b5484-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5484-129">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="b5484-130">actions</span><span class="sxs-lookup"><span data-stu-id="b5484-130">Actions</span></span>|[<span data-ttu-id="b5484-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="b5484-131">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="b5484-132">Ações a serem realizadas em uma mensagem quando as condições correspondentes, se houver, forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="b5484-132">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="b5484-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5484-133">Required.</span></span>|
|<span data-ttu-id="b5484-134">conditions</span><span class="sxs-lookup"><span data-stu-id="b5484-134">Conditions</span></span>|[<span data-ttu-id="b5484-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b5484-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="b5484-136">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="b5484-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="b5484-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b5484-137">Optional.</span></span>|
|<span data-ttu-id="b5484-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b5484-138">displayName</span></span>| <span data-ttu-id="b5484-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5484-139">String</span></span>  | <span data-ttu-id="b5484-140">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="b5484-140">The name of the new formatting rule.</span></span> <span data-ttu-id="b5484-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5484-141">Required.</span></span>|
|<span data-ttu-id="b5484-142">exceptions</span><span class="sxs-lookup"><span data-stu-id="b5484-142">exceptions</span></span>| [<span data-ttu-id="b5484-143">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b5484-143">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="b5484-144">Representa condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="b5484-144">Represents exception conditions for the rule.</span></span> <span data-ttu-id="b5484-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b5484-145">Optional.</span></span> |
|<span data-ttu-id="b5484-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b5484-146">isEnabled</span></span> | <span data-ttu-id="b5484-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5484-147">Boolean</span></span> | <span data-ttu-id="b5484-148">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="b5484-148">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="b5484-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b5484-149">Optional.</span></span> |
|<span data-ttu-id="b5484-150">sequence</span><span class="sxs-lookup"><span data-stu-id="b5484-150">Sequence</span></span>| <span data-ttu-id="b5484-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b5484-151">Int32</span></span> | <span data-ttu-id="b5484-152">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="b5484-152">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="b5484-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5484-153">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b5484-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5484-154">Response</span></span>
<span data-ttu-id="b5484-155">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto **messageRule** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5484-155">If successful, this method returns a `201 Created` response code and a **deviceEnrollmentWindowsHelloForBusinessConfiguration** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5484-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5484-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5484-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5484-157">Request</span></span>
<span data-ttu-id="b5484-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5484-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messagerules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
##### <a name="response"></a><span data-ttu-id="b5484-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5484-159">Response</span></span>
<span data-ttu-id="b5484-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5484-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
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
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->