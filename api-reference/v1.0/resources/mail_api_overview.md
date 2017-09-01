# <a name="use-the-microsoft-graph-api-to-integrate-with-outlook-mail"></a>Usar a API do Microsoft Graph para integração com o email do Outlook

O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos dados de email do Outlook do usuário em uma conta pessoal ou da organização. Com as [permissões de aplicativo e delegadas apropriadas](../../../concepts/permissions_reference.md), seu aplicativo pode acessar os dados de email do usuário conectado ou qualquer usuário em um locatário. Os dados de email podem estar na nuvem no Exchange Online como parte do Office 365, ou no Exchange no local em uma [implantação híbrida](../../../concepts/hybrid_rest_support.md).

## <a name="using-the-mail-rest-api"></a>Usar a API REST do email
As solicitações de API de email são realizadas em nome de um [usuário](../resources/user.md) que pode ser identificado pela propriedade **id** do usuário (um GUID exclusivo), endereço de email ou alias do atalho do `me` para o usuário conectado.

As mensagens de email são representadas pelo recurso [message](../resources/message.md) e organizado em uma [mailFolder](../resources/mailfolder.md). As mensagens e as pastas principais são identificadas por sua propriedade **id**, obtida das operações de `GET`. 

>**Observação:** em geral, não pressupõem que as IDs de **message** e **mailfolder** são únicas e imutáveis em uma caixa de correio. Elas podem mudar após certas ações, como copiar, mover ou enviar. 

Os corpos de mensagens podem estar no formato HTML ou no formato de texto.

Você pode usar nomes comuns, como `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`, para identificar certas pastas de email que existem por padrão para todos os usuários. Por exemplo, você pode obter mensagem na pasta **Itens enviados** do Outlook do usuário conectado, sem primeiro obter o ID da pasta:
```
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>Casos comuns de uso 

O recurso **message** expõe propriedades como **categories**, **conversationId**, **flag** e **importance** que correspondem a recursos disponíveis na interface do usuário, permitindo que os aplicativos automatizem ou integrem a experiência de usuário interna do Outlook. 

A API do Microsoft Graph também fornece métodos e ações que ofereçam suporte a casos de uso comuns de mensagens.

| Casos de uso        | Recursos REST | Veja também |
|:---------------|:--------|:----------|
| **Ações centradas no usuário** | | |
| Rascunho, ler, responder, encaminhar, enviar, atualizar ou excluir mensagens | [message](../resources/message.md) | [Métodos de mensagem](../resources/message.md#methods) |
| Delegar outro usuário para enviar mensagens em nome do proprietário da caixa de correio | [message](../resources/message.md) | Configurar as propriedades **from** e **sender** em uma [message](../resources/message.md) |
| Permitir que o usuário visualize as mensagens mais importantes primeiro | [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) | [Caixa de Entrada Prioritária](../resources/manage_focused_inbox.md) |
| Adicionar, obter ou excluir anexos de uma mensagem | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Métodos de anexo](../resources/attachment.md#methods) |
| Obter ou atualizar a resposta automática, localidade ou fuso horário de um usuário | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md) | [Obter configurações da caixa de correio do usuário](../api/user_get_mailboxsettings.md), <br> [Atualizar configurações da caixa de correio do usuários](../api/user_update_mailboxsettings.md) |
| **Gerenciamento de pasta e email** | | |
| Organizar mensagens em uma hierarquia de pasta de email | [mailFolder](../resources/mailfolder.md)  | [Métodos de mailFolder](../resources/mailfolder.md#methods) |
| Pesquisar e filtrar mensagens | [message](../resources/message.md) | [Parâmetros de consulta](../../../concepts/query_parameters.md)  |
| Receber notificações de alterações para as mensagens em uma pasta | [subscription](../resources/subscription.md) | [Trabalhando com webhooks no Microsoft Graph](../resources/webhooks.md) |
| Sincronizar mensagens ou a hierarquia da pasta de email | [message](../resources/message.md) | [Obter as alterações incrementais para as mensagens em uma pasta](../../../concepts/delta_query_messages.md) |
| **Desenvolvimento de aplicativo** | | |
| Adicionar dados personalizados de aplicativo a uma mensagem usando extensões | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md) |
| Acessar dados personalizados para propriedades subexpostas de MAPI do Outlook | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Próximas etapas
A API de email pode permitir novas formas de envolvimento com os usuários: 

- Analise em detalhes os [métodos](../resources/message.md#methods), [propriedades](../resources/message.md#properties) e [relações](../resources/message.md#relationships) dos recursos de [message](../resources/message.md) e [mailFolder](../resources/mailfolder.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/en-us/graph/graph/examples#partners).


