# <a name="delete-open-extension"></a><span data-ttu-id="31281-101">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="31281-101">Delete open extension</span></span>

<span data-ttu-id="31281-102">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="31281-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="31281-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="31281-103">Permissions</span></span>

<span data-ttu-id="31281-p101">Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso do qual você está excluindo a extensão. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31281-p101">One of the following permissions is required to call this API, depending on the resource you're deleting the extension from. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31281-106">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="31281-106">**Supported resource**</span></span>|<span data-ttu-id="31281-107">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="31281-107">**Permission**</span></span>|<span data-ttu-id="31281-108">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="31281-108">**Supported resource**</span></span>|<span data-ttu-id="31281-109">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="31281-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="31281-110">dispositivo</span><span class="sxs-lookup"><span data-stu-id="31281-110">device</span></span>](../resources/device.md) | <span data-ttu-id="31281-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31281-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="31281-112">evento</span><span class="sxs-lookup"><span data-stu-id="31281-112">event</span></span>](../resources/event.md) | <span data-ttu-id="31281-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31281-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="31281-114">grupo</span><span class="sxs-lookup"><span data-stu-id="31281-114">group</span></span>](../resources/group.md) | <span data-ttu-id="31281-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31281-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="31281-116">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="31281-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="31281-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31281-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="31281-118">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="31281-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="31281-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31281-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="31281-120">mensagem</span><span class="sxs-lookup"><span data-stu-id="31281-120">message</span></span>](../resources/message.md) | <span data-ttu-id="31281-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31281-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="31281-122">organização</span><span class="sxs-lookup"><span data-stu-id="31281-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="31281-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31281-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="31281-124">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="31281-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="31281-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31281-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="31281-126">usuário</span><span class="sxs-lookup"><span data-stu-id="31281-126">user</span></span>](../resources/user.md) | <span data-ttu-id="31281-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31281-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="31281-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31281-128">HTTP request</span></span>
<span data-ttu-id="31281-129">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="31281-129">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="31281-p102">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="31281-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="31281-132">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="31281-132">Parameters</span></span>
|<span data-ttu-id="31281-133">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="31281-133">**Parameter**</span></span>|<span data-ttu-id="31281-134">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="31281-134">**Type**</span></span>|<span data-ttu-id="31281-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31281-135">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="31281-136">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="31281-136">_URL parameters_</span></span>|
|<span data-ttu-id="31281-137">id</span><span class="sxs-lookup"><span data-stu-id="31281-137">id</span></span>|<span data-ttu-id="31281-138">string</span><span class="sxs-lookup"><span data-stu-id="31281-138">string</span></span>|<span data-ttu-id="31281-p103">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31281-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="31281-141">extensionId</span><span class="sxs-lookup"><span data-stu-id="31281-141">extensionId</span></span>|<span data-ttu-id="31281-142">string</span><span class="sxs-lookup"><span data-stu-id="31281-142">string</span></span>|<span data-ttu-id="31281-p104">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31281-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="31281-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31281-146">Request headers</span></span>
| <span data-ttu-id="31281-147">Nome</span><span class="sxs-lookup"><span data-stu-id="31281-147">Name</span></span>       | <span data-ttu-id="31281-148">Valor</span><span class="sxs-lookup"><span data-stu-id="31281-148">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="31281-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="31281-149">Authorization</span></span> | <span data-ttu-id="31281-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31281-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31281-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31281-152">Request body</span></span>
<span data-ttu-id="31281-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31281-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31281-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="31281-154">Response</span></span>

<span data-ttu-id="31281-p106">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31281-p106">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31281-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31281-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31281-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31281-158">Request</span></span>
<span data-ttu-id="31281-159">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="31281-159">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="31281-160">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="31281-160">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="31281-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="31281-161">Response</span></span>
<span data-ttu-id="31281-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31281-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->