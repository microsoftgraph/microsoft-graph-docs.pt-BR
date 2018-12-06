---
title: Criar e enviar mensagens do Outlook
description: Emails são representados pelo recurso de mensagem no Microsoft Graph.
ms.openlocfilehash: 49670df0d5d735e412a0fd97e3404fab044f6f50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091658"
---
# <a name="create-and-send-outlook-messages"></a><span data-ttu-id="1179d-103">Criar e enviar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="1179d-103">Create and send Outlook messages</span></span>

<span data-ttu-id="1179d-104">Emails são representados pelo recurso de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1179d-104">Emails are represented by the [message](/graph/api/resources/message?view=graph-rest-1.0) resource in Microsoft Graph.</span></span>

<span data-ttu-id="1179d-105">Por padrão, as mensagens são identificadas por uma ID de entrada exclusiva na propriedade **id**.</span><span class="sxs-lookup"><span data-stu-id="1179d-105">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="1179d-106">Um provedor de armazenamento atribui uma ID de entrada a uma mensagem quando a mensagem é salva incialmente como um rascunho ou enviada.</span><span class="sxs-lookup"><span data-stu-id="1179d-106">A store provider assigns a message an entry ID when the message is initially saved as a draft or sent.</span></span> <span data-ttu-id="1179d-107">Essa ID muda quando a mensagem é copiada ou movida para outra pasta, armazenada ou um arquivo .PST.</span><span class="sxs-lookup"><span data-stu-id="1179d-107">That ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="1179d-108">Criar e enviar mensagens</span><span class="sxs-lookup"><span data-stu-id="1179d-108">Creating and sending mail</span></span>

<span data-ttu-id="1179d-109">No Outlook, você pode criar e enviar um email na mesma ação [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) ou pode [criar](/graph/api/user-post-messages?view=graph-rest-1.0) um rascunho, posteriormente [adicionar conteúdo](/graph/api/message-update?view=graph-rest-1.0) e [enviar](/graph/api/message-send?view=graph-rest-1.0) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="1179d-109">In Outlook, you can create and send an email in the same [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) action, or you can [create](/graph/api/user-post-messages?view=graph-rest-1.0) a draft, subsequently [add content](/graph/api/message-update?view=graph-rest-1.0) and [send](/graph/api/message-send?view=graph-rest-1.0) the draft.</span></span>

<span data-ttu-id="1179d-110">Da mesma forma, quando responder a um email, você pode criar e enviar a resposta da mesma ação ([responder](/graph/api/message-reply?view=graph-rest-1.0), [responder a todos](/graph/api/message-replyall?view=graph-rest-1.0) ou [encaminhar](/graph/api/message-forward?view=graph-rest-1.0)).</span><span class="sxs-lookup"><span data-stu-id="1179d-110">Similarly, when responding to an email, you can create and send the response in the same action ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0), or [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span></span> <span data-ttu-id="1179d-111">Ou você pode criar um rascunho da resposta ([responder](/graph/api/message-createreply?view=graph-rest-1.0), [responder a todos](/graph/api/message-createreplyall?view=graph-rest-1.0), ou [encaminhar](/graph/api/message-createforward?view=graph-rest-1.0)), [adicionar conteúdo](/graph/api/message-update?view=graph-rest-1.0)e então [enviar](/graph/api/message-send?view=graph-rest-1.0) o rascunho mais tarde.</span><span class="sxs-lookup"><span data-stu-id="1179d-111">Or, you can create a draft for the response ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0), or [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [add content](/graph/api/message-update?view=graph-rest-1.0), and then [send](/graph/api/message-send?view=graph-rest-1.0) the draft at a later time.</span></span>

<span data-ttu-id="1179d-112">Para distinguir entre um rascunho e uma mensagem enviada por programação, verifique a propriedade **isDraft**.</span><span class="sxs-lookup"><span data-stu-id="1179d-112">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="1179d-113">Por padrão, as mensagens de rascunho são salvas na pasta `Drafts` As mensagens enviadas são salvas na pasta `Sent Items`.</span><span class="sxs-lookup"><span data-stu-id="1179d-113">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="1179d-114">Para sua conveniência, é possível identificar a pasta Rascunhos e a pasta Itens enviados por seus [nomes de pasta correspondentes já bem conhecidos](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="1179d-114">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span></span> <span data-ttu-id="1179d-115">Por exemplo, você pode fazer o seguinte para [acessar as mensagens](/graph/api/user-list-messages?view=graph-rest-1.0) na pasta Rascunhos:</span><span class="sxs-lookup"><span data-stu-id="1179d-115">For example, you can do the following to [get the messages](/graph/api/user-list-messages?view=graph-rest-1.0) in the Drafts folder:</span></span>

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a><span data-ttu-id="1179d-116">Formato do corpo e script mal-intencionado</span><span class="sxs-lookup"><span data-stu-id="1179d-116">Body format and malicious script</span></span>

<!-- Remove the following 2 sections from the message.md topics
-->

<span data-ttu-id="1179d-117">O corpo da mensagem pode ser HTML ou texto, com HTML sendo retornado como o tipo de corpo da mensagem padrão na resposta GET.</span><span class="sxs-lookup"><span data-stu-id="1179d-117">The message body can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="1179d-118">Quando [receber uma mensagem](/graph/api/message-get?view=graph-rest-1.0), você pode especificar o cabeçalho da solicitação a seguir para retornar as propriedades **body** e **uniqueBody** no formato de texto:</span><span class="sxs-lookup"><span data-stu-id="1179d-118">When [getting a message](/graph/api/message-get?view=graph-rest-1.0), you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="1179d-119">Você pode especificar o cabeçalho a seguir ou, apenas ignorar o cabeçalho, para obter o corpo da mensagem no formato HTML:</span><span class="sxs-lookup"><span data-stu-id="1179d-119">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="1179d-120">Quando você especifica um cabeçalho, uma resposta bem-sucedida inclui o cabeçalho `Preference-Applied` correspondente:</span><span class="sxs-lookup"><span data-stu-id="1179d-120">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="1179d-121">Para solicitações de formato de texto: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="1179d-121">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="1179d-122">Para solicitações de formato HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="1179d-122">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="1179d-123">Se o corpo for HTML, por padrão, o Outlook remove qualquer HTML potencialmente não seguro (por exemplo, JavaScript) inserido na propriedade **body** antes de retornar o conteúdo do corpo em uma resposta REST.</span><span class="sxs-lookup"><span data-stu-id="1179d-123">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="1179d-124">Para obter o conteúdo HTML completo original, inclua o seguinte cabeçalho da solicitação HTTP:</span><span class="sxs-lookup"><span data-stu-id="1179d-124">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a><span data-ttu-id="1179d-125">Diferenciar as propriedades from e sender</span><span class="sxs-lookup"><span data-stu-id="1179d-125">Differentiating the from and sender properties</span></span>

<span data-ttu-id="1179d-126">Quando uma mensagem está sendo redigida, na maioria dos casos, o Outlook configura as propriedades **from** e **sender** para o mesmo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="1179d-126">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="1179d-127">Você pode atualizar essas propriedades nas seguintes situações:</span><span class="sxs-lookup"><span data-stu-id="1179d-127">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="1179d-p105">A propriedade **from** poderá ser alterada se o administrador do Exchange tiver atribuído direitos **sendAs** da caixa de correio a alguns outros usuários. O administrador pode fazer isso selecionando as **Permissões de Caixa de Correio** do proprietário da caixa de correio no Portal do Azure ou usando o Centro de Administração do Exchange ou um cmdlet Add-ADPermission do Windows PowerShell. Em seguida, você pode definir programaticamente a propriedade **from** como um desses usuários com direitos **sendAs** para essa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1179d-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="1179d-131">A propriedade **sender** poderá ser alterada se o proprietário da caixa de correio tiver delegado o envio de mensagens dessa caixa de correio para um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="1179d-131">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="1179d-132">O proprietário da caixa de correio pode delegar no Outlook.</span><span class="sxs-lookup"><span data-stu-id="1179d-132">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="1179d-133">Quando um representante envia uma mensagem em nome do proprietário da caixa de correio, o Outlook define a propriedade **sender** como a conta desse representante, enquanto a propriedade **from** continua a do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1179d-133">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="1179d-134">Você pode definir programaticamente a propriedade **sender** para um usuário com permissões de representante para essa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1179d-134">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="1179d-135">Usar as Dicas de Email para verificar o status do destinatário e economizar tempo (prévia)</span><span class="sxs-lookup"><span data-stu-id="1179d-135">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="1179d-136">Use as [Dicas de Email](/graph/api/resources/mailtips?view=graph-rest-beta) para tomar decisões inteligentes antes de enviar um email.</span><span class="sxs-lookup"><span data-stu-id="1179d-136">Use [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="1179d-137">As Dicas de Email podem lhe dar informações, como saber que a caixa de correio do destinatário é restrita para remetentes específicos, ou que aprovação é necessária para enviar emails ao destinatário.</span><span class="sxs-lookup"><span data-stu-id="1179d-137">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="1179d-138">Integração com o gesto social "@" (prévia)</span><span class="sxs-lookup"><span data-stu-id="1179d-138">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="1179d-139">As menções com @ são notificações para alertar os usuários quando eles são mencionados nas mensagens.</span><span class="sxs-lookup"><span data-stu-id="1179d-139">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="1179d-140">O recurso [mention](/graph/api/resources/mention?view=graph-rest-beta) permite que os aplicativos configurem e acessem gestos sociais online comuns, como o prefixo "@", em emails.</span><span class="sxs-lookup"><span data-stu-id="1179d-140">The [mention](/graph/api/resources/mention?view=graph-rest-beta) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="1179d-141">Você pode:</span><span class="sxs-lookup"><span data-stu-id="1179d-141">You can:</span></span>

- <span data-ttu-id="1179d-142">Criar menções com @ quando [criar uma mensagem](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span><span class="sxs-lookup"><span data-stu-id="1179d-142">Create @-mentions when [creating a message](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span></span>
- [<span data-ttu-id="1179d-143">Obter todas as mensagens na caixa de correio do usuário que contenham uma menção com @ do usuário</span><span class="sxs-lookup"><span data-stu-id="1179d-143">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [<span data-ttu-id="1179d-144">Obter todas as menções com @ que sejam mensagens</span><span class="sxs-lookup"><span data-stu-id="1179d-144">Get all the @-mention is a message</span></span>](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="1179d-145">Outras funcionalidades compartilhadas</span><span class="sxs-lookup"><span data-stu-id="1179d-145">Other shared capabilities</span></span>

<span data-ttu-id="1179d-146">Aproveite as seguintes funcionalidades comuns que são compartilhadas entre entidades do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="1179d-146">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="1179d-147">Assine as [notificações de alteração](/graph/api/resources/webhooks?view=graph-rest-1.0) em mensagens quando ocorrem um ou mais tipos de alterações, como a criação de mensagens ou atualização.</span><span class="sxs-lookup"><span data-stu-id="1179d-147">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="1179d-148">[Acompanhar essas alterações incrementais para as mensagens em uma pasta](delta-query-messages.md)</span><span class="sxs-lookup"><span data-stu-id="1179d-148">[Track these incremental changes to messages in a folder](delta-query-messages.md).</span></span>
- <span data-ttu-id="1179d-149">Crie [extensões abertas](extensibility-overview.md#open-extensions) ou [extensões de esquema](extensibility-overview.md#schema-extensions) para adicionar dados personalizados a uma instância de mensagem.</span><span class="sxs-lookup"><span data-stu-id="1179d-149">Create [open extensions](extensibility-overview.md#open-extensions) or [schema extensions](extensibility-overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="1179d-150">Crie [propriedades estendidas](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) em uma instância da mensagem para armazenar dados personalizados para as propriedades MAPI do Outlook, quando essas propriedades ainda não estão expostas nos metadados da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1179d-150">Create [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1179d-151">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1179d-151">Next steps</span></span>

<span data-ttu-id="1179d-152">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="1179d-152">Find out more about:</span></span>

- [<span data-ttu-id="1179d-153">Por que integrar-se com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="1179d-153">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="1179d-154">[Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e seus [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="1179d-154">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
