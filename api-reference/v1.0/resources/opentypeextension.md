# <a name="opentypeextension-resource-type-open-extensions"></a>Tipo de recurso openTypeExtension (extensões abertas)

As extensões abertas (anteriormente conhecidas como extensões de dados do Office 365) oferecem uma maneira fácil de adicionar diretamente propriedades não tipadas a um recurso no Microsoft Graph.

Extensões abertas são representadas pelo recurso **openTypeExtension**. Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação **extensions**, que deriva do tipo abstrato [extension](extension.md). Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados.

Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`. Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.

Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)

As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).

|Recurso |Versão |
|:---------------|:-------|
| [Unidade administrativa](../../beta/resources/administrativeunit.md)  | Somente para visualização |
| [Evento de calendário](event.md) | GA |
| [Evento de calendário](event.md) do grupo | GA |
| [Postagem](post.md) de thread de conversa do grupo | GA |
| [dispositivo](device.md) | GA |
| [grupo](group.md) | GA |
| [mensagem](message.md) | GA |
| [organização](organization.md) | GA |
| [Contato pessoal](contact.md) | GA |
| [usuário](user.md) | GA |

## <a name="outlook-specific-considerations"></a>Considerações específicas do Outlook

Cada extensão aberta presente em um recurso do Outlook (evento, mensagem ou contato pessoal) é armazenado em uma [propriedade denominada MAPI](https://msdn.microsoft.com/en-us/library/cc765864(v=office.15).aspx). Quando você cria extensões abertas para o Outlook, considere que as propriedades denominadas MAPI são um recurso finito na caixa de correio do usuário. Quando uma cota da propriedade denominada de um usuário for esgotada, é possível criar outras propriedades denominadas para esse usuário. Isso pode resultar em um comportamento inesperado de clientes que dependem do funcionamento de propriedades denominadas.

Aplique as seguintes diretrizes ao criar extensões abertas nos recursos do Outlook:

- Crie o número mínimo de extensões necessárias. A maioria dos aplicativos não deve exigir mais de uma extensão. As extensões não têm propriedades ou estrutura de conjunto definidas, portanto você armazenar vários valores em um única extensão.
- Evite nomear as extensões de maneira variável (como com base na entrada do usuário etc.). Cada vez que uma extensão aberta é criada com um novo nome não foi usado antes na caixa de correio de um usuário, uma nova propriedade denominada MAPI é criada. Remover a extensão não remove a propriedade denominada.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Usar extensões abertas (para recursos do Outlook) ou propriedades estendidas

As extensões abertas são a solução recomendada para a maioria dos cenários que envolvem o armazenamento e o acesso a dados personalizados. Se, no entanto, você precisar acessar dados personalizados para as propriedades MAPI do Outlook que ainda não foram expostas por meio dos [metadados da API REST do Outlook](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), você poderá usar as [ propriedades estendidas e sua API REST](extended-properties-overview.md). Você pode verificar quais propriedades os metadados expõe em [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>Propriedades

|Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|extensionName|Sequência de caracteres|Um identificador de texto exclusivo para uma extensão de tipo aberto. Obrigatório.|
|id|Sequência de caracteres| Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="methods"></a>Métodos

|Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Postagem](../api/opentypeextension_post_opentypeextension.md) | [openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contact](../resources/contact.md), [event](../resources/event.md) ou [message](../resources/message.md) que contenha um objeto openTypeExtension | Crie um objeto openTypeExtension em uma instância de recurso nova ou existente.|
|[Obter](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |Leia propriedades e relações do objeto openTypeExtension.|
|[Atualizar](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md) |Atualize o objeto openTypeExtension. |
|[Excluir](../api/opentypeextension_delete.md) | Nenhuma |Exclua um objeto openTypeExtension. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
