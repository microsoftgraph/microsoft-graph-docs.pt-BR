---
title: Automatizar a criação, o envio e o processamento de mensagens
description: Emails são representados pelo recurso de mensagem no Microsoft Graph.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: b64c06d86cc4228a3254840103496dbe89890788
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474439"
---
# <a name="automate-creating-sending-and-processing-messages"></a><span data-ttu-id="2027e-103">Automatizar a criação, o envio e o processamento de mensagens</span><span class="sxs-lookup"><span data-stu-id="2027e-103">Automate creating, sending, and processing messages</span></span>

<span data-ttu-id="2027e-104">Emails são representados pelo recurso de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2027e-104">Emails are represented by the [message](/graph/api/resources/message?view=graph-rest-1.0) resource in Microsoft Graph.</span></span>

<span data-ttu-id="2027e-105">Por padrão, as mensagens são identificadas por uma ID de entrada exclusiva na propriedade **id**.</span><span class="sxs-lookup"><span data-stu-id="2027e-105">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="2027e-106">Quando uma mensagem é criada e salva incialmente como um rascunho ou enviada, o provedor de armazenamento atribui a mensagem a uma ID de entrada.</span><span class="sxs-lookup"><span data-stu-id="2027e-106">When a message is initially created and saved as a draft or sent, the store provider assigns the message an entry ID.</span></span> <span data-ttu-id="2027e-107">Por padrão, essa ID muda quando a mensagem é copiada ou movida para outra pasta, armazenada ou um arquivo .PST.</span><span class="sxs-lookup"><span data-stu-id="2027e-107">By default, that ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span> <span data-ttu-id="2027e-108">Faça referência à mensagem usando sua ID atual para o processá-la.</span><span class="sxs-lookup"><span data-stu-id="2027e-108">You reference the message by its current ID for further processing.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="2027e-109">Criar e enviar mensagens</span><span class="sxs-lookup"><span data-stu-id="2027e-109">Creating and sending mail</span></span>

<span data-ttu-id="2027e-110">No Outlook, você pode criar e enviar um email na mesma ação [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) ou pode [criar](/graph/api/user-post-messages?view=graph-rest-1.0) um rascunho, posteriormente [adicionar conteúdo](/graph/api/message-update?view=graph-rest-1.0) e [enviar](/graph/api/message-send?view=graph-rest-1.0) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="2027e-110">In Outlook, you can create and send an email in the same [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) action, or you can [create](/graph/api/user-post-messages?view=graph-rest-1.0) a draft, subsequently [add content](/graph/api/message-update?view=graph-rest-1.0) and [send](/graph/api/message-send?view=graph-rest-1.0) the draft.</span></span>

<span data-ttu-id="2027e-111">Da mesma forma, quando responder a um email, você pode criar e enviar a resposta da mesma ação ([responder](/graph/api/message-reply?view=graph-rest-1.0), [responder a todos](/graph/api/message-replyall?view=graph-rest-1.0) ou [encaminhar](/graph/api/message-forward?view=graph-rest-1.0)).</span><span class="sxs-lookup"><span data-stu-id="2027e-111">Similarly, when responding to an email, you can create and send the response in the same action ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0), or [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span></span> <span data-ttu-id="2027e-112">Ou você pode criar um rascunho da resposta ([responder](/graph/api/message-createreply?view=graph-rest-1.0), [responder a todos](/graph/api/message-createreplyall?view=graph-rest-1.0), ou [encaminhar](/graph/api/message-createforward?view=graph-rest-1.0)), [adicionar conteúdo](/graph/api/message-update?view=graph-rest-1.0)e então [enviar](/graph/api/message-send?view=graph-rest-1.0) o rascunho mais tarde.</span><span class="sxs-lookup"><span data-stu-id="2027e-112">Or, you can create a draft for the response ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0), or [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [add content](/graph/api/message-update?view=graph-rest-1.0), and then [send](/graph/api/message-send?view=graph-rest-1.0) the draft at a later time.</span></span>

<span data-ttu-id="2027e-113">Para distinguir entre um rascunho e uma mensagem enviada por programação, verifique a propriedade **isDraft**.</span><span class="sxs-lookup"><span data-stu-id="2027e-113">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="2027e-114">Por padrão, as mensagens de rascunho são salvas na pasta `Drafts` As mensagens enviadas são salvas na pasta `Sent Items`.</span><span class="sxs-lookup"><span data-stu-id="2027e-114">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="2027e-115">Para sua conveniência, é possível identificar a pasta Rascunhos e a pasta Itens enviados por seus [nomes de pasta correspondentes já bem conhecidos](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="2027e-115">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span></span>

### <a name="setting-the-from-and-sender-properties"></a><span data-ttu-id="2027e-116">Definindo as propriedades from e sender</span><span class="sxs-lookup"><span data-stu-id="2027e-116">Setting the from and sender properties</span></span>

<span data-ttu-id="2027e-117">Quando uma mensagem está sendo redigida, na maioria dos casos, o Outlook configura as propriedades **from** e **sender** para o mesmo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2027e-117">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="2027e-118">Você pode atualizar essas propriedades nas seguintes situações:</span><span class="sxs-lookup"><span data-stu-id="2027e-118">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="2027e-p105">A propriedade **from** poderá ser alterada se o administrador do Exchange tiver atribuído direitos **sendAs** da caixa de correio a alguns outros usuários. O administrador pode fazer isso selecionando as **Permissões de Caixa de Correio** do proprietário da caixa de correio no Portal do Azure ou usando o Centro de Administração do Exchange ou um cmdlet Add-ADPermission do Windows PowerShell. Em seguida, você pode definir programaticamente a propriedade **from** como um desses usuários com direitos **sendAs** para essa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2027e-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="2027e-122">A propriedade **sender** poderá ser alterada se o proprietário da caixa de correio tiver delegado o envio de mensagens dessa caixa de correio para um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="2027e-122">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="2027e-123">O proprietário da caixa de correio pode delegar no Outlook.</span><span class="sxs-lookup"><span data-stu-id="2027e-123">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="2027e-124">Quando um representante envia uma mensagem em nome do proprietário da caixa de correio, o Outlook define a propriedade **sender** como a conta desse representante, enquanto a propriedade **from** continua a do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2027e-124">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="2027e-125">Você pode definir programaticamente a propriedade **sender** para um usuário com permissões de representante para essa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2027e-125">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="2027e-126">Usar as Dicas de Email para verificar o status do destinatário e economizar tempo (prévia)</span><span class="sxs-lookup"><span data-stu-id="2027e-126">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="2027e-127">Use as [Dicas de Email](/graph/api/resources/mailtips?view=graph-rest-beta) para tomar decisões inteligentes antes de enviar um email.</span><span class="sxs-lookup"><span data-stu-id="2027e-127">Use [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="2027e-128">As Dicas de Email podem lhe dar informações, como saber que a caixa de correio do destinatário é restrita para remetentes específicos, ou que aprovação é necessária para enviar emails ao destinatário.</span><span class="sxs-lookup"><span data-stu-id="2027e-128">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>


## <a name="reading-messages-with-control-over-the-body-format-returned"></a><span data-ttu-id="2027e-129">Ler mensagens com controle sobre o formato de corpo retornado</span><span class="sxs-lookup"><span data-stu-id="2027e-129">Reading messages with control over the body format returned</span></span>

<span data-ttu-id="2027e-130">Você pode [ler uma mensagem](/graph/api/message-get?view=graph-rest-1.0) em uma caixa de correio fazendo referência a sua ID:</span><span class="sxs-lookup"><span data-stu-id="2027e-130">You can [read a message](/graph/api/message-get?view=graph-rest-1.0) in a mailbox by referencing its ID:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

Ou, pode [receber as mensagens](/graph/api/user-list-messages?view=graph-rest-1.0) em uma pasta específica. <span data-ttu-id="2027e-132">Por exemplo, para ler mensagens na pasta Rascunhos do usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="2027e-132">For example, to read messages in the signed-in user's Drafts folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

<span data-ttu-id="2027e-133">O corpo de uma mensagem do Outlook pode ser HTML ou texto, com HTML sendo retornado como o tipo de corpo da mensagem padrão na resposta GET.</span><span class="sxs-lookup"><span data-stu-id="2027e-133">The body of an Outlook message can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="2027e-134">Quando receber uma mensagem, você poderá especificar o cabeçalho da solicitação a seguir para retornar as propriedades **body** e **uniqueBody** no formato de texto:</span><span class="sxs-lookup"><span data-stu-id="2027e-134">When getting a message, you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="2027e-135">Você pode especificar o cabeçalho a seguir ou, apenas ignorar o cabeçalho, para obter o corpo da mensagem no formato HTML:</span><span class="sxs-lookup"><span data-stu-id="2027e-135">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="2027e-136">Quando você especifica um cabeçalho, uma resposta bem-sucedida inclui o cabeçalho `Preference-Applied` correspondente:</span><span class="sxs-lookup"><span data-stu-id="2027e-136">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="2027e-137">Para solicitações de formato de texto: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="2027e-137">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="2027e-138">Para solicitações de formato HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="2027e-138">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="2027e-139">Se o corpo for HTML, por padrão, o Outlook remove qualquer HTML potencialmente não seguro (por exemplo, JavaScript) inserido na propriedade **body** antes de retornar o conteúdo do corpo em uma resposta REST.</span><span class="sxs-lookup"><span data-stu-id="2027e-139">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="2027e-140">Para obter o conteúdo HTML completo original, inclua o seguinte cabeçalho da solicitação HTTP:</span><span class="sxs-lookup"><span data-stu-id="2027e-140">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="2027e-141">Integração com o gesto social "@" (prévia)</span><span class="sxs-lookup"><span data-stu-id="2027e-141">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="2027e-142">As menções com @ são notificações para alertar os usuários quando eles são mencionados nas mensagens.</span><span class="sxs-lookup"><span data-stu-id="2027e-142">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="2027e-143">O recurso [mention](/graph/api/resources/mention?view=graph-rest-beta) permite que os aplicativos configurem e acessem gestos sociais online comuns, como o prefixo "@", em emails.</span><span class="sxs-lookup"><span data-stu-id="2027e-143">The [mention](/graph/api/resources/mention?view=graph-rest-beta) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="2027e-144">Você pode:</span><span class="sxs-lookup"><span data-stu-id="2027e-144">You can:</span></span>

- <span data-ttu-id="2027e-145">Criar menções com @ quando [criar uma mensagem](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span><span class="sxs-lookup"><span data-stu-id="2027e-145">Create @-mentions when [creating a message](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span></span>
- [<span data-ttu-id="2027e-146">Obter todas as mensagens na caixa de correio do usuário que contenham uma menção com @ do usuário</span><span class="sxs-lookup"><span data-stu-id="2027e-146">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [<span data-ttu-id="2027e-147">Obter todas as menções com @ que sejam mensagens</span><span class="sxs-lookup"><span data-stu-id="2027e-147">Get all the @-mention is a message</span></span>](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="2027e-148">Outras funcionalidades compartilhadas</span><span class="sxs-lookup"><span data-stu-id="2027e-148">Other shared capabilities</span></span>

<span data-ttu-id="2027e-149">Aproveite as seguintes funcionalidades comuns que são compartilhadas entre entidades do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="2027e-149">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="2027e-150">Assine as [notificações de alteração](/graph/api/resources/webhooks?view=graph-rest-1.0) em mensagens quando ocorrem um ou mais tipos de alterações, como a criação de mensagens ou atualização.</span><span class="sxs-lookup"><span data-stu-id="2027e-150">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="2027e-151">[Acompanhar essas alterações incrementais para as mensagens em uma pasta](delta-query-messages.md)</span><span class="sxs-lookup"><span data-stu-id="2027e-151">[Track these incremental changes to messages in a folder](delta-query-messages.md).</span></span>
- <span data-ttu-id="2027e-152">Crie [extensões abertas](extensibility-overview.md#open-extensions) ou [extensões de esquema](extensibility-overview.md#schema-extensions) para adicionar dados personalizados a uma instância de mensagem.</span><span class="sxs-lookup"><span data-stu-id="2027e-152">Create [open extensions](extensibility-overview.md#open-extensions) or [schema extensions](extensibility-overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="2027e-153">Crie [propriedades estendidas](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) em uma instância da mensagem para armazenar dados personalizados para as propriedades MAPI do Outlook, quando essas propriedades ainda não estão expostas nos metadados da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2027e-153">Create [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2027e-154">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2027e-154">Next steps</span></span>

<span data-ttu-id="2027e-155">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="2027e-155">Find out more about:</span></span>

- [<span data-ttu-id="2027e-156">Por que integrar com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="2027e-156">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- [<span data-ttu-id="2027e-157">Obter conteúdo MIME (visualização)</span><span class="sxs-lookup"><span data-stu-id="2027e-157">Get MIME content (preview)</span></span>](outlook-get-mime-message.md)
- [<span data-ttu-id="2027e-158">Receber mensagens compartilhadas</span><span class="sxs-lookup"><span data-stu-id="2027e-158">Get shared messages</span></span>](outlook-share-messages-folders.md)
- [<span data-ttu-id="2027e-159">Enviar mensagens do Outlook de outro usuário</span><span class="sxs-lookup"><span data-stu-id="2027e-159">Send Outlook messages from another user</span></span>](outlook-send-mail-from-other-user.md)
- [<span data-ttu-id="2027e-160">Obter identificadores imutáveis para recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="2027e-160">Get immutable identifiers for Outlook resources</span></span>](outlook-immutable-id.md)
- <span data-ttu-id="2027e-161">[Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e seus [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="2027e-161">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
