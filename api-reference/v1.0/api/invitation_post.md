# <a name="create-invitation"></a><span data-ttu-id="228e0-101">Criar convite</span><span class="sxs-lookup"><span data-stu-id="228e0-101">Create invitation</span></span>

<span data-ttu-id="228e0-p101">Use essa API para criar um novo [convite](../resources/invitation.md). O convite adiciona um usuário externo à organização.</span><span class="sxs-lookup"><span data-stu-id="228e0-p101">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="228e0-104">Ao criar um novo convite, você tem várias opções disponíveis:</span><span class="sxs-lookup"><span data-stu-id="228e0-104">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="228e0-p102">À criação do convite, o Microsoft Graph pode enviar automaticamente um email de convite diretamente ao usuário convidado, ou seu aplicativo pode usar o *inviteRedeemUrl* retornado na resposta da criação para articular o seu próprio convite (por meio de seu mecanismo de comunicação de preferência) para o usuário convidado. Se você decidir fazer com que o Microsoft Graph envie um email de convite automaticamente, poderá controlar o conteúdo e o idioma do email usando [ *invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span><span class="sxs-lookup"><span data-stu-id="228e0-p102">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="228e0-p103">Quando o usuário é convidado, uma entidade de usuário (do userType Convidado) é criada e, agora, pode ser usada para o controle do acesso aos recursos. O usuário convidado precisa passar pelo processo de resgate para acessar os recursos para os quais ele foi convidado.</span><span class="sxs-lookup"><span data-stu-id="228e0-p103">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="228e0-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="228e0-109">Prerequisites</span></span>
<span data-ttu-id="228e0-110">Um dos seguintes escopos é necessário para a execução desta API: *User.Invite.All* ou *User.ReadWrite.All*  ou *Directory.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="228e0-110">One of the following scopes is required to execute this API: *User.Invite.All* or *User.ReadWrite.All*  or *Directory.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="228e0-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="228e0-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="228e0-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="228e0-112">Request headers</span></span>
| <span data-ttu-id="228e0-113">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="228e0-113">Header</span></span>       | <span data-ttu-id="228e0-114">Valor</span><span class="sxs-lookup"><span data-stu-id="228e0-114">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="228e0-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="228e0-115">Authorization</span></span>  | <span data-ttu-id="228e0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="228e0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="228e0-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="228e0-118">Content-Type</span></span>  | <span data-ttu-id="228e0-119">application/json</span><span class="sxs-lookup"><span data-stu-id="228e0-119">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="228e0-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="228e0-120">Request body</span></span>
<span data-ttu-id="228e0-121">No corpo da solicitação, forneça uma representação JSON do objeto [invitation](../resources/invitation.md).</span><span class="sxs-lookup"><span data-stu-id="228e0-121">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="228e0-122">A tabela a seguir mostra as propriedades que são necessárias ao criar um convite.</span><span class="sxs-lookup"><span data-stu-id="228e0-122">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="228e0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="228e0-123">Parameter</span></span> | <span data-ttu-id="228e0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="228e0-124">Type</span></span> | <span data-ttu-id="228e0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="228e0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="228e0-126">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="228e0-126">invitedUserEmailAddress</span></span> |<span data-ttu-id="228e0-127">string</span><span class="sxs-lookup"><span data-stu-id="228e0-127">string</span></span> | <span data-ttu-id="228e0-128">O endereço de email do usuário que você está convidando.</span><span class="sxs-lookup"><span data-stu-id="228e0-128">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="228e0-129">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="228e0-129">inviteRedirectUrl</span></span> |<span data-ttu-id="228e0-130">string</span><span class="sxs-lookup"><span data-stu-id="228e0-130">string</span></span> |<span data-ttu-id="228e0-131">A URL para a qual o usuário será redirecionado após o resgate.</span><span class="sxs-lookup"><span data-stu-id="228e0-131">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="228e0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="228e0-132">Response</span></span>

<span data-ttu-id="228e0-133">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [invitation](../resources/invitation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="228e0-133">If successful, this method returns `201, Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="228e0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="228e0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="228e0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="228e0-135">Request</span></span>
<span data-ttu-id="228e0-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="228e0-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a><span data-ttu-id="228e0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="228e0-137">Response</span></span>
<span data-ttu-id="228e0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="228e0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitations"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```
