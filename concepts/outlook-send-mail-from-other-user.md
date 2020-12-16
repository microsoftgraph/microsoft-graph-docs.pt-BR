---
title: Enviar mensagens do Outlook de outro usuário
description: Use as permissões enviar como e enviar em nome de para enviar mensagens do Outlook como outro usuário ou a caixa de correio compartilhada no Microsoft Graph.
author: jasonjoh
localization_priority: Priority
ms.prod: outlook
ms.date: 01/16/2019
ms.openlocfilehash: becb0c4eb76e7ae337d42739f064a15b7ce233ca
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895514"
---
# <a name="send-outlook-messages-from-another-user"></a><span data-ttu-id="4efbb-103">Enviar mensagens do Outlook de outro usuário</span><span class="sxs-lookup"><span data-stu-id="4efbb-103">Send Outlook messages from another user</span></span>

<span data-ttu-id="4efbb-104">Exchange Online fornece [permissões de caixa de correio](/Exchange/recipients/mailbox-permissions) que permitem um usuário enviar o email que parece ter sido enviado de outro usuário, a lista de distribuição, grupo, recurso ou caixa de correio compartilhada.</span><span class="sxs-lookup"><span data-stu-id="4efbb-104">Exchange Online provides [mailbox permissions](/Exchange/recipients/mailbox-permissions) that allow a user to send mail that appears to be sent from another user, distribution list, group, resource, or shared mailbox.</span></span> <span data-ttu-id="4efbb-105">O Microsoft Graph também dá suporte a este recurso, mas o resultado final varia dependendo das permissões exatas concedidas no Exchange Online e que API você usa para enviar o email.</span><span class="sxs-lookup"><span data-stu-id="4efbb-105">Microsoft Graph supports this feature as well, but the end result varies depending on the exact permissions granted in Exchange Online and which API you use to send the mail.</span></span>

## <a name="permissions"></a><span data-ttu-id="4efbb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4efbb-106">Permissions</span></span>

<span data-ttu-id="4efbb-107">Dois tipos de permissões são aplicáveis para enviar mensagens de outro usuário: [permissões do Microsoft Graph](permissions-reference.md)e as permissões de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4efbb-107">Two types of permissions apply to sending messages from another user: [Microsoft Graph permissions](permissions-reference.md), and mailbox permissions.</span></span>

### <a name="microsoft-graph-permissions"></a><span data-ttu-id="4efbb-108">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4efbb-108">Microsoft Graph permissions</span></span>

<span data-ttu-id="4efbb-109">Para enviar mensagens de outro usuário, aplicativos que usam tokens de usuário, use a permissão **Mail.Send.Shared**.</span><span class="sxs-lookup"><span data-stu-id="4efbb-109">In order to send messages from another user, applications that use user tokens use the **Mail.Send.Shared** permission.</span></span>

> [!NOTE]
> <span data-ttu-id="4efbb-110">Os aplicativos que usam tokens de aplicativo em vez de tokens de usuário e tem a permissão **Mail.Send** consentida por um administrador, pode enviar emails, como qualquer usuário na organização enviando o email normalmente através da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4efbb-110">Applications that use application tokens instead of user tokens and have the **Mail.Send** permission consented by an administrator can send mail as any user in the organization by sending the mail normally through the user's mailbox.</span></span>

### <a name="mailbox-permissions"></a><span data-ttu-id="4efbb-111">Permissões de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="4efbb-111">Mailbox permissions</span></span>

<span data-ttu-id="4efbb-112">Duas permissões afetam o resultado final de enviar uma mensagem de outro usuário: **enviar em nome** e **enviar como**.</span><span class="sxs-lookup"><span data-stu-id="4efbb-112">Two permissions affect the end result of sending a message from another user: **Send on Behalf** and **Send As**.</span></span> <span data-ttu-id="4efbb-113">O usuário que entra no aplicativo com a permissão **Mail.Send.Shared** DEVE ter pelo menos uma destas permissões que foram concedidas para a caixa de correio, grupo ou lista de distribuição de onde o email é.</span><span class="sxs-lookup"><span data-stu-id="4efbb-113">The user that is signed in to your application with the **Mail.Send.Shared** permission MUST have at least one of these permissions granted to the mailbox, group, or distribution list that the mail is from.</span></span>

#### <a name="send-on-behalf"></a><span data-ttu-id="4efbb-114">Enviar em Nome de</span><span class="sxs-lookup"><span data-stu-id="4efbb-114">Send on Behalf</span></span>

<span data-ttu-id="4efbb-115">Com essa permissão, o destinatário do email tem uma indicação em clientes de email que a mensagem foi enviada pelo usuário do seu aplicativo em nome de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4efbb-115">With this permission, the recipient of the email has an indication in their email client that the message was sent by the user of your application on behalf of another user.</span></span>

![Captura de tela do Outlook na web que indica que uma mensagem foi enviada por um usuário em nome do outro](images/outlook-sent-on-behalf.png)

<span data-ttu-id="4efbb-117">Isso é exibido no Microsoft Graph, como o `sender` (usuário realmente a enviou) e propriedades do `from` (usuário/grupo/etc que a mensagem aparece como sendo de).</span><span class="sxs-lookup"><span data-stu-id="4efbb-117">This is exposed in Microsoft Graph as the `sender` (user that actually sent the message) and `from` (user/group/etc. that the message appears to be from) properties.</span></span>

```json
{
  "id": "AAMkAGE1...",
  "subject": "Send mail test",
  "sender": {
    "emailAddress": {
      "name": "Adele Vance",
      "address": "AdeleV@contoso.com"
    }
  },
  "from": {
    "emailAddress": {
      "name": "Pradeep Gupta",
      "address": "PradeepG@contoso.com"
    }
  }
}
```

<span data-ttu-id="4efbb-118">Um usuário pode conceder permissão para suas caixas de correio a outro usuário, [usando o Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926).</span><span class="sxs-lookup"><span data-stu-id="4efbb-118">A user can grant this permission for their own mailbox to another user by [using Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926).</span></span> <span data-ttu-id="4efbb-119">Os administradores podem conceder permissão para qualquer lista de distribuição, grupo ou caixa de correio no [Centro de administração do Microsoft 365](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4efbb-119">Administrators can grant this permission for any mailbox, group, or distribution list in the [Microsoft 365 admin center](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide).</span></span>

#### <a name="send-as"></a><span data-ttu-id="4efbb-120">Enviar como</span><span class="sxs-lookup"><span data-stu-id="4efbb-120">Send As</span></span>

<span data-ttu-id="4efbb-121">Com essa permissão, não há nenhuma indicação de que a mensagem foi enviada como um usuário diferente.</span><span class="sxs-lookup"><span data-stu-id="4efbb-121">With this permission, there is no indication that the message was sent as a different user.</span></span> <span data-ttu-id="4efbb-122">As propriedades `sender` e `from` têm o mesmo valor.</span><span class="sxs-lookup"><span data-stu-id="4efbb-122">The `sender` and `from` properties have the same value.</span></span>

<span data-ttu-id="4efbb-123">Os usuários não podem conceder essa permissão para suas caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="4efbb-123">Users cannot grant this permission to their mailboxes.</span></span> <span data-ttu-id="4efbb-124">Os administradores podem conceder essa permissão no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4efbb-124">Admins can grant this permission in the Microsoft 365 admin center.</span></span>

## <a name="sending-with-microsoft-graph"></a><span data-ttu-id="4efbb-125">Enviar com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4efbb-125">Sending with Microsoft Graph</span></span>

<span data-ttu-id="4efbb-126">Você pode enviar mensagens de outro usuário seja [enviar diretamente](/graph/api/user-sendmail?view=graph-rest-1.0) ou [criar um rascunho](/graph/api/user-post-messages?view=graph-rest-1.0) e, em seguida, [enviá-lo](/graph/api/message-send?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="4efbb-126">You can send messages from another user by either [sending directly](/graph/api/user-sendmail?view=graph-rest-1.0) or by [creating a draft](/graph/api/user-post-messages?view=graph-rest-1.0) and then [sending it](/graph/api/message-send?view=graph-rest-1.0).</span></span>

<span data-ttu-id="4efbb-127">Para enviar de outro usuário, defina a `from` propriedade em [mensagem](/graph/api/resources/message?view=graph-rest-1.0) enviada ao endereço de email do usuário para enviar de.</span><span class="sxs-lookup"><span data-stu-id="4efbb-127">In order to send from another user, set the `from` property on the [message](/graph/api/resources/message?view=graph-rest-1.0) sent to the email address of the user to send from.</span></span> <span data-ttu-id="4efbb-128">Não é necessário configurar a propriedade `sender` - Microsoft Graph irá defini-la adequadamente, com base nas permissões de caixa de correio concedidas para usuários conectados.</span><span class="sxs-lookup"><span data-stu-id="4efbb-128">You don't need to set the `sender` property - Microsoft Graph will set it appropriately, based on the mailbox permissions granted to the user who has signed in.</span></span>

<span data-ttu-id="4efbb-129">Por exemplo, para enviar emails do grupo `sales@contoso.com`, configure a mensagem da seguinte maneira.</span><span class="sxs-lookup"><span data-stu-id="4efbb-129">For example, to send mail from the `sales@contoso.com` group, configure the message as follows.</span></span>

```json
{
  "subject": "January sales report",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "MeganB@contoso.com"
      }
    }
  ],
  "from": {
    "emailAddress": {
      "address": "sales@contoso.com"
    }
  }
}
```

## <a name="sent-items-behavior"></a><span data-ttu-id="4efbb-130">Comportamento de itens enviado</span><span class="sxs-lookup"><span data-stu-id="4efbb-130">Sent Items behavior</span></span>

<span data-ttu-id="4efbb-131">Depois que a mensagem é enviada, pode ser salva em pastas de itens enviados do usuário de envio, a sua pasta Itens enviados do usuário ou ambas.</span><span class="sxs-lookup"><span data-stu-id="4efbb-131">After the message is sent, it can be saved to the sending user's Sent Items folder, the from user's Sent Items folder, or both.</span></span> <span data-ttu-id="4efbb-132">Ele também não pode ser salvo de forma alguma.</span><span class="sxs-lookup"><span data-stu-id="4efbb-132">It can also not be saved at all.</span></span>

> [!NOTE]
> <span data-ttu-id="4efbb-133">Se a mensagem é enviada de um endereço que não tenha uma caixa de correio (uma lista de distribuição, por exemplo), não há nenhuma item enviados para o usuário.</span><span class="sxs-lookup"><span data-stu-id="4efbb-133">If the message is sent from an address that does not have a mailbox (a distribution list, for example), there is no Sent Items for the from user.</span></span>

- <span data-ttu-id="4efbb-134">Se o aplicativo enviar usando o `/me` ponto de extremidade (ou `/users/{user-id}` onde a `user-id` corresponde ao usuário conectado), por padrão, a mensagem será salva na pasta Itens enviados de envio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4efbb-134">If your application sends by using the `/me` endpoint (or `/users/{user-id}` where the `user-id` corresponds to the signed in user), by default, the message will be saved in the sending user's Sent Items folder.</span></span>
- <span data-ttu-id="4efbb-135">Se o aplicativo enviar usando o `/users/{user-id}` onde a `user-id` corresponde à de usuário, por padrão, a mensagem será salva na da pasta Itens enviados do usuário.</span><span class="sxs-lookup"><span data-stu-id="4efbb-135">If your application sends by using the `/users/{user-id}` where the `user-id` corresponds to the from user, by default, the message will be saved in the from user's Sent Items folder.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="4efbb-136">Para enviar dessa maneira, o usuário de envio deve ter a permissão de caixa de correio **acesso total**, além de uma permissão **enviar em nome** ou **enviar como**.</span><span class="sxs-lookup"><span data-stu-id="4efbb-136">In order to send this way, the sending user must have the **Full Access** mailbox permission in addition to either the **Send on Behalf** or **Send As** permission.</span></span>

<span data-ttu-id="4efbb-137">O comportamento padrão pode ser alterado por outros fatores externos:</span><span class="sxs-lookup"><span data-stu-id="4efbb-137">The default behavior can be changed by other outside factors:</span></span>

- <span data-ttu-id="4efbb-138">Os administradores podem atualizar na caixa de correio do usuário para [sempre salvar uma cópia das mensagens enviadas de um representante](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox) para seus itens enviados.</span><span class="sxs-lookup"><span data-stu-id="4efbb-138">Administrators can update the from user's mailbox to [always save a copy of messages sent from a delegate](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox) to their Sent Items.</span></span>
- <span data-ttu-id="4efbb-139">Configurando a `saveToSentItems` propriedade para `false` em um solicitação [enviar email](/graph/api/user-sendmail?view=graph-rest-1.0), você pode impedir o item de ser salvo na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="4efbb-139">By setting the `saveToSentItems` property to `false` in a [send mail](/graph/api/user-sendmail?view=graph-rest-1.0) request, you can prevent the item from being saved to the Sent Items folder.</span></span> <span data-ttu-id="4efbb-140">No entanto, se o administrador definiu a configuração "sempre salvar uma cópia", a mensagem será ainda salva a partir dos itens enviados do usuário.</span><span class="sxs-lookup"><span data-stu-id="4efbb-140">However, if an administrator has configured the "always save a copy" setting, the message will still be saved to the from user's Sent Items.</span></span>

## <a name="examples"></a><span data-ttu-id="4efbb-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4efbb-141">Examples</span></span>

### <a name="example-1-successful-send-through-me-endpoint"></a><span data-ttu-id="4efbb-142">Exemplo 1: Envio bem-sucedido pelo ponto de extremidade /me</span><span class="sxs-lookup"><span data-stu-id="4efbb-142">Example 1: Successful send through /me endpoint</span></span>

<span data-ttu-id="4efbb-143">Neste exemplo, Adele Vance recebeu a permissão **enviar em nome** para a caixa de correio de Allan Deyoung.</span><span class="sxs-lookup"><span data-stu-id="4efbb-143">In this example, Adele Vance has been granted **Send on Behalf** permission to Allan Deyoung's mailbox.</span></span>

#### <a name="request"></a><span data-ttu-id="4efbb-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4efbb-144">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Expense reports",
    "body": {
      "contentType": "text",
      "content": "Have you submitted your expense reports yet?"
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": {
      "emailAddress": {
        "address": "AllanD@contoso.com"
      }
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="4efbb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4efbb-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-unsuccessful-attempt-to-send-without-permissions"></a><span data-ttu-id="4efbb-146">Exemplo 2: Falha na tentativa de enviar sem permissões</span><span class="sxs-lookup"><span data-stu-id="4efbb-146">Example 2: Unsuccessful attempt to send without permissions</span></span>

<span data-ttu-id="4efbb-147">Neste exemplo, Adele Vance tenta enviar um email de Patti Fernandez, mas não recebeu uma permissão **enviar em nome** ou **enviar como**.</span><span class="sxs-lookup"><span data-stu-id="4efbb-147">In this example, Adele Vance attempts to send an email from Patti Fernandez, but has not been granted either the **Send on Behalf** or **Send As** permission.</span></span> <span data-ttu-id="4efbb-148">A resposta contém um `ErrorSendAsDenied` erro.</span><span class="sxs-lookup"><span data-stu-id="4efbb-148">The response contains a `ErrorSendAsDenied` error.</span></span>

<!-- markdownlint-disable MD024 -->

#### <a name="request"></a><span data-ttu-id="4efbb-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4efbb-149">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Support ticket",
    "body": {
      "contentType": "text",
      "content": "I noticed you opened a support ticket yesterday..."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": {
      "emailAddress": {
        "address": "PattiF@contoso.com"
      }
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="4efbb-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4efbb-150">Response</span></span>

```http
HTTP/1.1 403 Forbidden
Content-Type: application/json

{
  "error": {
    "code": "ErrorSendAsDenied",
    "message": "The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account. Cannot submit message.",
    "innerError": {
      "request-id": "24e7991e-01ae-4cc2-8e06-532a96fd8948",
      "date": "2019-01-16T18:53:25"
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="4efbb-151">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4efbb-151">Next steps</span></span>

<span data-ttu-id="4efbb-152">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="4efbb-152">Find out more about:</span></span>

- [<span data-ttu-id="4efbb-153">Por que integrar-se com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="4efbb-153">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="4efbb-154">[Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e email API [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="4efbb-154">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and mail API [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      FileNotFound: '[/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox](always save a copy of messages sent from a delegate)'.",
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      InvalidUrlFormat '[/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide](Office 365 admin center)'.",
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      FileNotFound: '[/Exchange/recipients/mailbox-permissions](mailbox permissions)'. "
  ]
}
-->
