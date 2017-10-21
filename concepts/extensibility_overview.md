# <a name="add-custom-data-to-resources-using-extensions"></a>Adicionar dados personalizados a recursos usando extensões

O Microsoft Graph fornece um único ponto de extremidade de API que dá acesso a dados avançados centrados em pessoas e percepções por meio de vários recursos, como [user](../api-reference/v1.0/resources/user.md) e [message](../api-reference/v1.0/resources/message.md). Agora há uma maneira de _**estender**_ o Microsoft Graph com seus próprios dados de aplicativo. Você pode adicionar propriedades personalizadas aos recursos do Microsoft Graph sem a necessidade de um repositório de dados externos. Por exemplo, você pode decidir manter seu aplicativo leve e armazenar dados de perfil de usuário específicos do aplicativo no Microsoft Graph estendendo o recurso **user**. Como alternativa, convém manter o repositório de perfil de usuário existente do aplicativo e simplesmente adicionar um identificador de repositório específico do aplicativo para o recurso **user**.

O Microsoft Graph oferece dois tipos de extensões. Escolha o tipo de extensão mais adequado às suas necessidades de aplicativo:

*  **Extensões abertas**: Um bom ponto de partida para os desenvolvedores.
*  **Extensões de esquema**: Um mecanismo mais versátil para desenvolvedores que se preocupam em armazenar dados digitados, tornando seu esquema detectável e compartilhável, ser capaz de filtrar e futuramente executar a validação de dados de entrada e a autorização.

>**Importante:** Você não deve usar extensões para armazenar informações de identificação pessoal confidenciais, como credenciais de conta, números de identificação do governo, dados do titular do cartão, dados de conta corrente, informações médicas ou informações básicas confidenciais.

## <a name="supported-resources"></a>Recursos com suporte

A seguinte tabela lista os recursos que oferecem suporte às extensões de abertura e esquema e indica se eles atingiram ou não a disponibilidade geral (GA) (disponível em ambos os pontos de extremidade V1.0 e beta) ou se estão como prévia (disponível apenas no ponto de extremidade beta).  

| Recurso | Extensões abertas | Extensões de esquema |
|---------------|-------|-------|
| [Unidade administrativa](../api-reference/beta/resources/administrativeunit.md) | Somente para visualização | Somente para visualização |
|  [Evento de calendário](../api-reference/v1.0/resources/event.md) | GA | GA |
|  [Dispositivo](../api-reference/v1.0/resources/device.md) | GA | GA |
|  [Grupo](../api-reference/v1.0/resources/group.md) | GA | GA |
|  [Evento de calendário do grupo](../api-reference/v1.0/resources/event.md) | GA | GA |
|  [Postagem de conversa em grupo](../api-reference/v1.0/resources/post.md) | GA | GA |
|  [Mensagem](../api-reference/v1.0/resources/message.md) | GA | GA |
|  [Organização](../api-reference/v1.0/resources/organization.md) | GA | GA |
|  [Contato pessoal](../api-reference/v1.0/resources/contact.md)| GA | GA |
|  [Usuário](../api-reference/v1.0/resources/user.md) | GA | GA |

Você pode usar extensões em todos esses recursos ao se conectar com uma conta de trabalho ou escolar. Além disso, você pode usar extensões desses recursos – **evento**, **postar**, **grupo**, **mensagem**, **contato** e **usuário** – quando conectado com uma conta pessoal. 

## <a name="open-extensions"></a>Extensões abertas

[Extensões abertas](../api-reference/v1.0/resources/opentypeextension.md) (anteriormente conhecidas como extensões de dados do Office 365) são [tipos abertos](http://www.odata.org/getting-started/advanced-tutorial/#openType) que oferecem uma maneira flexível de adicionar dados de aplicativo não tipados diretamente a uma instância do recurso. 

As extensões abertas, juntamente com seus dados personalizados, podem ser acessadas por meio da propriedade de navegação **extensões** da instância do recurso. A propriedade **extensionName** é a única propriedade _predefinida_ gravável em uma extensão aberta. Ao criar uma extensão aberta, você deve atribuir à propriedade **extensionName** um nome exclusivo no locatário. Uma maneira de fazer isso é usar um formato DNS (sistema de nomes de domínio) inverso que seja dependente de _seu próprio domínio_, por exemplo, `Com.Contoso.ContactInfo`. Não use o domínio Microsoft (`Com.Microsoft` ou `Com.OnMicrosoft`) em um nome de extensão.

Você pode [criar uma extensão aberta](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md) em uma instância de recurso e armazenar dados personalizados nela na mesma operação (observe a [limitação conhecida abaixo](known_issues.md#extensions) para alguns dos recursos com suporte). Você pode posteriormente [ler](../api-reference/v1.0/api/opentypeextension_get.md), [atualizar](../api-reference/v1.0/api/opentypeextension_update.md) ou [excluir](../api-reference/v1.0/api/opentypeextension_delete.md) a extensão e seus dados.

Exemplo de extensão aberta: [Adicionar dados personalizados aos usuários usando extensões abertas](extensibility_open_users.md)

## <a name="schema-extensions"></a>Extensões de esquema

[Extensões de esquema](../api-reference/v1.0/resources/schemaextension.md) permitem que você defina um esquema que pode usar para estender um tipo de recurso. Primeiro, crie a definição de extensão de esquema. Em seguida, use-a para estender instâncias de recurso com dados personalizados fortemente tipados. Além disso, você pode controlar o [status](#schema-extensions-lifecycle) da extensão de esquema e permitir que ela seja descoberta por outros aplicativos. Esses aplicativos, por sua, vez podem usar a extensão para seus dados e criar experiências adicionais nela.

Ao criar uma definição de extensão de esquema, você deve fornecer um nome exclusivo para sua **id**. Há duas opções de nomes:

- Se já tiver um domínio personalizado `.com`,`.net`, `.gov`, `.edu` ou `.org` que verificou com seu locatário, você poderá usar o nome de domínio com o nome de esquema para definir um nome exclusivo, neste formato: \{_&#65279;nomedoDomínio_\}\_\{_&#65279;nomedoEsquema_\}. Por exemplo, se seu domínio personalizado for contoso.com, você poderá definir a **id** de `contoso_mySchema`.  Essa é a opção preferencial.
- Se não tiver um domínio personalizado verificado, você poderá definir apenas a **id** para um nome de esquema (sem um prefixo de nome de domínio), por exemplo, `mySchema`. O Microsoft Graph atribuirá uma ID de cadeia de caracteres com base no nome fornecido, neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}.  Por exemplo, `extkvbmkofy_mySchema`.

Você verá esse nome exclusivo na **id** usada como o nome do tipo complexo que armazenará os dados personalizados na instância do recurso estendido.

Diferentemente das extensões abertas, o gerenciamento de definições de extensão de esquema ([list](../api-reference/v1.0/api/schemaextension_list.md), [create](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md), [get](../api-reference/v1.0/api/schemaextension_get.md), [update](../api-reference/v1.0/api/schemaextension_update.md) e [delete](../api-reference/v1.0/api/schemaextension_delete.md)) e gerenciar seus dados (adicionar, obter, atualizar e excluir dados) são conjuntos separados de operações de API. 

Como as extensões de esquema são acessíveis como tipos complexos em instâncias dos recursos de destino, você pode executar operações CRUD nos dados personalizados de uma extensão de esquema das seguintes maneiras:

- Use o método `POST` de recurso para especificar dados personalizados ao criar uma nova instância de recurso.
- Use o método `GET` de recurso para ler os dados personalizados.
- Use o método `PATCH` de recurso para adicionar ou atualizar dados personalizados em uma instância de recursos existentes.
- Use o método `PATCH` de recurso para definir o tipo complexo como nulo, para excluir os dados personalizados da instância do recurso. 

Exemplo de extensão do esquema: [Adicionar dados personalizados a grupos usando as extensões do esquema](extensibility_schema_groups.md)


### <a name="schema-extensions-lifecycle"></a>Ciclo de vida das extensões do esquema

Quando o aplicativo cria uma definição de extensão do esquema, ele é marcado como proprietária da extensão do esquema. 

O aplicativo proprietário pode mover a extensão pelos diferentes estados de um ciclo de vida, usando uma operação PATCH na propriedade **status**. Dependendo do estado atual, o aplicativo proprietário poderá atualizar ou excluir a extensão. Todas as atualizações para uma extensão de esquema devem ser sempre apenas aditivas e incondicionais.


| Estado | Comportamento de estado de ciclo de vida |
|-------------|------------|
| InDevelopment | <ul><li>Estado inicial após a criação. O aplicativo de proprietário ainda está desenvolvendo a extensão do esquema. </li><li>Nesse estado, somente o aplicativo do proprietário pode estender instâncias de recursos com essa definição do esquema e apenas no mesmo diretório onde o proprietário do aplicativo está registrado. </li><li>Apenas o aplicativo proprietário pode atualizar a definição de extensão com alterações aditivas ou excluí-la. </li><li>O aplicativo proprietário pode mover a extensão do esquema de **InDevelopment** para o estado **Disponível**.</li></ul> |
| Disponível | <ul><li>A extensão do esquema está disponível para ser usada por todos os aplicativos em qualquer locatário. </li><li>Depois que o aplicativo proprietário define a extensão como **Disponível**, qualquer aplicativo pode simplesmente adicionar dados personalizados a instâncias desses tipos de recursos especificados na extensão (desde que o aplicativo tenha permissões para esse recurso). O aplicativo pode atribuir dados personalizados ao criar uma nova instância ou atualizar uma instância existente. </li><li>O aplicativo proprietário pode atualizar a definição de extensão com alterações aditivas. <br>– Nenhum aplicativo pode excluir a definição de extensão nesse estado. </li><li>O proprietário do aplicativo pode mover a extensão do esquema de **Disponível** para o estado **Preterido**.</li></ul> |
| Preterido | <ul><li>A definição de extensão de esquema não pode ser lido nem modificada. </li><li>Nenhum aplicativo pode ler, atualizar, adicionar novas propriedades ou excluir a extensão. </li><li>No entanto, os aplicativos ainda podem ler, atualizar ou excluir _valores de propriedade_ de extensão existentes. </li><li>O aplicativo proprietário pode mover a extensão do esquema de **Preterida** de volta ao estado **Disponível**.</li></ul> |

### <a name="supported-property-data-types"></a>Tipos de dados de propriedade com suporte

Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:

| Tipo de propriedade | Comentários |
|-------------|------------|
| Binária | No máximo 256 bytes. |
| Booliano | Não é compatível com as mensagens, eventos e postagens. |
| DateTime | Deve ser especificado no formato ISO 8601. Serão armazenados no UTC. |
| Inteiro | Valor de 32 bits. Não é compatível com as mensagens, eventos e postagens. |
| String | Máximo de 256 caracteres. |

>**Observação:** Propriedades de múltiplos valores não são suportadas.

### <a name="azure-ad-directory-schema-extensions"></a>Extensões do esquema de diretório do Azure AD

O Azure AD dá suporte a um tipo semelhante de extensões, conhecido como [extensões de esquema de diretório](https://msdn.microsoft.com/en-us/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions), em alguns recursos [directoryObject](../api-reference/v1.0/resources/directoryObject.md). Embora você deva usar a API do Graph do Azure AD para criar e gerenciar as definições de extensões de esquema de diretório, pode usar a API do Microsoft Graph para adicionar, obter, atualizar e excluir _dados_ nas propriedades dessas extensões.

## <a name="permissions"></a>Permissions

As mesmas [permissões](./permissions_reference.md) necessárias para ler ou gravar um recurso específico também são necessárias para ler ou gravar quaisquer dados de extensões nesse recurso.  Por exemplo, para que um aplicativo seja capaz de atualizar o perfil de um usuário conectado com dados de aplicativo personalizados, o aplicativo deve receber a permissão *User.ReadWrite.All*.

Além disso, para criar e gerenciar definições de extensão do esquema, um aplicativo deve receber a permissão *Directory.AccessAsUser.All*.

## <a name="data-limits"></a>Limites de dados

### <a name="open-extension-limits"></a>Limites de extensão aberta
Os seguintes limites se aplicam aos recursos de diretório (como **usuário**, **grupo**, **dispositivo**):

- Cada extensão aberta pode ter até 2 KB de dados (incluindo a definição da extensão em si).
- Um aplicativo pode adicionar até duas extensões abertas por instância do recurso.

### <a name="schema-extension-limits"></a>Limites de extensão do esquema
Um aplicativo pode criar não mais de cinco definições de **extensão do esquema**.

## <a name="known-limitations"></a>Limitações conhecidas

Nas limitações conhecidas usando extensões, veja a [seção extensões](known_issues.md#extensions) no artigo problemas conhecidos.

## <a name="extension-examples"></a>Exemplos de extensão

[Adicionar dados personalizados aos usuários usando extensões abertas](extensibility_open_users.md)

[Adicionar dados personalizados a grupos usando as extensões do esquema](extensibility_schema_groups.md)

## <a name="see-also"></a>Confira também

[Domínios do Office 365](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[Adição e verificação de um domínio para um locatário do Office 365](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
