---
title: Adicionar dados personalizados aos recursos usando extensões
description: Você pode estender Microsoft Graph com seus próprios dados de aplicativo. Adicione propriedades personalizadas para armazenar dados personalizados em recursos do Microsoft Graph sem exigir um armazenamento de dados externo.
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: a7d2a2eeba27877afe5c1aba4fbc416ad10d48c9
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856110"
---
# <a name="add-custom-data-to-resources-using-extensions"></a>Adicionar dados personalizados aos recursos usando extensões

O Microsoft Graph fornece um único ponto de extremidade de API para acessar dados e insights avançados centrados em pessoas através de recursos, como [usuário](/graph/api/resources/user) e [mensagem](/graph/api/resources/message). Você também pode estender o Microsoft Graph adicionando propriedades personalizadas a instâncias de recursos sem a necessidade de um armazenamento de dados externo.

Neste artigo, discutiremos como o Microsoft Graph dá suporte à extensão de seus recursos, as opções disponíveis para adicionar propriedades personalizadas e quando usá-las.

> [!IMPORTANT]
> Não use extensões para armazenar informações de identificação pessoal confidenciais, como credenciais de conta, números de identificação do governo, dados do titular do cartão, dados de conta corrente, informações médicas ou informações básicas confidenciais.

## <a name="why-add-custom-properties-to-microsoft-graph"></a>Por que adicionar propriedades personalizadas do Microsoft Graph?

> [!IMPORTANT]
> Você não deve usar extensões para armazenar informações de identificação pessoal confidenciais, como credenciais de conta, números de identificação do governo, dados do titular do cartão, dados de conta corrente, informações médicas ou informações básicas confidenciais.
* Como desenvolvedor de ISV você pode decidir manter seu aplicativo leve e armazenar dados de perfil de usuário específicos do aplicativo no Microsoft Graph estendendo o recurso **usuário**.
* Como alternativa, convém manter o repositório de perfil de usuário existente do aplicativo e adicionar um identificador de específico do aplicativo para o recurso **usuário**.
* Como desenvolvedor corporativo, os aplicativos internos que você cria podem depender dos dados específicos de RH da sua organização. A integração em vários aplicativos pode ser simplificada armazenando esses dados em propriedades personalizadas no Microsoft Graph.

## <a name="custom-property-options-in-microsoft-graph"></a>Opções de propriedade personalizadas no Microsoft Graph

O Microsoft Graph oferece quatro tipos de extensões para adicionar propriedades personalizadas.

- Propriedades de atributos de extensão
- Extensões de diretório (Azure AD)
- Extensões de esquema
- Extensões abertas

### <a name="extension-attributes"></a>Atributos de extensão

O Azure AD oferece um conjunto de 15 propriedades personalizadas com nomes predefinidos nos recursos [user](/graph/api/resources/onpremisesextensionattributes) e [device](/graph/api/resources/onpremisesextensionattributes). Essas propriedades eram inicialmente atributos personalizados fornecidos no Active Directory local (AD) e no Microsoft Exchange. No entanto, agora elas podem ser usadas não apenas para sincronizar dados locais do AD e do Microsoft Exchange com o Azure AD por meio do Microsoft Graph.

#### <a name="developer-experience"></a>Experiência do desenvolvedor

Você pode usar os 15 atributos de extensão para armazenar valores string em instâncias de recurso de **usuário** ou **dispositivo**, por meio das propriedades **onPremisesExtensionAttributes** e **extensionAttributes**, respectivamente. Os valores podem ser atribuídos ao criar uma nova instância de recurso ou ao atualizar uma instância de recurso existente. Eles também podem ser filtrados.

##### <a name="add-or-update-data-in-extension-attributes"></a>Adicionar ou atualizar dados em atributos de extensão

O exemplo a seguir mostra como armazenar dados em **extensionAttribute1** e excluir dados existentes de **extensionAttribute12** por meio de uma operação de atualização com um método PATCH.

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b

{
    "onPremisesExtensionAttributes": {
        "extensionAttribute1": "skypeId.adeleVance",
        "extensionAttribute13": null
    }
}
```

A solicitação retorna uma resposta `204 No Content`.

##### <a name="retrieve-data-from-extension-attributes-1-15"></a>Recuperar dados de atributos de extensão de 1 a 15

###### <a name="request"></a>Solicitação

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,displayName,onPremisesExtensionAttributes
```

###### <a name="response"></a>Resposta

```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,onPremisesExtensionAttributes)",
    "value": [
        {
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "displayName": "Adele Vance",
            "onPremisesExtensionAttributes": {
                "extensionAttribute1": "Contractor",
                "extensionAttribute2": "50",
                "extensionAttribute3": null,
                "extensionAttribute4": "1478354",
                "extensionAttribute5": "10239390",
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": "11",
                "extensionAttribute11": null,
                "extensionAttribute12": "/o=ExchangeLabs/ou=Exchange Administrative Group (FYDIBOHF47SPDLT)/cn=Recipients/cn=5ee781fc7egc7aa0b9394bddb44e7f04-Adele Vance",
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            }
        }
    ]
}
```

### <a name="directory-azure-ad-extensions"></a>Extensões de diretório (Azure AD)

[As extensões de diretório](/graph/api/resources/extensionProperty) fornecem aos desenvolvedores uma experiência de extensão fortemente tipada, detectável e filtrável para objetos de diretório.

As extensões de diretório são registradas primeiro em um aplicativo por meio da operação [Create extensionProperty](/graph/api/application-post-extensionproperty) e devem ser explicitamente direcionadas a objetos de diretório específicos. Depois que o aplicativo tiver sido consentido por um usuário ou administrador, as propriedades de extensão se tornarão imediatamente acessíveis no locatário. Todos os aplicativos autorizados no locatário podem ler e gravar dados em quaisquer propriedades de extensão definidas em uma instância do objeto de diretório de destino.

Para obter a lista de tipos de recursos que podem ser especificados como objetos de destino para uma extensão de diretório, consulte [Escolha um tipo de extensão para seu aplicativo](#choose-an-extension-type-for-your-application).

#### <a name="developer-experience"></a>Experiência do desenvolvedor

As definições de extensão de diretório são gerenciadas por meio do recurso [extensionProperty](/graph/api/resources/extensionproperty) e seus métodos associados. Os dados são gerenciados por meio das mesmas solicitações REST que você usa para gerenciar a instância de recurso.

##### <a name="create-a-directory-extension-definition"></a>Criar uma definição de extensão de diretório

Antes de adicionar uma extensão de diretório a uma instância de recurso, você deve primeiro criar uma definição de extensão de diretório.

###### <a name="request"></a>Solicitação

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/applications/30a5435a-1871-485c-8c7b-65f69e287e7b/extensionProperties

{
    "name": "jobGroupTracker",
    "dataType": "String",
    "targetObjects": [
        "User"
    ]
}
```

###### <a name="response"></a>Resposta

Uma propriedade de extensão de diretório chamada `extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker` é criada com um nome de extensão que segue a seguinte convenção de nomenclatura: *extension_{appId-without-hyphens}_{extensionProperty-name}*.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications('30a5435a-1871-485c-8c7b-65f69e287e7b')/extensionProperties/$entity",
    "id": "4e3dbc8f-ca32-41b4-825a-346215d7d20f",
    "deletedDateTime": null,
    "appDisplayName": "HR-sync-app",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "name": "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker",
    "targetObjects": [
        "User"
    ]
}
```

##### <a name="add-a-directory-extension-property-to-a-target-object"></a>Adicionar uma propriedade de extensão de diretório a um objeto de destino

Depois de criar a definição de extensão de diretório, você pode adicioná-la a uma instância de um tipo de objeto de destino. Você pode armazenar dados na propriedade de extensão de diretório ao criar uma nova instância do objeto de destino ou ao atualizar um objeto existente. O exemplo a seguir mostra como armazenar dados na propriedade de extensão de diretório ao criar um novo objeto de usuário.

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": false,
        "password": "xWwvJ]6NMw+bWH-d"
    },
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "JobGroupN"
}
```

A solicitação retorna um código de resposta `201 Created` e um objeto [user](/graph/api/resources/user) no corpo da resposta.

##### <a name="retrieve-a-directory-extension-property"></a>Recuperar uma propriedade de extensão de diretório

O exemplo a seguir mostra como as propriedades de extensão de diretório e os dados associados são apresentados em uma instância de recurso. A propriedade de extensão será retornada por padrão por meio do ponto de extremidade `beta`, mas somente no ponto de extremidade `$select` por meio do ponto de extremidade `v1.0`.

##### <a name="request"></a>Solicitação

```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,displayName,extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker,extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable
```

##### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker,extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable)",
    "value": [
        {
            "id": "63384f56-42d2-4aa7-b1d6-b10c78f143a2",
            "displayName": "Adele Vance",
            "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "E4",
            "extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable": true
        }
    ]
}
```

##### <a name="update-or-delete-directory-extension-properties"></a>Atualizar ou excluir propriedades de extensão de diretório

Para atualizar ou excluir o valor da propriedade de extensão de diretório para uma instância de recurso, use o método PATCH. Para excluir a propriedade de extensão e seu valor associado da instância de recurso, defina seu valor como `null`.

A solicitação a seguir atualiza o valor de uma propriedade de extensão de diretório e exclui outra propriedade de extensão.

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/63384f56-42d2-4aa7-b1d6-b10c78f143a2

{
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable": null,
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "E4"
}
```

A solicitação retorna o código de resposta `204 No Content`.

### <a name="schema-extensions"></a>Extensões de esquema

[As extensões de esquema Microsoft Graph](/graph/api/resources/schemaextension) são conceitualmente semelhantes às extensões de diretório. Primeiro, crie a definição de extensão de esquema. Em seguida, use-o para estender instâncias de recursos com suporte com propriedades personalizadas fortemente tipadas. Além disso, você pode controlar o [status](/graph/api/resources/schemaextension#schema-extensions-lifecycle) da extensão de esquema e permitir que ela seja descoberta por outros aplicativos.

Para obter a lista de tipos de recursos que dão suporte a extensões de esquema, consulte [Escolha um tipo de extensão para seu aplicativo](#choose-an-extension-type-for-your-application).

> [!VIDEO https://www.youtube-nocookie.com/embed/3MOAlUFNus0]

#### <a name="developer-experience"></a>Experiência do desenvolvedor

Ao criar uma definição de extensão de esquema, você deve fornecer um nome exclusivo para sua **id**. Há duas opções de nomes:

- Se já tiver um domínio personalizado `.com`,`.net`, `.gov`, `.edu` ou `.org` que verificou com seu locatário, você poderá usar o nome de domínio com o nome de esquema para definir um nome exclusivo, neste formato: *{domainName}* _ *{schemaName}*. Por exemplo, se o seu domínio personalizado for `contoso.com`, você pode definir uma **id** de `contoso_mySchema`. Essa opção é altamente recomendada.
- Se não tiver um domínio personalizado verificado, você poderá definir apenas a **id** para um nome de esquema (sem um prefixo de nome de domínio). Por exemplo, `mySchema`. O Microsoft Graph atribuirá uma ID de cadeia de caracteres com base no nome fornecido, neste formato: `ext{8-random-alphanumeric-chars}_{schema-name}` Por exemplo, `extkvbmkofy_mySchema`.

O **ID** será o nome do tipo complexo que armazenará seus dados na instância de recurso estendido.

Depois que uma extensão de esquema é registrada, ela fica disponível para ser usada por todos os aplicativos no mesmo locatário que o aplicativo proprietário associado (quando no estado `InDevelopment`) ou por todos os aplicativos em qualquer locatário (quando no estado `Available`). Assim como as extensões de diretório, os aplicativos autorizados têm a capacidade de ler e gravar dados em quaisquer extensões definidas no objeto de destino.

Ao contrário das extensões abertas, você gerencia as [definições da extensão de esquema](/graph/api/resources/schemaextension) e seus dados na instância de recurso estendido como conjuntos separados de operações de API. Para gerenciar os dados de extensão de esquema na instância de recurso estendido, use a mesma solicitação REST que você usa para gerenciar a instância de recurso.

##### <a name="create-a-schema-extension-definition"></a>Crie uma definição de extensão de esquema

###### <a name="request"></a>Solicitação

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/schemaExtensions

{
    "id": "graphLearnCourses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "user"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

###### <a name="response"></a>Resposta

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#schemaExtensions/$entity",
    "id": "extkmpdyld2_graphLearnCourses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "user"
    ],
    "status": "InDevelopment",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="add-a-schema-extension-to-a-resource-instance"></a>Adicionar uma extensão de esquema a uma instância de recurso

Depois de criar a definição de extensão de esquema, agora você pode adicionar a propriedade de extensão a uma instância de um tipo de objeto de destino. Você pode armazenar dados na extensão de esquema ao criar uma nova instância do objeto de destino ou ao atualizar um objeto existente. O exemplo a seguir mostra como armazenar dados na propriedade de extensão de esquema ao criar um novo objeto de usuário.

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@m365x72712789.onmicrosoft.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": false,
        "password": "xWwvJ]6NMw+bWH-d"
    },
    "extkmpdyld2_graphLearnCourses": {
        "courseId": 100,
        "courseName": "Explore Microsoft Graph",
        "courseType": "Online"
    }
}
```

A solicitação retorna um código de resposta `201 Created` e um objeto [schemaExtension](/graph/api/resources/schemaextension) no corpo da resposta

##### <a name="update-or-delete-a-schema-extension-property"></a>Atualizar ou excluir uma propriedade de extensão de esquema

Use a operação PATCH para atualizar uma propriedade de extensão de esquema ou excluir um objeto de extensão de esquema existente. Para excluir a propriedade de extensão e seu valor associado da instância de recurso, defina seu valor como `null`.

O exemplo a seguir exclui o valor da propriedade **ddingId** e atualiza a propriedade **ddingType**. Para excluir a propriedade de extensão `extkmpdyld2_graphLearnCourses` em sua totalidade, defina seu valor como `null`.

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/users/0668e673-908b-44ea-861d-0661297e1a3e

{
    "extkmpdyld2_graphLearnCourses": {
        "courseType": "Instructor-led",
        "courseId": null
    }
}
```

A solicitação retorna uma resposta `204 No Content`.

##### <a name="retrieve-the-schema-extension-property"></a>Recuperar a propriedade de extensão de esquema

Para ler as propriedades de extensão de esquema em uma instância de recurso, especifique o nome da extensão em uma solicitação `$select`.

###### <a name="request"></a>Solicitação
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/0668e673-908b-44ea-861d-0661297e1a3e?$select=id,displayName,extkmpdyld2_graphLearnCourses
```

###### <a name="response"></a>Resposta
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(id,displayName,extkmpdyld2_graphLearnCourses)/$entity",
    "id": "63384f56-42d2-4aa7-b1d6-b10c78f143a2",
    "displayName": "Adele Vance",
    "extkmpdyld2_graphLearnCourses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseType": "Instructor-led",
        "courseName": "Explore Microsoft Graph",
        "courseId": null
    }
}
```

Para obter mais informações sobre como usar extensões de esquema para adicionar propriedades personalizadas e dados associados, consulte [tipo de recurso schemaExtension](/graph/api/resources/schemextension) e [Adicionar propriedades personalizadas a grupos usando extensões de esquema](extensibility-schema-groups.md).

### <a name="open-extensions"></a>Extensões abertas

[Extensões abertas do Microsoft Graph](/graph/api/resources/opentypeextension) são [tipos abertos](https://www.odata.org/getting-started/advanced-tutorial/#openType) que oferecem uma maneira flexível de adicionar dados de aplicativo não tipados diretamente a uma instância do recurso. Essas extensões não são fortemente tipadas, detectáveis ou filtráveis.

Para obter a lista de tipos de recursos que dão suporte às extensões abertas do Microsoft Graph, consulte [Escolha um tipo de extensão para seu aplicativo](#choose-an-extension-type-for-your-application).

> [!VIDEO https://www.youtube-nocookie.com/embed/ibdlADb8IZc]

#### <a name="developer-experience"></a>Experiência do desenvolvedor

As extensões abertas, juntamente com seus dados, podem ser acessadas por meio da propriedade de navegação **extensions** da instância do recurso. Eles permitem agrupar propriedades relacionadas para facilitar o acesso e o gerenciamento.

A propriedade **extensionName** é a única propriedade *predefinida* gravável em uma extensão aberta. Ao criar uma extensão aberta, você deve atribuir à propriedade **extensionName** um nome exclusivo no locatário. Uma maneira de fazer isso é usar um formato DNS (sistema de nomes de domínio) inverso que seja dependente de *seu próprio domínio*, por exemplo, `Com.Contoso.ContactInfo`. **Não use o domínio Microsoft (`Com.Microsoft` ou`Com.OnMicrosoft`) em um nome de extensão**.

##### <a name="create-an-open-extension"></a>Criar uma extensão aberta

O exemplo a seguir mostra uma definição de extensão aberta com três propriedades e como as propriedades personalizadas e os dados associados são apresentados em uma instância de recurso.

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.socialSettings",
    "skypeId": "skypeId.AdeleV",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile",
    "xboxGamerTag": "AwesomeAdele",
    "id": "com.contoso.socialSettings"
}
```

A solicitação retorna um código de resposta `201 Created` e um objeto [openTypeExtension](/graph/api/resources/opentypeextension) no corpo da resposta.

##### <a name="update-an-existing-open-extension"></a>Atualizar uma extensão aberta existente

Para atualizar uma extensão aberta, você deve especificar todas as suas propriedades no corpo da solicitação. Caso contrário, as propriedades não especificadas serão atualizadas para `null` e excluídas da extensão aberta.

A solicitação a seguir especifica apenas as propriedades **linkedInProfile** e **xboxGamerTag**. O valor da propriedade **xboxGamerTag** está sendo atualizado enquanto a propriedade **linkedInProfile** permanece a mesma. Essa solicitação também exclui a propriedade **skypeId** não especificada.

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions/com.contoso.socialSettings

{
    "xboxGamerTag": "FierceAdele",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile"
}
```
Essa solicitação retorna um código de resposta `204 No Content`.


##### <a name="retrieve-the-open-extensions"></a>Recuperar as extensões abertas

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions/com.contoso.socialSettings

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('3fbd929d-8c56-4462-851e-0eb9a7b3a2a5')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "xboxGamerTag": "FierceAdele",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile",
    "id": "com.contoso.socialSettings"
}
```

Para obter mais informações sobre como usar extensões abertas para adicionar propriedades personalizadas e dados associados, consulte [tipo de recurso openTypeExtension](/graph/api/resources/opentypeextension) e [Adicionar propriedades personalizadas aos usuários que usam extensões abertas](extensibility-open-users.md).

## <a name="choose-an-extension-type-for-your-application"></a>Escolha um tipo de extensão para seu aplicativo

A tabela abaixo contrasta e compara os tipos de extensão, o que deve ajudá-lo a decidir qual opção é mais apropriada para seu cenário.

| Recursos | Atributos de extensão de 1 a 15 | Extensões de diretório | Extensões de esquema | Extensões abertas |
|--|--|--|--|--|
| Tipos de recurso com suporte | [user][] <br/>[device][] | [user][] <br/> [group][] [administrativeUnit][] <br/> [application][] <br/>[device][] <br/> [organization][] | [user][] <br/> [group][] [administrativeUnit][] <br/> [contact][] <br/> [device][] <br/> [event][] (calendários de usuário e grupo) <br/> [message][] <br/> [organização][] <br/> [postagem][] <br/> [todoTask][] <br/> [todoTaskList][] | [user][] <br/> [group][] <!--<br/> [administrativeUnit][]--> <br/> [contact][] <br/> [device][] <br/> [event][]<sup>1</sup> (calendários de usuário e grupo) <br/> [message][] <br/> [organização][] <br/> [postagem][] |
| Fortemente tipado | Não | Sim | Sim | Não |
| Filtráveis | Sim | Sim | Sim | Não |
| Gerenciado por meio de | Microsoft Graph <br/> Centro de administração do Exchange | Microsoft Graph | Microsoft Graph | Microsoft Graph |
| Sincronizar dados do local para extensões usando [o AD Connect][] | Sim, para usuários | Sim | Não | Não |
| Criar [regras de associação dinâmica][] usando dados e propriedades de extensão personalizadas | [Sim][DynamicMembership-YES] | Sim | Não | Não |
| Utilizável para personalizar declarações de token | Sim | Sim | Não | Não |
| Disponível no Azure AD B2C | Sim | [Sim][B2CDirectoryExt] | Sim | Sim |
| Limites | <li>15 atributos predefinidos por instância de recurso de dispositivo ou usuário | <li>100 valores de extensão por instância de recurso | <li>Máximo de cinco definições por aplicativo proprietário <br/><li> 100 valores de extensão por instância de recurso (somente objetos de diretório) | <li>Duas extensões abertas por aplicativo criador por instância de recurso<sup>2</sup> <br/><li> Máx. de 2 Kb por extensão aberta<sup>2</sup><li> Para recursos do Outlook, cada extensão aberta é armazenada em um [Propriedade mapeada MAPI][MAPI-named-property]<sup>3</sup> |


> [!NOTE]
> 
> <sup>1</sup> Devido a uma limitação de serviço existente, os representantes não podem criar eventos abertos acrescentados à extensão em calendários de caixa de correio compartilhados. As tentativas de fazer isso resultarão em uma resposta de `ErrorAccessDenied`.
>
> <sup>2</sup> Esses limites em extensões abertas se aplicam aos seguintes recursos de diretório: **usuário**, **grupo**, **dispositivo**, <!--**administrativeUnit**,--> e **organização**.
>
> <sup>3</sup>Cada [extensão aberta](/graph/api/resources/opentypeextension) é armazenada em uma [propriedade nomeada MAPI](/office/client-developer/outlook/mapi/mapi-named-properties), que é um recurso limitado na caixa de correio de um usuário. Esse limite se aplica aos seguintes recursos do Outlook: **mensagem**, **evento** e **contato**
>
> Você pode gerenciar todas as extensões quando estiver conectado com uma conta corporativa ou de estudante. Além disso, você pode gerenciar extensões abertas para os seguintes recursos quando conectado com uma conta pessoal Microsoft: **evento**, **postagem**, **grupo**, **mensagem**, **contato** e **usuário**.

## <a name="permissions"></a>Permissões

As mesmas [permissões](./permissions-reference.md) necessárias para ler ou gravar um recurso específico também são necessárias para ler ou gravar quaisquer dados de extensões nesse recurso. Por exemplo, para um aplicativo atualizar o perfil de qualquer usuário com dados de aplicativo personalizados, o aplicativo deve ter recebido a permissão *User.ReadWrite.All*.

## <a name="known-limitations"></a>Limitações conhecidas

Nas limitações conhecidas usando extensões, veja a [seção extensões](known-issues.md#extensions) no artigo problemas conhecidos.

## <a name="next-steps"></a>Próximas etapas

- [Adicionar dados personalizados aos usuários usando extensões abertas](extensibility-open-users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](extensibility-schema-groups.md)


<!-- Links -->

[user]: /graph/api/resources/user
[group]: /graph/api/resources/group
[contato]: /graph/api/resources/contact
[administrativeUnit]: /graph/api/resources/administrativeunit
[application]: /graph/api/resources/application
[device]: /graph/api/resources/device
[event]: /graph/api/resources/event
[message]: /graph/api/resources/message
[organização]: /graph/api/resources/organization
[postagem]: /graph/api/resources/post
[todoTask]: /graph/api/resources/todotask
[todoTaskList]: /graph/api/resources/todotasklist
[servicePrincipal]: /graph/api/resources/serviceprincipal
[AD connect]: /azure/active-directory/hybrid/whatis-hybrid-identity?context=/azure/active-directory/enterprise-users/context/ugr-context
[ADConnect-YES]: /azure/active-directory/hybrid/how-to-connect-sync-feature-directory-extensions
[regras de associação dinâmica]: /azure/active-directory/enterprise-users/groups-dynamic-membership
[DynamicMembership-YES]: /azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties
[DirectoryExt-CustomClaims]: /azure/active-directory/develop/active-directory-optional-claims#configuring-directory-extension-optional-claims
[B2CDirectoryExt]: /azure/active-directory-b2c/user-profile-attributes#extension-attributes
[MAPI-named-property]: /office/client-developer/outlook/mapi/mapi-named-properties