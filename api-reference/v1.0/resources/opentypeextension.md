# <a name="opentypeextension-resource-type-open-extensions"></a>Tipo de recurso openTypeExtension (extensões abertas)

As extensões abertas (conhecidas anteriormente como extensões de dados do Office 365) fornecem uma maneira fácil de adicionar propriedades não tipadas diretamente a um recurso no Microsoft Graph. Extensões abertas são representadas pelo recurso **openTypeExtension**. Qualquer extensão aberta adicionada a um recurso é mostrada na propriedade de navegação das **extensions**, que deriva do tipo abstrato [extension](extension.md).  Cada extensão tem uma propriedade **extensionName**, que é a única propriedade predefinida e gravável para todas as extensões, juntamente com seus dados personalizados. Um modo de garantir que os nomes de extensão sejam exclusivos é usar um formato reverso de DNS no sistema de nomes de domínio que dependa de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`. Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.

Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)

As extensões abertas têm suporte nos recursos a seguir nas versões correspondentes - disponibilidade geral (GA: /v1.0 e /beta) ou visualização (/beta).

| Recurso | Versão |
|---------------|-------|
| [Unidade administrativa](../../beta/resources/administrativeunit.md)  | Somente para visualização |
| [Evento de calendário](event.md) | GA |
| [Evento de calendário](event.md) do grupo | GA |
| [Postagem](post.md) de thread de conversa do grupo | GA |
| [device](device.md) | GA |
| [group](group.md) | GA |
| [message](message.md) | GA |
| [organization](organization.md) | GA |
| [Contato pessoal](contact.md) | GA |
| [user](user.md) | GA |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Usar extensões abertas (para recursos do Outlook) ou propriedades estendidas?

As extensões abertas são a solução recomendada para a maioria dos cenários que envolvem armazenar e acessar dados personalizados. Se, no entanto, você precisar acessar dados personalizados para as propriedades do Outlook MAPI que já não estão expostos por meio dos [metadados da API do Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), você pode usar [as propriedades estendidas e sua API REST](extended-properties-overview.md). Você pode confirmar quais propriedades os metadados expõem em https://graph.microsoft.com/v1.0/$ metadados.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensionName|String|Um identificador de texto exclusivo para uma extensão de tipo aberto. Obrigatório.|
|id|String| Um identificador totalmente qualificado que concatena o tipo de extensão com **extensionName**. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension_post_opentypeextension.md) | [openTypeExtension](opentypeextension.md) (em uma instância de recurso existente) ou um novo [contato](../resources/contact.md), [evento](../resources/event.md) ou [mensagem](../resources/message.md) que contenha um objeto openTypeExtension. | Crie um objeto openTypeExtension em uma instância de recurso novo ou existente.|
|[Get](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |Leia propriedades e relações do objeto openTypeExtension.|
|[Update](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md)   |Atualize o objeto openTypeExtension. |
|[Delete](../api/opentypeextension_delete.md) | Nenhuma |Exclua um objeto openTypeExtension. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->