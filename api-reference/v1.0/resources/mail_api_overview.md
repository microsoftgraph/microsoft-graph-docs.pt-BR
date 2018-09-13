# <a name="use-the-outlook-mail-rest-api"></a>Usar a API REST do Outlook

O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos dados de email do Outlook do usuário em uma conta pessoal ou da organização. Com as [permissões de aplicativo e delegadas apropriadas](../../../concepts/permissions_reference.md), seu aplicativo pode acessar os dados de email do usuário conectado ou qualquer usuário em um locatário. Os dados de email podem estar na nuvem no Exchange Online como parte do Office 365, ou no Exchange no local em uma [implantação híbrida](../../../concepts/hybrid_rest_support.md).

## <a name="using-the-mail-rest-api"></a>Usar a API REST do email

As solicitações de API de email são realizadas em nome de um [usuário](../resources/user.md) que pode ser identificado pela propriedade **id** do usuário (um GUID exclusivo), endereço de email ou alias do atalho do `me` para o usuário conectado.

As mensagens de email são representadas pelo recurso [message](../resources/message.md) e organizado em uma [mailFolder](../resources/mailfolder.md). As mensagens e as pastas principais são identificadas por sua propriedade **id**, obtida das operações de `GET`.

>**Observação:** em geral, não pressupõem que as IDs de **message** e **mailfolder** são únicas e imutáveis em uma caixa de correio. Elas podem mudar após certas ações, como copiar, mover ou enviar.

Os corpos de mensagens podem estar no formato HTML ou no formato de texto.

Você pode usar nomes de pasta conhecidos como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems` para identificar determinadas pastas de e-mail que existem por padrão para todos os usuários. Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).

Por exemplo, você pode obter mensagens na pasta **Itens enviados** do Outlook do usuário conectado, sem primeiro obter a ID da pasta:

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>Casos comuns de uso

O recurso **message** expõe propriedades como **categories**, **conversationId**, **flag** e **importance** que correspondem a recursos disponíveis na interface do usuário, permitindo que os aplicativos automatizem ou integrem a experiência de usuário interna do Outlook.

A API do Microsoft Graph também fornece métodos e ações que ofereçam suporte a casos de uso comuns de mensagens.

| Casos de uso | Recursos REST | Confira também |
|:----------|:---------------|:---------|
| **Ações centradas no usuário** | | |
| Rascunho, ler, responder, encaminhar, enviar, atualizar ou excluir mensagens | [mensagem](../resources/message.md) | [Métodos de mensagem](../resources/message.md#methods) |
| Delegar outro usuário para enviar mensagens em nome do proprietário da caixa de correio | [mensagem](../resources/message.md) | Configurar as propriedades **from** e **sender** em uma [message](../resources/message.md) |
| Permitir que o usuário visualize as mensagens mais importantes primeiro | [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) | [Caixa de Entrada Prioritária](../resources/manage_focused_inbox.md) |
| Adicionar, obter ou excluir anexos de uma mensagem | [anexo](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [mensagem](../resources/message.md) | [Métodos de anexo](../resources/attachment.md#methods) |
| Obter ou atualizar resposta automática, localidade, fuso horário ou horário de trabalho de um usuário | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Obter configurações da caixa de correio do usuário](../api/user_get_mailboxsettings.md), <br> [Atualizar configurações da caixa de correio do usuários](../api/user_update_mailboxsettings.md) |
| Obtenha dicas de e-mail do status especiais de outros destinatários, como fora do escritório | [user](../resources/user.md), <br> [Dicas de E-mail](../resources/mailtips.md) | [Obtenha dicas de e-mail](../api/user_getmailtips.md) |
| **Gerenciamento de pasta e email** | | |
| Organizar mensagens em uma hierarquia de pasta de email | [mailFolder](../resources/mailfolder.md)  | [Métodos de mailFolder](../resources/mailfolder.md#methods) |
| Pesquisar e filtrar mensagens | [mensagem](../resources/message.md) | [Parâmetros de consulta](../../../concepts/query_parameters.md)  |
| Receber notificações de alterações para as mensagens em uma pasta | [subscription](../resources/subscription.md) | [Trabalhando com webhooks no Microsoft Graph](../resources/webhooks.md) |
| Sincronizar mensagens ou a hierarquia da pasta de email | [mensagem](../resources/message.md) | [Obter as alterações incrementais para as mensagens em uma pasta](../../../concepts/delta_query_messages.md) |
| **Desenvolvimento de aplicativo** | | |
| Adicionar dados de aplicativo personalizado como cabeçalhos de mensagem da Internet de uma mensagem | [mensagem](../resources/message.md) | Adicione dados personalizados para a propriedade **internetMessageHeaders** da mensagem. |
| Adicionar dados personalizados de aplicativo a uma mensagem usando extensões | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md) |
| Acessar dados personalizados para propriedades subexpostas de MAPI do Outlook | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Próximas etapas

A API de email pode permitir novas formas de envolvimento com os usuários:

- [Visão geral da API de email do Outlook](../../../concepts/outlook-mail-concept-overview.md)
- Analise em detalhes os [métodos](../resources/message.md#methods), [propriedades](../resources/message.md#properties) e [relações](../resources/message.md#relationships) dos recursos de [message](../resources/message.md) e [mailFolder](../resources/mailfolder.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/en-us/graph/graph/examples#partners).
