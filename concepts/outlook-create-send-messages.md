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
# <a name="automate-creating-sending-and-processing-messages"></a>Automatizar a criação, o envio e o processamento de mensagens

Emails são representados pelo recurso de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) no Microsoft Graph.

Por padrão, as mensagens são identificadas por uma ID de entrada exclusiva na propriedade **id**. Quando uma mensagem é criada e salva incialmente como um rascunho ou enviada, o provedor de armazenamento atribui a mensagem a uma ID de entrada. Por padrão, essa ID muda quando a mensagem é copiada ou movida para outra pasta, armazenada ou um arquivo .PST. Faça referência à mensagem usando sua ID atual para o processá-la.

## <a name="creating-and-sending-mail"></a>Criar e enviar mensagens

No Outlook, você pode criar e enviar um email na mesma ação [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) ou pode [criar](/graph/api/user-post-messages?view=graph-rest-1.0) um rascunho, posteriormente [adicionar conteúdo](/graph/api/message-update?view=graph-rest-1.0) e [enviar](/graph/api/message-send?view=graph-rest-1.0) o rascunho.

Da mesma forma, quando responder a um email, você pode criar e enviar a resposta da mesma ação ([responder](/graph/api/message-reply?view=graph-rest-1.0), [responder a todos](/graph/api/message-replyall?view=graph-rest-1.0) ou [encaminhar](/graph/api/message-forward?view=graph-rest-1.0)). Ou você pode criar um rascunho da resposta ([responder](/graph/api/message-createreply?view=graph-rest-1.0), [responder a todos](/graph/api/message-createreplyall?view=graph-rest-1.0), ou [encaminhar](/graph/api/message-createforward?view=graph-rest-1.0)), [adicionar conteúdo](/graph/api/message-update?view=graph-rest-1.0)e então [enviar](/graph/api/message-send?view=graph-rest-1.0) o rascunho mais tarde.

Para distinguir entre um rascunho e uma mensagem enviada por programação, verifique a propriedade **isDraft**.

Por padrão, as mensagens de rascunho são salvas na pasta `Drafts` As mensagens enviadas são salvas na pasta `Sent Items`. Para sua conveniência, é possível identificar a pasta Rascunhos e a pasta Itens enviados por seus [nomes de pasta correspondentes já bem conhecidos](/graph/api/resources/mailfolder?view=graph-rest-1.0).

### <a name="setting-the-from-and-sender-properties"></a>Definindo as propriedades from e sender

Quando uma mensagem está sendo redigida, na maioria dos casos, o Outlook configura as propriedades **from** e **sender** para o mesmo usuário conectado. Você pode atualizar essas propriedades nas seguintes situações:

- A propriedade **from** poderá ser alterada se o administrador do Exchange tiver atribuído direitos **sendAs** da caixa de correio a alguns outros usuários. O administrador pode fazer isso selecionando as **Permissões de Caixa de Correio** do proprietário da caixa de correio no Portal do Azure ou usando o Centro de Administração do Exchange ou um cmdlet Add-ADPermission do Windows PowerShell. Em seguida, você pode definir programaticamente a propriedade **from** como um desses usuários com direitos **sendAs** para essa caixa de correio.
- A propriedade **sender** poderá ser alterada se o proprietário da caixa de correio tiver delegado o envio de mensagens dessa caixa de correio para um ou mais usuários. O proprietário da caixa de correio pode delegar no Outlook. Quando um representante envia uma mensagem em nome do proprietário da caixa de correio, o Outlook define a propriedade **sender** como a conta desse representante, enquanto a propriedade **from** continua a do proprietário da caixa de correio. Você pode definir programaticamente a propriedade **sender** para um usuário com permissões de representante para essa caixa de correio.

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a>Usar as Dicas de Email para verificar o status do destinatário e economizar tempo (prévia)

Use as [Dicas de Email](/graph/api/resources/mailtips?view=graph-rest-beta) para tomar decisões inteligentes antes de enviar um email.
As Dicas de Email podem lhe dar informações, como saber que a caixa de correio do destinatário é restrita para remetentes específicos, ou que aprovação é necessária para enviar emails ao destinatário.


## <a name="reading-messages-with-control-over-the-body-format-returned"></a>Ler mensagens com controle sobre o formato de corpo retornado

Você pode [ler uma mensagem](/graph/api/message-get?view=graph-rest-1.0) em uma caixa de correio fazendo referência a sua ID:

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

Ou, pode [receber as mensagens](/graph/api/user-list-messages?view=graph-rest-1.0) em uma pasta específica. Por exemplo, para ler mensagens na pasta Rascunhos do usuário conectado:

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

O corpo de uma mensagem do Outlook pode ser HTML ou texto, com HTML sendo retornado como o tipo de corpo da mensagem padrão na resposta GET.

Quando receber uma mensagem, você poderá especificar o cabeçalho da solicitação a seguir para retornar as propriedades **body** e **uniqueBody** no formato de texto:

```http
Prefer: outlook.body-content-type="text"
```

Você pode especificar o cabeçalho a seguir ou, apenas ignorar o cabeçalho, para obter o corpo da mensagem no formato HTML:

```http
Prefer: outlook.body-content-type="html"
```

Quando você especifica um cabeçalho, uma resposta bem-sucedida inclui o cabeçalho `Preference-Applied` correspondente:

- Para solicitações de formato de texto: `Preference-Applied: outlook.body-content-type="text"`
- Para solicitações de formato HTML: `Preference-Applied: outlook.body-content-type="html"`

Se o corpo for HTML, por padrão, o Outlook remove qualquer HTML potencialmente não seguro (por exemplo, JavaScript) inserido na propriedade **body** antes de retornar o conteúdo do corpo em uma resposta REST.

Para obter o conteúdo HTML completo original, inclua o seguinte cabeçalho da solicitação HTTP:

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a>Integração com o gesto social "@" (prévia)

As menções com @ são notificações para alertar os usuários quando eles são mencionados nas mensagens. O recurso [mention](/graph/api/resources/mention?view=graph-rest-beta) permite que os aplicativos configurem e acessem gestos sociais online comuns, como o prefixo "@", em emails.
Você pode:

- Criar menções com @ quando [criar uma mensagem](/graph/api/user-post-messages?view=graph-rest-beta#request-2)
- [Obter todas as mensagens na caixa de correio do usuário que contenham uma menção com @ do usuário](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [Obter todas as menções com @ que sejam mensagens](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a>Outras funcionalidades compartilhadas

Aproveite as seguintes funcionalidades comuns que são compartilhadas entre entidades do Microsoft Graph:

- Assine as [notificações de alteração](/graph/api/resources/webhooks?view=graph-rest-1.0) em mensagens quando ocorrem um ou mais tipos de alterações, como a criação de mensagens ou atualização.
- [Acompanhar essas alterações incrementais para as mensagens em uma pasta](delta-query-messages.md)
- Crie [extensões abertas](extensibility-overview.md#open-extensions) ou [extensões de esquema](extensibility-overview.md#schema-extensions) para adicionar dados personalizados a uma instância de mensagem.
- Crie [propriedades estendidas](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) em uma instância da mensagem para armazenar dados personalizados para as propriedades MAPI do Outlook, quando essas propriedades ainda não estão expostas nos metadados da API do Microsoft Graph.

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar com o email do Outlook](outlook-mail-concept-overview.md)
- [Obter conteúdo MIME (visualização)](outlook-get-mime-message.md)
- [Receber mensagens compartilhadas](outlook-share-messages-folders.md)
- [Enviar mensagens do Outlook de outro usuário](outlook-send-mail-from-other-user.md)
- [Obter identificadores imutáveis para recursos do Outlook](outlook-immutable-id.md)
- [Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e seus [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.
