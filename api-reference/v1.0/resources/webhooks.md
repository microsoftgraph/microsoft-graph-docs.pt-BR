# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para obter notificações de alteração

A API REST do Microsoft Graph usa um mecanismo de webhook para enviar notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após as alterações. Para obter mais detalhes, incluindo como assinar e manipular notificações de entrada, consulte [Configurar notificações para alterações nos dados do usuário](../../../concepts/webhooks.md).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para ser notificado de alterações nos seguintes recursos:

- Mensagens
- Eventos
- Contatos
- Usuários
- Grupos
- Conversas em grupo
- Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint
- Pastas pessoais de usuários no OneDrive

## <a name="permissions"></a>Permissões

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription_post_subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso com suporte na v1.0                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| Delegado - conta corporativa ou de estudante     | [contato][], [conversa][], [unidade][], [evento][], [mensagem][] |
| Delegado - conta pessoal da Microsoft | Nenhum                                                             |
| Aplicativo                            | [contato][], [conversa][], [evento][], [mensagem][]            |

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](./subscription.md)
- [Obter assinatura](../api/subscription_get.md)
- [Criar assinatura](../api/subscription_post_subscriptions.md)
- [Atualizar assinatura](../api/subscription_update.md)
- [Excluir assinatura](../api/subscription_delete.md)

[contato]: ./contact.md
[conversa]: ./conversation.md
[unidade]: ./drive.md
[evento]: ./event.md
[mensagem]: ./message.md
