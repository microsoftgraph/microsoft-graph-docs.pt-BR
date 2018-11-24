# <a name="delete-open-extension"></a><span data-ttu-id="14970-101">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="14970-101">Delete open extension</span></span>

<span data-ttu-id="14970-102">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="14970-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="14970-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="14970-103">Permissions</span></span>

<span data-ttu-id="14970-104">Dependendo de permissão e o recurso que você está excluindo a extensão do tipo (delegado ou aplicativo) solicitada, a permissão especificada na tabela a seguir é menos privilegiada necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="14970-104">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="14970-105">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="14970-105">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="14970-106">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="14970-106">Supported resource</span></span> | <span data-ttu-id="14970-107">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14970-107">Delegated (work or school account)</span></span> | <span data-ttu-id="14970-108">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14970-108">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14970-109">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14970-109">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="14970-110">dispositivo</span><span class="sxs-lookup"><span data-stu-id="14970-110">device</span></span>](../resources/device.md) | <span data-ttu-id="14970-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14970-111">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="14970-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-112">Not supported</span></span> | <span data-ttu-id="14970-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-113">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="14970-114">evento</span><span class="sxs-lookup"><span data-stu-id="14970-114">event</span></span>](../resources/event.md) | <span data-ttu-id="14970-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="14970-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="14970-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-117">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="14970-118">grupo</span><span class="sxs-lookup"><span data-stu-id="14970-118">group</span></span>](../resources/group.md) | <span data-ttu-id="14970-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="14970-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-120">Not supported</span></span> | <span data-ttu-id="14970-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-121">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="14970-122">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="14970-122">group event</span></span>](../resources/event.md) | <span data-ttu-id="14970-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="14970-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-124">Not supported</span></span> | <span data-ttu-id="14970-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-125">Not supported</span></span> |
| [<span data-ttu-id="14970-126">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="14970-126">group post</span></span>](../resources/post.md) | <span data-ttu-id="14970-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="14970-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-128">Not supported</span></span> | <span data-ttu-id="14970-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-129">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="14970-130">mensagem</span><span class="sxs-lookup"><span data-stu-id="14970-130">message</span></span>](../resources/message.md) | <span data-ttu-id="14970-131">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-131">Mail.ReadWrite</span></span> | <span data-ttu-id="14970-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-132">Mail.ReadWrite</span></span> | <span data-ttu-id="14970-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-133">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="14970-134">organização</span><span class="sxs-lookup"><span data-stu-id="14970-134">organization</span></span>](../resources/organization.md) | <span data-ttu-id="14970-135">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14970-135">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="14970-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-136">Not supported</span></span> | <span data-ttu-id="14970-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="14970-137">Not supported</span></span> |
| [<span data-ttu-id="14970-138">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="14970-138">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="14970-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-139">Contacts.ReadWrite</span></span> | <span data-ttu-id="14970-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="14970-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-141">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="14970-142">usuário</span><span class="sxs-lookup"><span data-stu-id="14970-142">user</span></span>](../resources/user.md) | <span data-ttu-id="14970-143">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-143">User.ReadWrite.All</span></span> | <span data-ttu-id="14970-144">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14970-144">User.ReadWrite</span></span> | <span data-ttu-id="14970-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14970-145">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14970-146">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14970-146">HTTP request</span></span>
<span data-ttu-id="14970-147">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="14970-147">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="14970-p102">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="14970-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="14970-150">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="14970-150">Path parameters</span></span>
|<span data-ttu-id="14970-151">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="14970-151">Parameter</span></span>|<span data-ttu-id="14970-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="14970-152">Type</span></span>|<span data-ttu-id="14970-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="14970-153">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="14970-154">id</span><span class="sxs-lookup"><span data-stu-id="14970-154">id</span></span>|<span data-ttu-id="14970-155">string</span><span class="sxs-lookup"><span data-stu-id="14970-155">string</span></span>|<span data-ttu-id="14970-p103">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14970-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="14970-158">extensionId</span><span class="sxs-lookup"><span data-stu-id="14970-158">extensionId</span></span>|<span data-ttu-id="14970-159">string</span><span class="sxs-lookup"><span data-stu-id="14970-159">string</span></span>|<span data-ttu-id="14970-p104">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14970-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="14970-163">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14970-163">Request headers</span></span>
| <span data-ttu-id="14970-164">Nome</span><span class="sxs-lookup"><span data-stu-id="14970-164">Name</span></span>       | <span data-ttu-id="14970-165">Valor</span><span class="sxs-lookup"><span data-stu-id="14970-165">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="14970-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="14970-166">Authorization</span></span> | <span data-ttu-id="14970-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14970-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14970-169">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14970-169">Request body</span></span>
<span data-ttu-id="14970-170">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14970-170">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14970-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="14970-171">Response</span></span>

<span data-ttu-id="14970-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14970-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14970-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14970-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14970-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14970-175">Request</span></span>
<span data-ttu-id="14970-176">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="14970-176">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="14970-177">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="14970-177">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="14970-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="14970-178">Response</span></span>
<span data-ttu-id="14970-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14970-179">Here is an example of the response.</span></span>
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