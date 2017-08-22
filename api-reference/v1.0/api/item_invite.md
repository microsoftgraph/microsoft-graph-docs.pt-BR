# <a name="send-a-sharing-invitation"></a><span data-ttu-id="27d06-101">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="27d06-101">Send a sharing invitation</span></span>

<span data-ttu-id="27d06-p101">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="27d06-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27d06-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27d06-104">Prerequisites</span></span>
<span data-ttu-id="27d06-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="27d06-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="27d06-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27d06-106">Files.ReadWrite</span></span>
* <span data-ttu-id="27d06-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d06-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="27d06-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d06-108">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="27d06-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27d06-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a><span data-ttu-id="27d06-110">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27d06-110">Request body</span></span>
<span data-ttu-id="27d06-111">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d06-111">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27d06-112">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27d06-112">Parameter</span></span>        | <span data-ttu-id="27d06-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="27d06-113">Type</span></span>                                            | <span data-ttu-id="27d06-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="27d06-114">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="27d06-115">destinatários</span><span class="sxs-lookup"><span data-stu-id="27d06-115">recipients</span></span>       | <span data-ttu-id="27d06-116">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="27d06-116">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="27d06-117">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="27d06-117">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="27d06-118">mensagem</span><span class="sxs-lookup"><span data-stu-id="27d06-118">message</span></span>          | <span data-ttu-id="27d06-119">String</span><span class="sxs-lookup"><span data-stu-id="27d06-119">String</span></span>                                          | <span data-ttu-id="27d06-p102">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="27d06-p102">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="27d06-122">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="27d06-122">requireSignIn</span></span>    | <span data-ttu-id="27d06-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="27d06-123">Boolean</span></span>                                         | <span data-ttu-id="27d06-124">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="27d06-124">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="27d06-125">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="27d06-125">sendInvitation</span></span>   | <span data-ttu-id="27d06-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="27d06-126">Boolean</span></span>                                         | <span data-ttu-id="27d06-127">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="27d06-127">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="27d06-128">funções</span><span class="sxs-lookup"><span data-stu-id="27d06-128">roles</span></span>            | <span data-ttu-id="27d06-129">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="27d06-129">Collection(String)</span></span>                              | <span data-ttu-id="27d06-130">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="27d06-130">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="27d06-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d06-131">Response</span></span>

<span data-ttu-id="27d06-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d06-132">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27d06-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27d06-133">Example</span></span>
<span data-ttu-id="27d06-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="27d06-134">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="27d06-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27d06-135">Request</span></span>
<span data-ttu-id="27d06-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d06-136">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="27d06-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d06-137">Response</span></span>
<span data-ttu-id="27d06-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d06-138">Here is an example of the response.</span></span>
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

## <a name="remarks"></a><span data-ttu-id="27d06-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="27d06-139">Remarks</span></span>

* <span data-ttu-id="27d06-140">[Drives](../resources/drive.md) com **driveType** `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="27d06-140">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="27d06-141">Para obter uma lista das funções disponíveis, confira [Funções de enumeração](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="27d06-141">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
