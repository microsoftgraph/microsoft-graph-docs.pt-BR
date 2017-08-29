# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="184f4-101">Atualizar inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="184f4-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="184f4-102">Altere o campo **classifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="184f4-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="184f4-103">Você não pode usar PATCH para alterar outros campos em uma instância de [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md).</span><span class="sxs-lookup"><span data-stu-id="184f4-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="184f4-104">Se houver uma substituição de um remetente e o remetente alterar seu nome de exibição, você poderá usar [POST](inferenceclassification_post_overrides.md) para forçar uma atualização para o campo de nome em uma substituição existente.</span><span class="sxs-lookup"><span data-stu-id="184f4-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="184f4-105">Se houver uma substituição de um remetente e o remetente alterar seu endereço SMTP, [excluir](inferenceclassificationoverride_delete.md) a substituição existente e [criar](inferenceclassification_post_overrides.md) uma nova com o novo endereço SMTP será a única maneira de "atualizar" a substituição deste remetente.</span><span class="sxs-lookup"><span data-stu-id="184f4-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="184f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="184f4-106">Permissions</span></span>
<span data-ttu-id="184f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="184f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="184f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="184f4-109">Permission type</span></span>      | <span data-ttu-id="184f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="184f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="184f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="184f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="184f4-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="184f4-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="184f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="184f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="184f4-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="184f4-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="184f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="184f4-115">Application</span></span> | <span data-ttu-id="184f4-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="184f4-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="184f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="184f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="184f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="184f4-118">Request headers</span></span>
| <span data-ttu-id="184f4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="184f4-119">Name</span></span>       | <span data-ttu-id="184f4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="184f4-120">Type</span></span> | <span data-ttu-id="184f4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="184f4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="184f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="184f4-122">Authorization</span></span>  | <span data-ttu-id="184f4-123">string</span><span class="sxs-lookup"><span data-stu-id="184f4-123">string</span></span>  | <span data-ttu-id="184f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="184f4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="184f4-126">Content-Type</span></span> | <span data-ttu-id="184f4-127">string</span><span class="sxs-lookup"><span data-stu-id="184f4-127">string</span></span>  | <span data-ttu-id="184f4-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184f4-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="184f4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="184f4-130">Request body</span></span>
<span data-ttu-id="184f4-p104">No corpo da solicitação, forneça o novo valor para **classifyAs**. Para obter o melhor desempenho, não inclua valores existentes que não estão sendo alterados.</span><span class="sxs-lookup"><span data-stu-id="184f4-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="184f4-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="184f4-133">Property</span></span>     | <span data-ttu-id="184f4-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="184f4-134">Type</span></span>   |<span data-ttu-id="184f4-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="184f4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="184f4-136">classifyAs</span><span class="sxs-lookup"><span data-stu-id="184f4-136">classifyAs</span></span>|<span data-ttu-id="184f4-137">string</span><span class="sxs-lookup"><span data-stu-id="184f4-137">string</span></span>| <span data-ttu-id="184f4-p105">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="184f4-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="184f4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="184f4-140">Response</span></span>

<span data-ttu-id="184f4-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="184f4-141">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="184f4-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="184f4-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="184f4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="184f4-143">Request</span></span>
<span data-ttu-id="184f4-144">O exemplo a seguir altera a substituição para o endereço SMTP randiw@adatum.onmicrosoft.com de `other` para `focused`.</span><span class="sxs-lookup"><span data-stu-id="184f4-144">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="184f4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="184f4-145">Response</span></span>
<span data-ttu-id="184f4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="184f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->