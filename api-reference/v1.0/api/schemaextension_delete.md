# <a name="delete-schemaextension"></a><span data-ttu-id="7e998-101">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="7e998-101">Delete schemaExtension</span></span>

<span data-ttu-id="7e998-102">Exclui uma definição da [extensão de esquema](../resources/schemaExtension.md).</span><span class="sxs-lookup"><span data-stu-id="7e998-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="7e998-p101">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="7e998-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="7e998-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e998-105">Permissions</span></span>
<span data-ttu-id="7e998-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e998-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7e998-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e998-108">Permission type</span></span>      | <span data-ttu-id="7e998-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e998-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e998-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e998-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e998-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e998-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e998-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e998-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e998-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e998-113">Not supported.</span></span>    |
|<span data-ttu-id="7e998-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e998-114">Application</span></span> | <span data-ttu-id="7e998-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e998-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e998-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e998-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e998-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e998-117">Request headers</span></span>
| <span data-ttu-id="7e998-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7e998-118">Name</span></span>      |<span data-ttu-id="7e998-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e998-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7e998-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e998-120">Authorization</span></span>  | <span data-ttu-id="7e998-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e998-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e998-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e998-123">Request body</span></span>
<span data-ttu-id="7e998-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e998-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e998-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e998-125">Response</span></span>

<span data-ttu-id="7e998-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e998-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e998-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e998-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e998-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e998-129">Request</span></span>
<span data-ttu-id="7e998-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e998-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="7e998-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e998-131">Response</span></span>
<span data-ttu-id="7e998-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e998-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="7e998-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="7e998-133">See also</span></span>

- [<span data-ttu-id="7e998-134">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7e998-134">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="7e998-135">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="7e998-135">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->