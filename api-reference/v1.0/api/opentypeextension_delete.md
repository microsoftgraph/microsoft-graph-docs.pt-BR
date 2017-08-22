# <a name="delete-open-extension"></a><span data-ttu-id="5fa5f-101">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="5fa5f-101">Delete open extension</span></span>

<span data-ttu-id="5fa5f-102">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="5fa5f-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5fa5f-103">Prerequisites</span></span>

<span data-ttu-id="5fa5f-104">Um dos seguintes valores de **permissões** é necessário para executar essa API, dependendo do recurso do qual você está excluindo a extensão:</span><span class="sxs-lookup"><span data-stu-id="5fa5f-104">One of the following **permissions** is required to execute this API, depending on the resource you're deleting the extension from:</span></span>

|<span data-ttu-id="5fa5f-105">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-105">**Supported resource**</span></span>|<span data-ttu-id="5fa5f-106">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-106">**Permission**</span></span>|<span data-ttu-id="5fa5f-107">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-107">**Supported resource**</span></span>|<span data-ttu-id="5fa5f-108">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-108">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="5fa5f-109">device</span><span class="sxs-lookup"><span data-stu-id="5fa5f-109">device</span></span>](../resources/device.md) | <span data-ttu-id="5fa5f-110">_Device.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-110">_Device.ReadWrite.All_</span></span> | [<span data-ttu-id="5fa5f-111">event</span><span class="sxs-lookup"><span data-stu-id="5fa5f-111">event</span></span>](../resources/event.md) | <span data-ttu-id="5fa5f-112">_Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-112">_Calendars.ReadWrite_</span></span> |
| [<span data-ttu-id="5fa5f-113">group</span><span class="sxs-lookup"><span data-stu-id="5fa5f-113">group</span></span>](../resources/group.md) | <span data-ttu-id="5fa5f-114">_Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-114">_Group.ReadWrite.All_</span></span> | [<span data-ttu-id="5fa5f-115">group event</span><span class="sxs-lookup"><span data-stu-id="5fa5f-115">Group event</span></span>](../resources/event.md) | <span data-ttu-id="5fa5f-116">_Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-116">_Group.ReadWrite.All_</span></span> |
| [<span data-ttu-id="5fa5f-117">group post</span><span class="sxs-lookup"><span data-stu-id="5fa5f-117">Group post</span></span>](../resources/post.md) | <span data-ttu-id="5fa5f-118">_Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-118">_Group.ReadWrite.All_</span></span> | [<span data-ttu-id="5fa5f-119">mensagem</span><span class="sxs-lookup"><span data-stu-id="5fa5f-119">message</span></span>](../resources/message.md) | <span data-ttu-id="5fa5f-120">_Mail.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-120">_Mail.ReadWrite_</span></span> |
| [<span data-ttu-id="5fa5f-121">organization</span><span class="sxs-lookup"><span data-stu-id="5fa5f-121">organization</span></span>](../resources/organization.md) | <span data-ttu-id="5fa5f-122">_Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-122">_Directory.AccessAsUser.All_</span></span> | [<span data-ttu-id="5fa5f-123">personal contact</span><span class="sxs-lookup"><span data-stu-id="5fa5f-123">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="5fa5f-124">_Contacts.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-124">_Contacts.ReadWrite_</span></span> |
| [<span data-ttu-id="5fa5f-125">user</span><span class="sxs-lookup"><span data-stu-id="5fa5f-125">user</span></span>](../resources/user.md) | <span data-ttu-id="5fa5f-126">_Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-126">_Directory.AccessAsUser.All_</span></span> | | |

 
## <a name="http-request"></a><span data-ttu-id="5fa5f-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fa5f-127">HTTP request</span></span>
<span data-ttu-id="5fa5f-128">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-128">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="5fa5f-p101">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-p101">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="5fa5f-131">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="5fa5f-131">Parameters</span></span>
|<span data-ttu-id="5fa5f-132">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-132">**Parameter**</span></span>|<span data-ttu-id="5fa5f-133">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-133">**Type**</span></span>|<span data-ttu-id="5fa5f-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5fa5f-134">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5fa5f-135">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="5fa5f-135">_URL parameters_</span></span>|
|<span data-ttu-id="5fa5f-136">id</span><span class="sxs-lookup"><span data-stu-id="5fa5f-136">id</span></span>|<span data-ttu-id="5fa5f-137">string</span><span class="sxs-lookup"><span data-stu-id="5fa5f-137">string</span></span>|<span data-ttu-id="5fa5f-p102">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-p102">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="5fa5f-140">extensionId</span><span class="sxs-lookup"><span data-stu-id="5fa5f-140">extensionId</span></span>|<span data-ttu-id="5fa5f-141">string</span><span class="sxs-lookup"><span data-stu-id="5fa5f-141">string</span></span>|<span data-ttu-id="5fa5f-p103">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-p103">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="5fa5f-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fa5f-145">Request headers</span></span>
| <span data-ttu-id="5fa5f-146">Nome</span><span class="sxs-lookup"><span data-stu-id="5fa5f-146">Name</span></span>       | <span data-ttu-id="5fa5f-147">Valor</span><span class="sxs-lookup"><span data-stu-id="5fa5f-147">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5fa5f-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fa5f-148">Authorization</span></span> | <span data-ttu-id="5fa5f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5fa5f-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fa5f-151">Request body</span></span>
<span data-ttu-id="5fa5f-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fa5f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fa5f-153">Response</span></span>

<span data-ttu-id="5fa5f-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-p105">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fa5f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fa5f-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fa5f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fa5f-157">Request</span></span>
<span data-ttu-id="5fa5f-158">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-158">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="5fa5f-159">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-159">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="5fa5f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fa5f-160">Response</span></span>
<span data-ttu-id="5fa5f-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fa5f-161">Here is an example of the response.</span></span>
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