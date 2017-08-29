# <a name="send-a-sharing-invitation"></a><span data-ttu-id="2e8ae-101">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="2e8ae-101">Send a sharing invitation</span></span>

<span data-ttu-id="2e8ae-p101">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e8ae-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e8ae-104">Permissions</span></span>
<span data-ttu-id="2e8ae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e8ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e8ae-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e8ae-107">Permission type</span></span>      | <span data-ttu-id="2e8ae-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e8ae-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e8ae-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e8ae-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2e8ae-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8ae-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e8ae-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e8ae-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e8ae-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8ae-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e8ae-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e8ae-113">Application</span></span> | <span data-ttu-id="2e8ae-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8ae-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e8ae-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e8ae-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a><span data-ttu-id="2e8ae-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e8ae-116">Request body</span></span>
<span data-ttu-id="2e8ae-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e8ae-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2e8ae-118">Parameter</span></span>        | <span data-ttu-id="2e8ae-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e8ae-119">Type</span></span>                                            | <span data-ttu-id="2e8ae-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e8ae-120">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2e8ae-121">destinatários</span><span class="sxs-lookup"><span data-stu-id="2e8ae-121">recipients</span></span>       | <span data-ttu-id="2e8ae-122">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="2e8ae-122">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="2e8ae-123">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-123">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="2e8ae-124">mensagem</span><span class="sxs-lookup"><span data-stu-id="2e8ae-124">message</span></span>          | <span data-ttu-id="2e8ae-125">String</span><span class="sxs-lookup"><span data-stu-id="2e8ae-125">String</span></span>                                          | <span data-ttu-id="2e8ae-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="2e8ae-128">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="2e8ae-128">requireSignIn</span></span>    | <span data-ttu-id="2e8ae-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e8ae-129">Boolean</span></span>                                         | <span data-ttu-id="2e8ae-130">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-130">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="2e8ae-131">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="2e8ae-131">sendInvitation</span></span>   | <span data-ttu-id="2e8ae-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e8ae-132">Boolean</span></span>                                         | <span data-ttu-id="2e8ae-133">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="2e8ae-133">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="2e8ae-134">funções</span><span class="sxs-lookup"><span data-stu-id="2e8ae-134">roles</span></span>            | <span data-ttu-id="2e8ae-135">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="2e8ae-135">Collection(String)</span></span>                              | <span data-ttu-id="2e8ae-136">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-136">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="2e8ae-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e8ae-137">Response</span></span>

<span data-ttu-id="2e8ae-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-138">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e8ae-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e8ae-139">Example</span></span>
<span data-ttu-id="2e8ae-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2e8ae-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e8ae-141">Request</span></span>
<span data-ttu-id="2e8ae-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a><span data-ttu-id="2e8ae-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e8ae-143">Response</span></span>
<span data-ttu-id="2e8ae-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="2e8ae-145">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e8ae-145">Remarks</span></span>

* <span data-ttu-id="2e8ae-146">[Drives](../resources/drive.md) com **driveType** `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="2e8ae-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="2e8ae-147">Para obter uma lista das funções disponíveis, confira [Funções de enumeração](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="2e8ae-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
