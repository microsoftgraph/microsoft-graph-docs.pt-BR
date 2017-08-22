# <a name="delete-schemaextension"></a><span data-ttu-id="1da26-101">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="1da26-101">Delete schemaExtension</span></span>

<span data-ttu-id="1da26-102">Exclui uma definição da [extensão de esquema](../resources/schemaExtension.md).</span><span class="sxs-lookup"><span data-stu-id="1da26-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="1da26-p101">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="1da26-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="1da26-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1da26-105">Prerequisites</span></span>
<span data-ttu-id="1da26-106">O seguinte **escopo** é obrigatório para executar esta API: *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="1da26-106">The following **scope** is required to execute this API: *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="1da26-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1da26-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1da26-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1da26-108">Request headers</span></span>
| <span data-ttu-id="1da26-109">Nome</span><span class="sxs-lookup"><span data-stu-id="1da26-109">Name</span></span>      |<span data-ttu-id="1da26-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1da26-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1da26-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="1da26-111">Authorization</span></span>  | <span data-ttu-id="1da26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1da26-p102">Bearer {token}. Required.</span></span> |
 

## <a name="request-body"></a><span data-ttu-id="1da26-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1da26-114">Request body</span></span>
<span data-ttu-id="1da26-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1da26-115">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1da26-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="1da26-116">Response</span></span>

<span data-ttu-id="1da26-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1da26-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1da26-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1da26-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1da26-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1da26-120">Request</span></span>
<span data-ttu-id="1da26-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1da26-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="1da26-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1da26-122">Response</span></span>
<span data-ttu-id="1da26-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1da26-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="1da26-124">Veja também</span><span class="sxs-lookup"><span data-stu-id="1da26-124">See also</span></span>

- [<span data-ttu-id="1da26-125">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1da26-125">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="1da26-126">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="1da26-126">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->