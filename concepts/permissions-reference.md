---
title: 'Referência de permissões do Microsoft Graph '
description: O Microsoft Graph expõe as permissões granulares que controlam o acesso que os aplicativos têm aos recursos, como email, grupos e usuários. Como desenvolvedor, você decide quais permissões para o Microsoft Graph seu aplicativo deverá solicitar.
author: jackson-woods
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 67b5398e5e8374e55f54af399d6c045624d8e6cb
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247326"
---
# <a name="microsoft-graph-permissions-reference"></a>Referência de permissões do Microsoft Graph

Para que o aplicativo acesse os dados no Microsoft Graph, o usuário ou administrador deve conceder a ele as permissões corretas por meio de um processo de consentimento. Este tópico lista as permissões associadas a cada grande conjunto de APIs do Microsoft Graph. Ele também fornece orientações sobre como usar as permissões.

[!INCLUDE [auth-use-least-privileged](../includes/auth-use-least-privileged.md)]

Para saber mais sobre como funcionam as permissões, [Confira noções básicas de autenticação e autorização](auth/auth-concepts.md#microsoft-graph-permissions) e assista ao vídeo a seguir.

> [!VIDEO https://www.youtube-nocookie.com/embed/yXYzgWWVdSM]

## <a name="microsoft-graph-permission-names"></a>Nomes de permissões do Microsoft Graph

Os nomes de permissões do Microsoft Graph seguem um padrão simples: _resource.operation.constraint_. Por exemplo, _User.Read_ concede permissão para ler o perfil do usuário conectado, _User.ReadWrite_ concede permissão para ler e modificar o perfil do usuário conectado e _Mail.Send_ concede permissão para enviar emails em nome do usuário conectado.

O elemento _constraint_ do nome determina a extensão potencial do acesso que o aplicativo terá dentro do diretório. No momento, o Microsoft Graph é compatível com as seguintes restrições:

* **Todos** concede permissão para o aplicativo realizar as operações em todos os recursos do tipo especificado em um diretório. Por exemplo, _User.Read.All_ potencialmente concede privilégios ao aplicativo para ler os perfis de todos os usuários em um diretório.
* **Compartilhado** concede permissão para o aplicativo realizar as operações em recursos que outros usuários compartilharam com o usuário conectado. Essa restrição é usada principalmente com recursos como emails, calendários e contatos do Outlook. Por exemplo, _Mail.Read.Shared_ concede privilégios para ler email na caixa de correio do usuário conectado e emails em caixas de correio que outros usuários na organização compartilharam com o usuário conectado.
* **AppFolder** concede permissão para o aplicativo ler e gravar arquivos em uma pasta dedicada no OneDrive. Essa restrição é exposta somente em [Permissões de arquivos](#files-permissions) e só é válida para contas da Microsoft.
* Se **sem restrição** estiver especificado, o aplicativo estará limitado a executar as operações nos recursos pertencentes ao usuário conectado. Por exemplo, _User.Read_ concede privilégios para ler o perfil apenas do usuário conectado e _Mail.Read_ concede permissão para ler apenas os emails na caixa de correio do usuário conectado.

> [!NOTE]
> Em cenários delegados, o acesso de seu aplicativo também é limitado pelos privilégios do usuário conectado. Estes privilégios são determinados pelas funções atribuídas ao usuário e sua relação com os dados que estão sendo acessados.
> Por exemplo, se o usuário assinante não tiver os privilégios apropriados para visualizar um arquivo, então o aplicativo cliente também não poderá ler esse arquivo, mesmo que o aplicativo tenha a `File.Read.All` permissão delegada.

## <a name="microsoft-accounts-and-work-or-school-accounts"></a>Contas da Microsoft e contas corporativas e de estudante

Nem todas as permissões são válidas para contas da Microsoft e contas corporativas ou estudante. Você pode verificar a coluna da **Conta com Suporte da Microsoft** para cada grupo de permissão para determinar se uma permissão específica é válida para contas Microsoft, contas corporativas ou de estudante, ou ambas.

## <a name="limits-on-requested-permissions-per-app"></a>Limites de permissões solicitadas por aplicativo

O Azure AD limita o número de permissões que podem ser solicitadas e consentidas por um aplicativo cliente. Esses limites dependem do valor `signInAudience` do aplicativo, mostrado no manifesto do aplicativo. 

| signInAudience                     | Usuários permitidos                                            | Máximo de permissões que o aplicativo pode solicitar   | Máximo de permissões do Microsoft Graph que o aplicativo pode solicitar   | Máximo de permissões que podem ser consentidas em uma única solicitação         |
| ---------------------------------- | -------------------------------------------------------- | ----------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------------------- |
| AzureADMyOrg                       | Usuários da organização em que o aplicativo está registrado  | 400                                       | 400                                                       | Cerca de 155 permissões delegadas e cerca de 300 permissões de aplicativo |
| AzureADMultipleOrgs                | Usuários de qualquer organização do Azure AD                     | 400                                       | 400                                                       | Cerca de 155 permissões delegadas e cerca de 300 permissões de aplicativo |
| PersonalMicrosoftAccount           | Usuários consumidores (como contas do Outlook.com ou Live.com)  | 30                                        | 30                                                        | 30                                                                    |
| AzureADandPersonalMicrosoftAccount | Usuários e usuários consumidores de qualquer organização do Azure AD  | 30                                        | 30                                                        | 30                                                                    |

## <a name="permissions-availability-status"></a>Status de disponibilidade de permissões

As permissões do Microsoft Graph no [portal do Azure](https://portal.azure.com/) geralmente estão disponíveis e no status DG para todos os aplicativos usarem, exceto alguns conjuntos que estão no status de visualização ou visualização privada. As permissões na visualização estão disponíveis para o público; elas podem mudar e podem não ser promovidas ao status DG. As permissões no status de visualização privada não estão disponíveis e talvez nunca sejam disponibilizadas ao público. Não use as permissões no status de visualização ou visualização privada em aplicativos de produção.

## <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>Limitações de pesquisa de usuário e grupo para usuários convidados em organizações

Os recursos de pesquisa de usuário e grupo permitem que o aplicativo pesquise qualquer usuário ou grupo no diretório de uma organização, executando consultas no conjunto de recursos `/users` ou `/groups` (por exemplo, `https://graph.microsoft.com/v1.0/users`). Tanto administradores quanto usuários têm esse recurso; no entanto, os usuários convidados não.

Se o usuário conectado for um usuário convidado, dependendo das permissões que recebeu um aplicativo, ele pode ler o perfil de um usuário específico ou grupo (por exemplo, `https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`). No entanto, o usuário não pode executar consultas no conjunto de recursos `/users` ou `/groups` que, potencialmente, retornam mais de um recurso.

Com as permissões apropriadas, o aplicativo pode ler os perfis de usuários ou grupos que ele obtém seguindo os links nas propriedades de navegação. Por exemplo, `/users/{id}/directReports` ou `/groups/{id}/members`.

## <a name="limited-information-returned-for-inaccessible-member-objects"></a>Informações limitadas retornadas para objetos membro inacessíveis

Objetos de contêiner, como grupos, oferecem suporte a membros de vários tipos; por exemplo, usuários e dispositivos. Quando um aplicativo consulta a associação de um objeto contêiner e não tem permissão para ler um determinado tipo, os membros desse tipo são retornados, mas com informações limitadas.  O aplicativo recebe umas 200 respostas e uma coleção de objetos.  Informações completas são retornadas para os tipos de objetos que o aplicativo tem permissões para ler.  Para os tipos de objetos que o aplicativo não tem permissão para ler, apenas o tipo e a ID do objeto são retornados.

Isso é aplicado a todos as relações que são do tipo [directoryObject](/graph/api/resources/directoryobject) (não apenas aos links de membro). Exemplos incluem `/groups/{id}/members`, `/users/{id}/memberOf`, ou `me/ownedObjects`.

Por exemplo, digamos que um aplicativo tenha as permissões de [User.Read.All](#user-permissions) e [Group.Read.All](#group-permissions) do Microsoft Graph.  Um grupo foi criado e esse grupo contém um usuário, um grupo e um dispositivo.  O aplicativo chama aos [membros do grupo de listas](/graph/api/group-list-members).  O aplicativo tem acesso aos objetos de usuário e grupo no grupo, mas não ao objeto do dispositivo.  Na resposta, todas as propriedades selecionadas dos objetos de usuário e grupo são retornadas. No entanto, para o objeto de dispositivo, apenas as informações limitadas são retornadas.  O tipo de dados e a ID do objeto são retornados para o dispositivo, mas todas as outras propriedades têm um valor *nulo*. Os aplicativos sem permissão não poderão usar a ID para obter o objeto real.

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members?$select=id,displayName,description,createdDateTime,deletedDateTime,homepage,loginUrl HTTP/1.1
```

Segue a resposta de JSON:

```json
{
"@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects(id,displayName,description,createdDateTime,deletedDateTime,homepage,loginUrl)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.user",
            "id":"69d035a3-29c9-469f-809d-d21a4ae69e65",
            "displayName":"Jane Dane",
            "createdDateTime":"2019-09-18T09:06:51Z",
            "deletedDateTime":null
        },
        {
            "@odata.type":"#microsoft.graph.group",
            "id":"c43a7cc9-2d95-44b6-bf6a-6392e41949b4",
            "displayName":"Group 1",
            "description":null,
            "createdDateTime":"2019-10-24T01:34:35Z",
            "deletedDateTime":null
        },
        {
            "@odata.type":"#microsoft.graph.device",
            "id": "d282309e-f91d-43b6-badb-9e68aa4b4fc8",
            "accountEnabled":null,
            "deviceId":null,
            "displayName":null,
            "operatingSystem":null,
            "operatingSystemVersion":null
        }
    ]
}
```

## <a name="access-reviews-permissions"></a>Permissões de revisões de acesso

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _AccessReview.Read.All_ |   Ler todas as revisões de acesso  | Permite que o aplicativo leia as revisões de acesso em nome do usuário conectado. | Sim | Não |
| _AccessReview.ReadWrite.All_ |   Gerenciar todas as revisões de acesso  | Permite que o aplicativo leia e grave revisões de acesso em nome do usuário conectado. | Sim | Não |
| _AccessReview.ReadWrite.Membership_ |   Gerenciar revisões de acesso para participações em grupo e aplicativos | Permite que o aplicativo leia e grave revisões de acesso de grupos e aplicativos em nome do usuário conectado. | Sim | Não |



#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _AccessReview.Read.All_ |   Ler todas as revisões de acesso | Permite que o aplicativo leia revisões de acesso sem um usuário conectado. | Sim |
| _AccessReview.ReadWrite.All_ |   Gerenciar todas as revisões de acesso | Permite que o aplicativo leia, atualize, exclua e execute ações nas revisões de acesso, revisores, decisões e configurações na organização, sem um usuário conectado. | Sim |
| _AccessReview.ReadWrite.Membership_ | Gerenciar revisões de acesso para participações em grupo e aplicativos | Permite que o aplicativo gerencie o acesso a revisões de aplicativos e grupos sem um usuário conectado. | Sim |


### <a name="remarks"></a>Comentários

_AccessReview.Read.All_, _AccessReview.ReadWrite.All_, _AccessReview.ReadWrite.Membership_ são válidos apenas para contas corporativas ou de estudante.

Para um aplicativo com permissões delegadas para ler as revisões de acesso de um grupo ou aplicativo, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador Global, Administrador de Segurança, Leitor de Segurança ou Administrador de Usuários. Para um aplicativo com permissões delegadas para gravar revisões de acesso de um grupo ou aplicativo, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador Global ou Administrador de Usuários.

Para um aplicativo com permissões delegadas para ler revisões de acesso de uma função do Azure AD, o usuário conectado deve ser um membro de uma das seguintes funções de administrador: Administrador Global, Administrador de Segurança, Leitor de Segurança ou Administrador de Função Privilegiada. Para um aplicativo com permissões delegadas para gravar revisões de acesso de uma função do Azure AD, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador Global ou Administrador de Função Privilegiada.

Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

---

## <a name="administrative-units-permissions"></a>Permissões de unidades administrativas

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _AdministrativeUnit.Read.All_ |   Ler unidades administrativas  | Permite que o aplicativo leia as unidades administrativas e a associação de unidade administrativa em nome do usuário conectado. | Sim | Não |
| _AdministrativeUnit.ReadWrite.All_ |   Ler e gravar unidades administrativas  | Permite que o aplicativo crie, leia, atualize e exclua unidades administrativas e gerencie a associação de unidade administrativa em nome do usuário conectado. | Sim | Não |


#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _AdministrativeUnit.Read.All_ |   Ler todas as unidades administrativas | Permite que o aplicativo leia as unidades administrativas e a associação de unidade administrativa sem um usuário conectado. | Sim |
| _AdministrativeUnit.ReadWrite.All_ |   Ler e gravar todas as unidades administrativas | Permite que o aplicativo crie, leia, atualize e exclua as unidades administrativas e gerencie a participação em unidades administrativas sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários
Com a permissão _AdministrativeUnit.Read.All_ um aplicativo pode ler informações sobre a unidade administrativa, incluindo membros. 

Com a permissão _AdministrativeUnit.Read.All_ um aplicativo pode cria, ler, atualizar e deletar informações sobre a unidade administrativa, incluindo membros. 

_AdministrativeUnit.Read.All_ e _AdministrativeUnit. ReadWrite.All_ só são válidos para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

> [!NOTE]
> O `v1.0` ponto de extremidade para a API de unidades administrativas é `/v1.0/directory/administrativeUnits`.

- _AdministrativeUnit.Read.All_: Ler unidades administrativas (`GET /beta/administrativeUnits`)
- _AdministrativeUnit.Read.All_: Ler lista de membros de uma unidade administrativa (`GET /beta/administrativeUnits/<id>/members`)
- _AdministrativeUnit.ReadWrite.All_: Criar uma unidade administrativa (`POST /beta/administrativeUnits`)
- _AdministrativeUnit.ReadWrite.All_: Atualizar uma unidade administrativa (`PATCH /beta/administrativeUnits/<id>`)
- _AdministrativeUnit.ReadWrite.All_: Adicionar membros a uma unidade administrativa (`POST /beta/administrativeUnits/<id>/members`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="analytics-resource-permissions"></a>Permissões de recurso do Analytics

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Analytics.Read_ |   Leia as estatísticas das atividades do usuário. | Permite que o aplicativo leia as estatísticas das atividades do usuário conectado, como quanto tempo o usuário gastou em e-mails, em reuniões ou em sessões de chat. | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

Nenhuma.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Analytics.Read_: [Listar as configurações relacionadas para um usuário](/graph/api/useranalytics-get-settings?view=graph-rest-beta&preserve-view=true) (`GET /beta/me/analytics/settings`)

#### <a name="application"></a>Application

Nenhum

---

## <a name="appcatalog-resource-permissions"></a>Permissões de recurso AppCatalog

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Conta da Microsoft necessária |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------| :----------|
| _AppCatalog.Read.All_ | Ler todos os catálogos de aplicativos | Permite que o aplicativo leia os aplicativos no catálogo de aplicativos.| Não | Não |
| _AppCatalog.ReadWrite.All_ | Ler e gravar em todos os catálogos de aplicativo  | Permite que o aplicativo crie, leia, atualize e exclua aplicativos nos catálogos do aplicativo. | Sim | Não |
|_AppCatalog.Submit_|Envie um aplicativo para análise do administrador|Permite que o usuário envie um aplicativo para revisão do administrador para publicação no catálogo de aplicativos de uma organização e permite que o usuário cancele envios anteriores que não foram publicados.</br> &#119821;&#119822;&#119827;&#119812;: Usuários não administradores enviam aplicativos para revisão incluindo o parâmetro de consulta `requiresReview=true`.|Sim|Não|

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _AppCatalog.Read.All_ | Ler todos os catálogos de aplicativos | Permite que o aplicativo leia aplicativos nos catálogos de aplicativos sem um usuário conectado. | Sim |
| _AppCatalog.ReadWrite.All_ | Ler e gravar em todos os catálogos de aplicativo | Permite que o aplicativo crie, leia, atualize e exclua aplicativos nos catálogos de aplicativos sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

No momento o único catálogo é a lista de aplicativos no [Microsoft Teams](teams-concept-overview.md).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegated
* _AppCatalog.ReadWrite.All_: [Lista todos os aplicativos no catálogo](/graph/api/appcatalogs-list-teamsapps) (`GET /beta/appCatalogs/teamsApps`)
* _AppCatalog.ReadWrite.All_: [Publicar um aplicativo](/graph/api/teamsapp-publish?view=graph-rest-beta&preserve-view=true) (`POST /beta/appCatalogs/teamsApps`)
* _AppCatalog.ReadWrite.All_: [Atualizar um aplicativo publicado](/graph/api/teamsapp-update?view=graph-rest-beta&preserve-view=true) (`PATCH /beta/appCatalogs/teamsApps/{id}`)
* _AppCatalog.ReadWrite.All_: [Remover um aplicativo publicado](/graph/api/teamsapp-delete?view=graph-rest-beta&preserve-view=true) (`DELETE /beta/appCatalogs/teamsApps/{id}`)

#### <a name="application"></a>Aplicativo

Nenhum.

---

## <a name="application-resource-permissions"></a>Permissões de recursos de aplicação

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Application.Read.All_ | Ler aplicativos | Permite que o aplicativo leia aplicativos e entidades de serviço em nome do usuário conectado. | Sim |
| _Application.ReadWrite.All_ | Ler e gravar todos os aplicativos |  Permite que o aplicativo crie, leia, atualize e exclua aplicativos e entidades de serviço em nome do usuário conectado. | Sim |
| _AppRoleAssignment.ReadWrite.All_ | Gerenciar concessões de permissão de aplicativo e atribuições de função de aplicativo | Permite que o aplicativo gerencie concessões de permissão para permissões de aplicativos para qualquer API (incluindo o Microsoft Graph) e atribuições de aplicativos para qualquer aplicativo, em nome do usuário conectado. | Sim |
| _DelegatedPermissionGrant.ReadWrite.All_ | Gerenciar concessões de permissão delegadas | Permite que o aplicativo gerencie concessões de permissão para permissões de representante expostas por qualquer API (incluindo o Microsoft Graph), em nome do usuário conectado. | Sim |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Application.Read.All_ | Ler aplicativos | Permite que o aplicativo leia aplicativos e entidades de serviço sem um usuário conectado. | Sim |
| _Application.ReadWrite.All_ | Ler e gravar todos os aplicativos | Permite que o aplicativo de chamada crie e gerencie (leia, atualize, atualize segredos do aplicativo e exclua) aplicativos e serviços sem um usuário conectado.  Não permite o gerenciamento de concessões de autorizações ou atribuições de aplicativos a usuários ou grupos. | Sim |
| _Application.ReadWrite.OwnedBy_ | Gerenciar aplicativos que este aplicativo criar ou possuir | Permite que o aplicativo de chamada crie outros aplicativos e entidades de serviço, e gerencie completamente esses aplicativos e entidades de serviço (leia, atualize, atualize os segredos do aplicativo e exclua), sem um usuário conectado.  Ele não poderá atualizar os aplicativos que não pertencem a ele. Não permite o gerenciamento de concessões de autorizações ou atribuições de aplicativos a usuários ou grupos. | Sim |
| _AppRoleAssignment.ReadWrite.All_ | Gerenciar concessões de permissão de aplicativo e atribuições de função de aplicativo | Permite que o aplicativo gerencie concessões de permissão para permissões de aplicativos para qualquer API (incluindo o Microsoft Graph) e atribuições de aplicativos para qualquer aplicativo, sem um usuário conectado. | Sim |
| _DelegatedPermissionGrant.ReadWrite.All_ | Gerenciar todas as concessões de permissão de representante | Permite que o aplicativo conceda ou revogue qualquer permissão delegada para qualquer API (incluindo Microsoft Graph), sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

> [!CAUTION]
> Permissões que permitem conceder autorização, tais como _ApproleAssignment.readwrite.all_, permitem que um aplicativo conceda privilégios adicionais a si mesmo, a outros aplicativos ou a qualquer usuário. Da mesma forma, as permissões que permitem o gerenciamento de credenciais, tais como _application.readwrite.all_, permitem que um aplicativo atue como outras entidades e use os privilégios que lhes foram concedidos. Tenha cuidado ao conceder qualquer uma dessas permissões.

A permissão _Application.ReadWrite.OwnedBy_ permite as mesmas operações que _Application.ReadWrite.All_, exceto que a primeira permite essas operações apenas em aplicativos e entidades de serviço dos quais o aplicativo de chamada é proprietário. A propriedade é indicada pela `owners` propriedade de navegação no [aplicativo](/graph/api/application-list-owners?view=graph-rest-beta&preserve-view=true) de destino ou no recurso [principal de serviço](/graph/api/serviceprincipal-list-owners?view=graph-rest-beta&preserve-view=true).
> OBSERVAÇÃO: o uso da permissão _Application.ReadWrite.OwnedBy_ para chamar `GET /applications` para listar aplicativos falhará com um erro 403.  Use `GET servicePrincipals/{id}/ownedObjects` para listar os aplicativos que pertencem ao aplicativo da chamada.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Application.Read.All_: listar todos os aplicativos (`GET /v1.0/applications`)
* _Application.ReadWrite.All_: atualizar uma entidade de serviço (`PATCH /v1.0/servicePrincipals/{id}`)

#### <a name="application"></a>Aplicativo

* _Application.Read.All_: listar todos os aplicativos (`GET /v1.0/applications`)
* _Application.ReadWrite.All_: excluir uma entidade de serviço (`DELETE /v1.0/servicePrincipals/{id}`)
* _Application.ReadWrite.OwnedBy_: criar um aplicativo (`POST /v1.0/applications`)
* _Application.ReadWrite.OwnedBy_: Listar todos os aplicativos pertencentes ao aplicativo da chamada (`GET /v1.0/servicePrincipals/{id}/ownedObjects`)
* _Application.ReadWrite.OwnedBy_: adicionar outro proprietário a um aplicativo próprio (`POST /v1.0/applications/{id}/owners/$ref`).
    > OBSERVAÇÃO: isso pode exigir permissões adicionais.

---

## <a name="audit-log-permissions"></a>Permissões de log de auditoria

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _AuditLog.Read.All_ | Ler dados de log de auditoria | Permite que o aplicativo leia e consulte suas atividades de log de auditoria, em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_AuditLog.Read.All_ |Ler todos os dados do log de auditoria |Permite que o aplicativo leia e consulte suas atividades de log de auditoria, sem um usuário conectado. |Sim |

---

## <a name="bitlocker-recovery-key-permissions"></a>Permissões da chave de recuperação do BitLocker

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _BitlockerKey.ReadBasic.All_ | Ler as informações básicas das chaves do BitLocker | Permite que um aplicativo leia as propriedades da chave do BitLocker para todos os dispositivos no locatário. A chave de recuperação não é retornada. | Sim | Não |
| _BitlockerKey.Read.All_ | Ler a chave do BitLocker | Permite que um aplicativo leia as propriedades da chave do BitLocker para todos os dispositivos no locatário. A chave de recuperação é retornada. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

Nenhuma.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _BitlockerKey.ReadBasic.All_: Listar as chaves de recuperação do BitLocker para todos os dispositivos no locatário sem retornar a propriedade 'key' (`GET /bitlocker/recoveryKeys`).
* _BitlockerKey.Read.All_: Obter uma chave de recuperação do BitLocker com a chave de recuperação (`GET /bitlocker/recoveryKeys/{bitlockerRecoveryKeyId}?$select=key`)

---

## <a name="bookings-permissions"></a>Permissões do Bookings

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Bookings.Read.All_ |  Permite que um aplicativo leia compromissos, empresas, clientes, serviços e funcionários do Bookings em nome do usuário conectado. | Destinados a aplicativos somente leitura. O usuário-alvo típico é o cliente de uma empresa de reservas. | Não | Não |
| _BookingsAppointment.ReadWrite.All_ | Permite que um aplicativo leia e grave compromissos e clientes do Bookings, permitindo também a leitura de empresas, serviços e funcionários em nome do usuário conectado. | Desenvolvido para aplicativos de agendamento que precisam manipular compromissos e clientes. Não pode alterar informações fundamentais sobre a empresa de reservas, nem seus serviços e funcionários. O usuário-alvo típico é o cliente de uma empresa de reservas.| Não | Não |
| _Bookings.ReadWrite.All_ | Permite que um aplicativo leia e grave compromissos, empresas, clientes, serviços e funcionários do Bookings em nome do usuário conectado. Não permite criar, excluir ou publicar de empresas do Bookings. | Voltado a aplicativos de gerenciamento que manipulam empresas existentes, seus serviços e seus funcionários. Não pode criar, excluir ou alterar o status de publicação de uma empresa de reservas. O usuário-alvo típico é o funcionário de suporte de uma organização.| Não | Não |
| _Bookings.Manage.All_ | Permite que um aplicativo leia, grave e gerencie compromissos, empresas, clientes, serviços e funcionários do Bookings em nome do usuário conectado.  | Permite que o aplicativo tenha acesso total. <br>Voltado a uma experiência de gerenciamento completa. O usuário-alvo típico é o administrador de uma organização.| Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Bookings.Read.All_ |  Permite que um aplicativo leia compromissos, empresas, clientes, serviços e funcionários do Bookings em nome do usuário conectado. | Destinados a aplicativos somente leitura. O usuário-alvo típico é o cliente de uma empresa de reservas. | Não | Não |
| _BookingsAppointment.ReadWrite.All_ | Permite que um aplicativo leia e grave compromissos e clientes do Bookings, permitindo também a leitura de empresas, serviços e funcionários em nome do usuário conectado. | Desenvolvido para aplicativos de agendamento que precisam manipular compromissos e clientes. Não pode alterar informações fundamentais sobre a empresa de reservas, nem seus serviços e funcionários. O usuário-alvo típico é o cliente de uma empresa de reservas.| Não | Não |
| _Bookings.ReadWrite.All_ | Permite que um aplicativo leia e grave compromissos, empresas, clientes, serviços e funcionários do Bookings em nome do usuário conectado. Não permite criar, excluir ou publicar de empresas do Bookings. | Voltado a aplicativos de gerenciamento que manipulam empresas existentes, seus serviços e seus funcionários. Não pode criar, excluir ou alterar o status de publicação de uma empresa de reservas. O usuário-alvo típico é o funcionário de suporte de uma organização.| Não | Não |
| _Bookings.Manage.All_ | Permite que um aplicativo leia, grave e gerencie compromissos, empresas, clientes, serviços e funcionários do Bookings em nome do usuário conectado.  | Permite que o aplicativo tenha acesso total. <br>Voltado a uma experiência de gerenciamento completa. O usuário-alvo típico é o administrador de uma organização.| Não | Não |

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Bookings.Read.All_: obter a ID e os nomes do conjunto de empresas do Bookings que foi criado para um locatário (`GET /bookingBusinesses`).
* _BookingsAppointment.ReadWrite.All_: criar um compromisso para um serviço em uma empresa de reservas (`POST /bookingBusinesses/{id}/appointments`).
* _Bookings.ReadWrite.All_: criar um novo serviço para as empresas especificadas de reservas (`POST /bookingBusinesses/{id}/services`).
* _Bookings.Manage.All_: disponibilizar a página de agendamento dessa empresa para clientes externos (`POST /bookingBusinesses/{id}/publish`).

## <a name="calendars-permissions"></a>Permissões de calendários

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Calendars.Read_ |Ler calendários do usuário |Permite ao aplicativo ler eventos nos calendários do usuário. |Não | Sim |
| _Calendars.Read.Shared_ |Ler usuários e calendários compartilhados |Permite que o aplicativo leia os eventos em todos os calendários a que o usuário tem acesso, incluindo os delegados e os calendários compartilhados. |Não | Não |
| _Calendars.ReadWrite_ |Ter acesso total aos calendários do usuário |Permite ao aplicativo criar, ler, atualizar e excluir eventos em calendários do usuário. |Não | Sim |
| _Calendars.ReadWrite.Shared_ |Ler e registrar usuário e calendários compartilhados |Permite ao aplicativo criar, ler, atualizar e excluir eventos de todos os calendários que o usuário tenha permissão para acessar. Isso inclui o delegado e os calendários compartilhados.|Não | Não |

<br/>

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Calendars.Read_ |Ler calendários em todas as caixas de correio |Permite ao aplicativo ler eventos de todos os calendários sem um usuário conectado. |Sim |
|_Calendars.ReadWrite_ |Ler e gravar calendários em todas as caixas de correio |Permite ao aplicativo criar, ler, atualizar e excluir eventos de todos os calendários sem um usuário conectado. |Sim |

> Os Administradores **Importantes** podem configurar a [política de acesso ao aplicativo](auth-limit-mailbox-access.md) para limitar o acesso do aplicativo às caixas de correio _específicas_ e não a todas as caixas de correio na organização, mesmo que as permissões de aplicativo do Calendars.Read ou Calendars.ReadWrite sejam concedidas ao aplicativo. 
<br/>

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Calendars.Read_: Obter eventos do calendário do usuário entre 23 de abril de 2017 e 29 de abril de 2017 (`GET /me/calendarView?startDateTime=2017-04-23T00:00:00&endDateTime=2017-04-29T00:00:00`).
* _Calendars.Read.Shared_: Encontrar horários de reuniões onde todos os participantes estejam disponíveis (`POST /users/{id|userPrincipalName}/findMeetingTimes`).
* _Calendars.ReadWrite_: Adicionar um evento ao calendário do usuário (`POST /me/events`).

#### <a name="application"></a>Aplicativo

* _Calendars.Read_: Localizar eventos do calendário de uma sala de conferências organizado por pedro@contoso.com (`GET /users/{id | userPrincipalName}/events?$filter=organizer/emailAddress/address eq 'bob@contoso.com'`).
* _Calendars.Read_: Listar todos os eventos do mês de maio do calendário de um usuário (`GET /users/{id | userPrincipalName}/calendarView?startDateTime=2017-05-01T00:00:00&endDateTime=2017-06-01T00:00:00`)
* _Calendars.ReadWrite_: Adicionar um evento de folga aprovada (`POST /users/{id | userPrincipalName}/events`) ao calendário de um usuário.

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

## <a name="calls-permissions"></a>Permissões de chamadas

#### <a name="delegated-permissions"></a>Permissões delegadas

Nenhum.

<br/>

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Calls.Initiate.All_|Iniciar chamadas de saída 1:1 a partir do aplicativo|Permite que o aplicativo faça chamadas de saída para um único usuário e transfira chamadas para usuários no diretório da sua organização, sem um usuário conectado.|Sim|
|_Calls.InitiateGroupCall.All_|Iniciar chamadas de saída em grupo a partir do aplicativo|Permite que o aplicativo faça chamadas para vários usuários e adicione participantes a reuniões em sua organização, sem um usuário conectado.|Sim|
|_Calls.JoinGroupCall.All_|Ingressar em reuniões e chamadas de grupo como um aplicativo|Permite que o aplicativo ingresse em reuniões agendadas e chamadas de grupo em sua organização, sem um usuário conectado. O aplicativo será associado aos privilégios de um usuário do diretório para reuniões em seu locatário.|Sim|
|_Calls.JoinGroupCallasGuest.All_|Ingressar em reuniões e chamadas de grupo como um convidado|Permite que o aplicativo ingresse anonimamente no grupo chamadas e em reuniões agendadas em sua organização, sem um usuário conectado. O aplicativo ingressará como convidado para reuniões em seu locatário.|Sim|
|_Calls.AccessMedia.All_\*|Acessar fluxos de mídia em uma chamada como um aplicativo|Permite que o aplicativo obtenha acesso direto aos fluxos de mídia em uma chamada sem um usuário conectado.|Sim|

> \***Importante:** NÃO é possível usar as APIs de comunicações na nuvem para gravar ou persistir o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia. Certifique-se de que você está em conformidade com as leis e regulamentações de sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

<br/>

### <a name="example-usage"></a>Exemplo de uso

#### <a name="application"></a>Aplicativo

* _Calls.Initiate.All_: fazer uma chamada de ponto a ponto do aplicativo para um usuário na organização (`POST /beta/communications/calls`).
* _Calls.InitiateGroupCall.All_: Faça uma chamada em grupo do aplicativo para um grupo de usuários na organização (`POST /beta/communications/calls`).
* _Calls.JoinGroupCall.All_: ingressar em uma chamada de grupo ou em uma reunião online do aplicativo (`POST /beta/communications/calls`).
* _Calls.JoinGroupCallasGuest.All_: Ingresse em uma chamada de grupo ou em uma reunião online do aplicativo, mas o aplicativo só tem privilégios de convidado na reunião (`POST /beta/communications/calls`).
* _Calls.AccessMedia.All_: criar ou ingressar em uma chamada e o aplicativo é o acesso direto aos fluxos de participantes de mídia na chamada (`POST /beta/communications/calls`).

> **Observação:** para obter exemplos solicitação, confira [Criar chamada](/graph/api/application-post-calls?view=graph-rest-beta&preserve-view=true).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

## <a name="call-records-permissions"></a>Permissões dos registros de chamadas

#### <a name="delegated-permissions"></a>Permissões delegadas

Nenhum.

<br/>

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_CallRecords.Read.All_|Ler todos os registros de chamadas|Permite que o aplicativo leia registros de chamadas de todas as chamadas e reuniões on-line sem um usuário conectado.|Sim|
|_CallRecord-PstnCalls.Read.All_|Ler PSTN e dados de log de chamadas de roteamento direto|Permite que o aplicativo leia todos os dados de registro de chamadas PSTN e roteamento direto sem um usuário conectado.|Sim|

### <a name="remarks"></a>Comentários

A permissão _CallRecords.Read.All_ concede a um aplicativo acesso privilegiado ao [callRecords](/graph/api/resources/callrecords-callrecord) para todas as chamadas e reuniões online dentro da organização, incluindo chamadas de e para números de telefone externos. Isso inclui detalhes potencialmente confidenciais sobre quem participou da chamada, bem como informações técnicas referentes a essas chamadas e reuniões, que podem ser usadas para solucionar problemas de rede, como endereços IP, detalhes do dispositivo e outras informações de rede.

A permissão _CallRecord-PstnCalls.Read.All_ concede a um aplicativo acesso a [PSTN (planos de chamadas)](/graph/api/callrecords-callrecord-getpstncalls) e registros de chamadas de [roteamento direto](/graph/api/callrecords-callrecord-getdirectroutingcalls). Isso inclui informações potencialmente confidenciais sobre os usuários, bem como chamadas de e para números de telefone externos.

> **Importante:** A discrição deve ser usada ao conceder essas permissões aos aplicativos. Os registros de chamadas podem fornecer informações sobre a operação de seus negócios e, portanto, podem ser um alvo para agentes mal-intencionados. Conceda essas permissões apenas aos aplicativos em que você confia para atender aos seus requisitos de proteção de dados.

> **Importante:** certifique-se de que está em conformidade com as leis e regulamentos da sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

<br/>

### <a name="example-usage"></a>Exemplo de uso

#### <a name="application"></a>Aplicativo

* _CallRecords.Read.All_: recuperar um registro de chamada (`GET /v1.0/communications/callRecords/{id}`).
* _CallRecords.Read.All_: assinar novos registros de chamadas (`POST /v1.0/subscriptions`).
* _CallRecords.Read.All_: recuperar os registros de chamadas de roteamento direto no intervalo de tempo especificado (`GET /v1.0/communications/callRecords/microsoft.graph.callRecords.getDirectRoutingCalls(fromDateTime={start date and time),toDateTime={end date and time))`)
* _CallRecord-PstnCalls.Read.All_: recupera registros de chamadas PSTN dentro do intervalo de tempo especificado (`GET /v1.0/communications/callRecords/microsoft.graph.callRecords.getPstnCalls(fromDateTime={start date and time),toDateTime={end date and time))`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

## <a name="channel-permissions"></a>Permissões de canal

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Channel.ReadBasic.All_ | Ler os nomes e descrições dos canais. | Ler os nomes e as descrições dos canais, em nome do usuário conectado.    | Não | Não |
| _Channel.Create_ | Criar canais. | Criar canais em qualquer equipe, em nome do usuário conectado.   | Sim | Não |
| _Channel.Delete.All_ | Excluir canais. | Excluir os canais de qualquer equipe, em nome do usuário conectado.   | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Channel.ReadBasic.All_ | Ler os nomes e as descrições de todos os canais. | Ler todos os nomes e descrições do canal, sem um usuário conectado.  | Sim | Não |
| _Channel.Create_ | Criar canais. | Criar canais em qualquer equipe, sem um usuário conectado.  | Sim | Não |
| _Channel.Delete.All_ | Excluir canais. | Excluir os canais de qualquer equipe, sem um usuário conectado.  | Sim | Não |
|_Teamwork.Migrate.All_|Gerenciar a migração do Microsoft Teams|Criar e gerenciar recursos de migração do Microsoft Teams|Sim|Sim|

## <a name="channel-member-permissions"></a>Permissões de membro do canal

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMember.Read.All_  |Leia os membros dos canais. |Leia os membros dos canais em nome do usuário conectado. |Sim | Não |
|_ChannelMember.ReadWrite.All_ | Adicione e remova membros dos canais.| Adicione e remova membros dos canais em nome do usuário conectado. Também permite alterar a função de um membro. Por exemplo: de proprietário para não proprietário.| Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMember.Read.All_ |Leia os membros dos canais. |Leia os membros dos canais sem um usuário conectado. |Sim | Não |
|_ChannelMember.ReadWrite.All_ |Adicione e remova membros dos canais.|Adicione e remova membros dos canais sem um usuário conectado. Também permite alterar a função de um membro. Por exemplo: de proprietário para não proprietário.| Sim | Não |

## <a name="channel-message-permissions"></a>Permissões de mensagem de canal

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMessage.Edit_ (visualização privada)|Editar mensagens de canal do usuário |Permite que um aplicativo edite mensagens de canal no Microsoft Teams, em nome do usuário conectado. |Sim | Não |
|_ChannelMessage.Read.All_ |Ler mensagens do canal do usuário  |Permite que um aplicativo leia as mensagens de um canal no Microsoft Teams, em nome do usuário conectado. |Sim | Não |
|_ChannelMessage.Send_ |Enviar a mensagem do canal |Permite que um aplicativo envie mensagens de canal no Microsoft Teams, em nome do usuário conectado. |Não| Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMessage.Read.All_ |Listar mensagens do canal  |Permite que um aplicativo leia todas as mensagens de canal do Microsoft Teams, sem um usuário conectado. |Sim | Não |
|_ChannelMessage.UpdatePolicyViolation.All_ |Sinalizar mensagens de canal para a política de violação |Permite que o aplicativo atualize as mensagens do canal do Microsoft Teams, aplicando um conjunto de propriedades de violação da política de prevenção contra perda de dados (DLP) para controlar a saída de processamento DLP. | Sim | Não |

> **Observação:** consulte também [Group. Read. All](#group-permissions).

## <a name="channel-settings-permissions"></a>Permissões de configurações de canal 

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChannelSettings.Read.All_ | Ler os nomes, descrições e configurações dos canais. | Ler todos os nomes, descrições e configurações dos canais, em nome do usuário conectado.| Sim | Não |
| _ChannelSettings.ReadWrite.All_ | Ler e gravar os nomes, descrições e configurações dos canais. | Ler e gravar os nomes, descrições e configurações de todos os canais, em nome do usuário conectado.| Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChannelSettings.Read.All_ | Ler os nomes, descrições e configurações de todos os canais. | Ler todos os nomes, descrições e configurações do canal, sem um usuário conectado.| Sim | Não |
| _ChannelSettings.ReadWrite.All_ | Ler e gravar os nomes, descrições e configurações de todos os canais. | Ler e gravar os nomes, descrições e configurações de todos os canais, sem um usuário conectado.| Sim | Não |

## <a name="chat-permissions"></a>Permissões de chat

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Chat.Read_ |Ler suas mensagens de bate-papo  |Permite que um aplicativo leia, em seu nome, suas mensagens de bate-papo de um para um ou de grupo no Microsoft Teams. |Não | Não |
|_Chat.ReadBasic_ |Ler nomes e membros de threads de chat do usuário  |Permite que um aplicativo leia os membros e as descrições de threads de chat individuais e de grupo, em nome do usuário conectado. |Não | Não |
|_Chat.ReadWrite_ |Leia as suas mensagens de chat e envie novas mensagens   |Permite que um aplicativo leia e envie, em seu nome, suas mensagens de chat individual ou em grupo no Microsoft Teams. |Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Chat.Read.All_ |Ler todas as mensagens de bate-papo  |Permite que um aplicativo leia, sem um usuário conectado, suas mensagens de bate-papo de um para um ou de grupo no Microsoft Teams. |Sim | Não |
|_Chat.ReadBasic.All_ |Ler nomes e membros de threads de chat do usuário  |Ler nomes e membros de todos os threads de chat. |Sim | Não |
|_Chat.UpdatePolicyViolation.All_ |Sinalizar mensagens de chat para a política de violação |Permite que o aplicativo atualize as mensagens de chat de grupo ou Microsoft Teams 1:1, aplicando um conjunto de propriedades de violação da política de prevenção contra perda de dados (DLP) para controlar a saída de processamento DLP. | Sim | Não |

> **Observação:** para mensagens em um canal, consulte [permissões ChannelMessage](#channel-message-permissions).

## <a name="chat-resource-specific-consent-permissions"></a>Permissões de consentimento específicas do recurso de chat

#### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão                     | Exibir Cadeia de Caracteres                                                | Descrição  | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:-------------------------------|:--------------------------------------------------------------|:-------------|:-----------------------|:----------------------------|
| _ChatSettings.Read.Chat_         | Leia as configurações deste chat.                                    | Permite que o aplicativo leia as configurações deste chat, sem um usuário conectado. |Não | Não |
| _ChatSettings.ReadWrite.Chat_    | Leia e escreva as configurações deste chat.                          | Permite que o aplicativo leia e grave as configurações deste chat, sem um usuário conectado. |Não | Não |
| _ChatMessage.Read.Chat_          | Leia as mensagens deste chat.                                    | Permite que o aplicativo leia as mensagens deste chat, sem um usuário conectado. |Não | Não |
| _ChatMember.Read.Chat_           | Leia os membros deste chat.                                     | Permite que o aplicativo leia os membros deste chat, sem um usuário conectado. |Não | Não |
| _Chat.Manage.Chat_               | Gerenciar este chat                                             | Permite que o aplicativo gerencie o chat, os membros do chat e conceda acesso aos dados do chat, sem um usuário conectado.  |Não | Não |
| _TeamsTab.Read.Chat_             | Leia as guias deste chat.                                        | Permite que o aplicativo leia as guias deste chat, sem um usuário conectado. |Não | Não |
| _TeamsTab.Create.Chat_           | Criar as guias neste chat.                                     | Permite que o aplicativo crie guias neste chat, sem um usuário conectado. |Não | Não |
| _TeamsTab.Delete.Chat_           | Exclua as guias deste chat.                                      | Permite que o aplicativo exclua as guias deste chat, sem um usuário conectado. |Não | Não |
| _TeamsTab.ReadWrite.Chat_        | Gerenciar as guias deste chat.                                      | Permite que o aplicativo gerencie as guias deste chat, sem um usuário conectado. |Não | Não |
| _TeamsAppInstallation.Read.Chat_ | Leia quais aplicativos estão instalados neste chat.                   | Permite que o aplicativo leia os aplicativos Teams que estão instalados neste chat junto com as permissões concedidas a cada aplicativo, sem um usuário conectado.  |Não | Não |
| _OnlineMeeting.ReadBasic.Chat_   | Leia as propriedades básicas de uma reunião associada a este chat. | Permite que o aplicativo leia as propriedades básicas - como nome, programação, organizador e link de ingresso - de uma reunião associada a este chat, sem um usuário conectado. |Não | Não |
| _Calls.AccessMedia.Chat_         | Acesse fluxos de mídia em chamadas associadas a esse chat ou reunião.                                    | Permite que o aplicativo acesse fluxos de mídia em chamadas associadas a esse chat ou reunião, sem um usuário conectado. |Não | Não |
| _Calls.JoinGroupCalls.Chat_         | Participe de chamadas associadas a esse chat ou reunião.                                    | Permite que o aplicativo leia as propriedades básicas - como nome, programação, organizador e link de ingresso - de uma reunião associada a este chat, sem um usuário conectado. |Não | Não |
| _TeamsActivity.Send.Chat_        | Envie notificações de feed de atividades para usuários neste chat.       | Permite que o aplicativo crie novas notificações nos feeds de atividades de trabalho em equipe dos usuários neste chat, sem um usuário conectado. | Não | Não |

>[!NOTE]
> Atualmente, estas permissões são suportadas apenas na versão beta do Microsoft Graph.

## <a name="chatmessage-permissions"></a>Permissões chatMessage

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChatMessage.Send_ | Enviar mensagens de chat do usuário | Permite que o aplicativo envie mensagens de chat individuais e de grupo no Microsoft Teams, em nome do usuário conectado. | Não | Não |

---

## <a name="cloud-pc-permissions"></a>Permissões do PC na nuvem

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_CloudPC.Read.All_ | Leia PCs na Internet | Permite que o aplicativo leia objetos do PC na Internet, como políticas de provisionamento, em nome do usuário conectado. | Não | Não |
|_CloudPC.ReadWrite.All_ | Ler e escrever PCs na Internet | Permite que o aplicativo crie, leia, atualize e exclua objetos do PC na Nuvem, tais como conexões de rede do Azure, políticas de provisionamento e imagens de dispositivos, em nome do usuário. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_CloudPC.Read.All_ | Leia PCs na Internet | Permite que o aplicativo leia objetos do PC na Internet, como políticas de provisionamento, sem um usuário conectado. | Não | Não |
|_CloudPC.ReadWrite.All_ | Ler e escrever PCs na Internet | Permite que o aplicativo crie, leia, atualize e exclua objetos do PC na Nuvem, como conexões de rede Azure, políticas de provisionamento e imagens de dispositivos, sem um usuário conectado. | Sim | Não |

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _CloudPC.Read.All_: visualize as propriedades de todos os PCs na Internet(`GET /deviceManagement/virtualEndpoint/cloudPCs`).
* _CloudPC.ReadWrite.All_: edite a política de provisionamento do PC na Internet(`PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}`).

#### <a name="application"></a>Aplicativo

* _CloudPC.Read.All_: visualize as propriedades de todos os PCs na Internet(`GET /deviceManagement/virtualEndpoint/cloudPCs`).
* _CloudPC.ReadWrite.All_: edite a política de provisionamento do PC na Internet(`PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}`).

---

## <a name="consent-requests-permissions"></a>Autorizações de pedidos de consentimento

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ConsentRequest.Read.All_ |Ler solicitações de consentimento |Permite que o aplicativo leia solicitações e aprovações de consentimento, em nome do usuário conectado. |Sim | Não |
|_ConsentRequest.ReadWrite.All_ |Ler e gravar solicitações de consentimento |Permite que o aplicativo leia solicitações e aprovações de consentimento e negue ou aprove essas solicitações em nome do usuário conectado. |Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_ConsentRequest.Read.All_ |Ler solicitações de consentimento |Permite que o aplicativo leia as solicitações e aprovações de consentimento do aplicativo sem um usuário conectado. |Sim |
|_ConsentRequest.ReadWrite.All_ |Ler e gravar solicitações de consentimento |Permite que o aplicativo leia solicitações e aprovações de consentimento de aplicativo e negue ou aprove essas solicitações sem um usuário conectado. |Sim |

## <a name="contacts-permissions"></a>Permissões de contatos

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Contacts.Read_ |Ler contatos do usuário  |Permite ao aplicativo ler os contatos do usuário. |Não | Sim |
|_Contacts.Read.Shared_ |Ler usuário e contatos compartilhados |Permite que o aplicativo leia os contatos que o usuário tem permissão de acessar, incluindo os próprios contatos do usuário e os contatos compartilhados. |Não |Não|
|_Contacts.ReadWrite_ |Ter acesso total aos contatos do usuário |Permite ao aplicativo criar, ler, atualizar e excluir contatos do usuário. |Não |Sim|
|_Contacts.ReadWrite.Shared_ |Ler e registrar usuário e contatos compartilhados |Permite que o aplicativo crie, leia, atualize e exclua os contatos para os quais o usuário tem permissão, incluindo os próprios contatos do usuário e os contatos compartilhados. |Não |Não|

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Contacts.Read_ |Ler contatos em todas as caixas de correio |Permite ao aplicativo ler todos os contatos em todas as caixas de correio sem um usuário conectado. |Sim |
|_Contacts.ReadWrite_ |Ler e gravar contatos em todas as caixas de correio |Permite ao aplicativo criar, ler, atualizar e excluir todos os contatos em todas as caixas de correio sem um usuário conectado. |Sim |

> Os Administradores **Importantes** podem configurar a [política de acesso ao aplicativo](auth-limit-mailbox-access.md) para limitar o acesso do aplicativo às caixas de correio _específicas_ e não a todas as caixas de correio na organização, mesmo que as permissões de aplicativo do Contacts.Read or Contacts.ReadWrite sejam concedidas ao aplicativo. 

### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegado

* _Contacts.Read_: Ler um contato a partir de uma das pastas de contatos de nível superior do usuário conectado (`GET /me/contactfolders/{Id}/contacts/{id}`).
* _Contacts.ReadWrite_: Atualizar a foto de contato de um dos contatos do usuário conectado (`PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`).
* _Contacts.ReadWrite_: Adicionar contatos à pasta raiz do usuário conectado (`POST /me/contacts`).

#### <a name="application"></a>Aplicativo

* _Contacts.Read_: Ler contatos a parir de uma das pastas de contatos de nível superior de qualquer usuário da organização (`GET /users/{id | userPrincipalName}/contactfolders/{Id}/contacts/{id}`).
* _Contacts.ReadWrite_: Atualizar a foto de qualquer contato de qualquer usuário em uma organização (`PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`).
* _Contacts.ReadWrite_: Adicionar contatos à pasta raiz de qualquer usuário da organização (`POST /users/{id | userPrincipalName}/contacts`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="custom-security-attributes-permissions"></a>Permissões de atributos de segurança personalizados

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _CustomSecAttributeAssignment.Read.All_ | Ler atribuições de atributo de segurança personalizadas | Permite que o aplicativo leia e grave atribuições de atributos de segurança personalizados para todos os principais no locatário em nome de um usuário conectado. | Sim | Não |
| _CustomSecAttributeAssignment.ReadWrite.All_ | Ler e escrever atribuições de atributos de segurança personalizados | Permite que o aplicativo leia e grave atribuições de atributos de segurança personalizados para todos os principais no locatário em nome de um usuário conectado. | Sim | Não |
| _CustomSecAttributeDefinition.Read.All_ | Ler definições de atributo de segurança personalizadas | Permite que o aplicativo leia e grave definições de atributo de segurança personalizadas para o locatário em nome de um usuário conectado. | Sim | Não |
| _CustomSecAttributeDefinition.ReadWrite.All_ | Ler e escrever definições de atributos de segurança personalizados | Permite que o aplicativo leia e grave definições de atributo de segurança personalizadas para o locatário em nome de um usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _CustomSecAttributeAssignment.Read.All_ | Ler atribuições de atributo de segurança personalizadas | Permite que o aplicativo leia e grave atribuições de atributos de segurança personalizados para todos os principais no locatário sem um usuário conectado. | Sim |
| _CustomSecAttributeAssignment.ReadWrite.All_ | Ler e escrever atribuições de atributos de segurança personalizados | Permite que o aplicativo leia e grave atribuições de atributos de segurança personalizados para todos os principais no locatário sem um usuário conectado. | Sim |
| _CustomSecAttributeDefinition.Read.All_ | Ler definições de atributo de segurança personalizadas | Permite que o aplicativo leia e grave definições de atributos de segurança personalizados para o locatário sem um usuário conectado. | Sim |
| _CustomSecAttributeDefinition.ReadWrite.All_ | Ler e escrever definições de atributos de segurança personalizados | Permite que o aplicativo leia e grave definições de atributos de segurança personalizados para o locatário sem um usuário conectado. | Sim |

---

## <a name="granular-delegated-admin-privileges-gdap-permissions"></a>Permissões granulares de privilégios de administrador delegado (GDAP)

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _DelegatedAdminRelationship.Read.All_ | Leia sobre as relações do Administrador Delegado com os clientes | Permite que o aplicativo leia os detalhes das relações do administrador delegado com clientes, tais como os detalhes de acesso (que incluem funções) e a duração, bem como as atribuições de funções específicas para grupos de segurança em nome do usuário conectado. | Sim | Não |
| _DelegatedAdminRelationship.ReadWrite.All_ | Gerenciar as relações do Administrador Delegado com os clientes | Permite que o aplicativo gerencie (criar-atualizar-encerrar) as relações do Administrador Delegado com clientes e atribuições de função a grupos de segurança para relações ativas do Administrador Delegado em seu nome. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _DelegatedAdminRelationship.Read.All_ | Leia sobre as relações do Administrador Delegado com os clientes | Permite que o aplicativo leia os detalhes das relações do administrador delegado com clientes, tais como os detalhes de acesso (que incluem funções) e a duração, bem como as atribuições de funções específicas para grupos de segurança sem um usuário conectado. | Sim | Não |
| _DelegatedAdminRelationship.ReadWrite.All_ | Gerenciar as relações do Administrador Delegado com os clientes | Permite que o aplicativo gerencie (criar-atualizar-encerrar) as relações do Administrador Delegado com clientes e atribuições de função a grupos de segurança para relações ativas do Administrador Delegado sem um usuário conectado. | Sim | Não |

---

## <a name="device-permissions"></a>Permissões de dispositivos

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Device.Read_ |Ler os dispositivos do usuário |Permite ao aplicativo ler a lista de dispositivos do usuário em nome do usuário conectado. |Não | Sim |
|_Device.Read.All_ |Leia todos os dispositivos |Permite que o aplicativo leia as informações de configuração dos dispositivos da sua organização, em nome do usuário conectado.|Sim | Sim |
|_Device.Command_ |Comunicar-se com os dispositivos do usuário |Permite ao aplicativo se comunicar ou inicializar outro aplicativo no dispositivo do usuário em nome do usuário conectado. |Não | Sim |


#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Device.Read.All_ |Leia todos os dispositivos |Permite que o aplicativo leia as informações de configuração dos dispositivos da sua organização sem um usuário conectado. |Sim |
|_Device.ReadWrite.All_ |Ler e registrar dispositivos |Permite que o aplicativo leia e registre todas as propriedades dos dispositivos sem um usuário conectado. Não permite a criação de dispositivos, exclusão de dispositivos ou atualização de identificadores de segurança de dispositivo alternativo. |Sim |

> [!NOTE]
> Antes de 3 de dezembro de 2020, quando a permissão de solicitação do aplicativo *Device.ReadWrite.All* foi concedida, a função do diretório [Gerenciadores de Diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#deprecated-roles) também foi atribuída ao diretor de serviços do aplicativo. Essa atribuição de função de diretório não é removida automaticamente quando as permissões de aplicativo associadas são revogadas. Para garantir que o acesso de um aplicativo a leitura ou gravação nos dispositivos seja removido, os clientes também devem remover as funções de diretório que foram concedidas ao aplicativo.
> 
> Uma atualização de serviço desativando esse comportamento começou a ser lançada em 3 de dezembro de 2020. Implantação para todos os clientes concluída em 11 de janeiro de 2021. As funções de diretório não são mais atribuídas automaticamente quando as permissões do aplicativo são concedidas.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="application"></a>Aplicativo

* _Device.ReadWrite.All_: Ler todos os dispositivos registrados na organização (`GET /devices`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="directory-permissions"></a>Permissões do diretório

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Directory.Read.All_ |Ler dados do diretório | Permite ao aplicativo ler dados no diretório da sua organização, como usuários, grupos e aplicativos. **Observação**: os usuários poderão dar o consentimento aos aplicativos que exigem essa permissão se o aplicativo estiver registrado no locatário da própria organização.| Sim | Não |
| _Directory.ReadWrite.All_ |Ler e gravar dados de diretório | Permite ao aplicativo ler e gravar dados no diretório da sua organização, como usuários e grupos. Não permite ao aplicativo excluir usuários ou grupos, ou redefinir senhas de usuário. | Sim | Não |
| _Directory.AccessAsUser.All_ |Access Directory como o usuário conectado  | Permite ao aplicativo ter o mesmo acesso que o usuário conectado a informações no diretório. | Sim | Não |

<br/>

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_ | Ler dados do diretório | Permite ao aplicativo ler dados no diretório da sua organização, como usuários, grupos e aplicativos, sem um usuário conectado. | Sim |
| _Directory.ReadWrite.All_ | Ler e gravar dados de diretório | Permite ao aplicativo ler e registrar dados no diretório de sua organização, como usuários e grupos, sem um usuário conectado. Não permite a exclusão de usuários ou grupos. | Sim |

### <a name="remarks"></a>Comentários

As permissões de diretório fornecem o nível mais alto de privilégio para acessar recursos de diretório, como [usuário](/graph/api/resources/user), [grupo](/graph/api/resources/group) e [dispositivo](/graph/api/resources/device) em uma organização.

Eles também controlam exclusivamente o acesso a outros recursos de diretório, como: [contatos organizacionais](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true), [APIs de extensão de esquema](/graph/api/resources/schemaextension?view=graph-rest-beta&preserve-view=true), [APIs de gerenciamento de identidade privilegiada (PIM)](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true), bem como muitos dos recursos e APIs listados no nó **Azure Active Directory** na documentação de referência da API v1.0 e beta. Isso inclui unidades administrativas, funções de diretório, configurações de diretório, política e muito mais.

> [!NOTE]
> Antes de 3 de dezembro de 2020, quando a permissão do aplicativo *Directory.Read.All* foi concedido, o [Leitores de diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#directory-readers-permissions) a função de diretório também foi atribuída ao principal de serviço do aplicativo.  Quando *Directory.ReadWrite.All* foi concedido, o [Escritores de diretório](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#directory-writers-permissions)a função de diretório também foi atribuída. Essas funções de diretório não são removidas automaticamente quando as permissões de aplicativo associadas são revogadas. Para remover o acesso de um aplicativo para ler ou gravar no diretório, os clientes também deve remover as funções de diretório que foram concedidas ao aplicativo.
> 
> Uma atualização de serviço desativando esse comportamento começou a ser lançada em 3 de dezembro de 2020. Implantação para todos os clientes concluída em 11 de janeiro de 2021. As funções de diretório não são mais atribuídas automaticamente quando as permissões do aplicativo são concedidas.

A permissão _Directory.ReadWrite.All_ concede os seguintes privilégios:

- Leitura completa de todos os recursos de diretório (propriedades declaradas e propriedades de navegação)
- Criar e atualizar usuários
- Desabilitar e habilitar usuários (mas não o Administrador da Empresa)
- Definir o identificador de segurança alternativa do usuário (mas não administradores)
- Criar e atualizar grupos
- Gerenciar associações do grupo
- Atualizar o proprietário do grupo
- Gerenciar as atribuições de licença
- Definir as extensões de esquema em aplicativos
- Gerenciar configurações de diretório
- Gerenciar a configuração do fluxo de trabalho de consentimento do administrador (mas não se o consentimento do administrador é necessário ou quem está autorizado a conceder o consentimento do administrador)

> **Observação**:
> - Nenhum direito de redefinir senhas de usuários.
> - A atualização das propriedades **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida somente para usuários que não sejam administradores ou que tenham uma das seguintes funções atribuídas: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios. Para obter mais detalhes, confira Administrador de suporte técnico (senha) nas [funções disponíveis do Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).  Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.
> - Nenhum direito de excluir recursos (incluindo usuários ou grupos).
> - Exclui especificamente a criação ou a atualização de recursos que não estão listados acima. Isso inclui: application, oAauth2Permissiongrant, appRoleAssignment, device, servicePrincipal, organization, domains e assim por diante.


### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado
* _Directory.Read.All_: Listar todas as unidades administrativas em uma organização (`GET /beta/administrativeUnits`)
* _Directory.ReadWrite.All_: Adicionar membros a uma função de diretório (`POST /directoryRoles/{id}/members/$ref`)

#### <a name="application"></a>Aplicativo
* _Directory.Read.All_: Listar todas as associações de um usuário, incluindo funções de diretório e unidades administrativas (`GET /beta/users/{id}/memberOf`)
* _Directory.Read.All_: Listar todos os membros do grupo, incluindo as entidades de serviço (`GET /beta/groups/{id}/members`)
* _Directory.ReadWrite.All_: Adicionar um proprietário a um grupo (`POST /groups/{id}/owners/$ref`)


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="domain-permissions"></a>Permissões de domínio

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Domain.Read.All_ |Ler domínios|Permite que o aplicativo leia todas as propriedades de domínio, em nome do usuário conectado. |Sim | Não |
|_Domain.ReadWrite.All_ | Ler e registrar domínios |Permite que o aplicativo leia e grave todas as propriedades de domínio, em nome do usuário conectado. Também permite que o aplicativo adicione, verifique e remova domínios. |Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Domain.Read.All_ | Ler domínios | Permite que o aplicativo leia todas as propriedades de domínio sem um usuário conectado. | Sim |
| _Domain.ReadWrite.All_ | Ler e registrar domínios | Permite que o aplicativo leia e escreva domínios sem um usuário conectado. | Sim |

---

## <a name="ediscovery-permissions"></a>Permissões de eDiscovery

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_eDiscovery.Read.All_ |Ler dados de casos de eDiscovery do usuário |Permite que o aplicativo leia objetos de eDiscovery, como casos, custodiantes, conjuntos de revisão e outros objetos relacionados em nome do usuário conectado.. |Sim | Não |
|_eDiscovery.ReadWrite.All_ | Ler e gravar dados de casos de eDiscovery |Permite que o aplicativo leia e grave objetos de descoberta eletrônica, como casos, custodiantes, conjuntos de revisão e outros objetos relacionados em nome do usuário conectado. |Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

Nenhum

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _eDiscovery.Read.All_: Obtenha a lista de casos disponíveis para o (`GET /compliance/ediscovery/cases`)
* _eDiscovery.ReadWrite.All_: Criar uma consulta de conjunto de revisões em um conjunto de revisões (`POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewSetId}/queries`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="education-permissions"></a>Permissões de educação

#### <a name="delegated-permissions"></a>Permissões delegadas

| Permissão                      | Exibir Cadeia de Caracteres                                                   | Descrição                                                                                                                                                                                                                                                                      | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
| :------------------------------ | :--------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------- | :-------------------------- |
| _EduAdministration.Read_        | Ler configurações do aplicativo educacional                                      | Permite que o aplicativo leia as configurações do aplicativo de educação em nome do usuário.                                                                                                                                                                                                             | Sim                    | Não                          |
| _EduAdministration.ReadWrite_   | Gerenciar as configurações do aplicativo educacional                                    | Permite que o aplicativo gerencie as configurações do aplicativo de educação em nome do usuário.                                                                                                                                                                                                           | Sim                    | Não                          |
| _EduAssignments.ReadBasic_      | Ler as tarefas de classe sem notas dos usuários                     | Permite ao aplicativo ler as tarefas sem notas em nome do usuário                                                                                                                                                                                                          | Sim                    | Não                          |
| _EduAssignments.ReadWriteBasic_ | Ler e gravar as tarefas de classe sem notas dos usuários           | Permite ao aplicativo ler e gravar as tarefas sem notas em nome do usuário                                                                                                                                                                                                | Sim                    | Não                          |
| _EduAssignments.Read_           | Ler o modo de exibição de tarefas de classe e as notas delas dos usuários           | Permite ao aplicativo ler as tarefas e as notas delas em nome do usuário                                                                                                                                                                                                        | Sim                    | Não                          |
| _EduAssignments.ReadWrite_      | Ler e gravar o modo de exibição de tarefas da classe e as notas delas dos usuários | Permite ao aplicativo ler e gravar as tarefas e as notas delas em nome do usuário                                                                                                                                                                                              | Sim                    | Não                          |
| _EduRoster.ReadBasic_           | Ler um subconjunto limitado do modo de exibição dos usuários da lista de participantes               | Permite que o aplicativo leia um subconjunto limitado de propriedades da estrutura das escolas e classes de uma organização e um subconjunto limitado de propriedades sobre os usuários para ser lido em nome do usuário. Inclui nome, status, função educacional, endereço de e-mail e foto. | Sim                    | Não                          |
| _EduRoster. Read_                | Ler modo de exibição dos usuários da lista de participantes                                   | Permite ao aplicativo ler a estrutura de escolas e aulas na lista de participação de uma organização e informações específicas de educação sobre os usuários a serem lidas em nome do usuário.                                                                                                         | Sim                    |
| _EduRoster.ReadWrite_           | Ler e escrever o modo de exibição dos usuários da lista de participantes                         | Permite ao aplicativo ler e escrever a estrutura de escolas e aulas na lista de participação de uma organização e informações específicas de educação sobre os usuários a serem lidas e escritas em nome do usuário.                                                                                   | Sim                    |

#### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão                          | Exibir Cadeia de Caracteres                                      | Descrição                                                                                                                                                                   | Consentimento Obrigatório do Administrador |
| :---------------------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------- |
| _EduAdministration.Read.All_        | Ler configurações do aplicativo ducacional                         | Ler o estado e as configurações de todos os aplicativos educacionais da Microsoft em nome do usuário                                                                                             | Sim                    |
| _EduAdministration.ReadWrite.All_   | Gerenciar as configurações do aplicativo educacional                       | Gerenciar o estado e as configurações de todos os aplicativos educacionais da Microsoft em nome do usuário                                                                                           | sim                    |
| _EduAssignments.ReadBasic.All_      | Ler as tarefas de classe sem notas               | Permite ao aplicativo ler as tarefas sem notas para todos os usuários                                                                                                               | Sim                    |
| _EduAssignments.ReadWriteBasic.All_ | Ler e gravar as tarefas de classe sem notas     | Permite ao aplicativo ler e gravar as tarefas sem notas para todos os usuários                                                                                                     | Sim                    |
| _EduAssignments.Read.All_           | Ler as tarefas de classe com notas                  | Permite ao aplicativo ler as tarefas e as notas delas para todos os usuários                                                                                                             | Sim                    |
| _EduAssignments.ReadWrite.All_      | Ler e gravar as tarefas de classe com notas        | Permite ao aplicativo ler e gravar as tarefas e as notas delas para todos os usuários                                                                                                   | Sim                    |
| _EduRoster.ReadBasic.All_           | Ler um subconjunto limitado da lista de participação da organização. | Permite ao aplicativo ler um subconjunto limitado de estrutura de escolas e aulas na lista de participação de uma organização e informações específicas de educação sobre todos os usuários.          | Sim                    |
| _EduRoster.Read.All_                | Ler a lista de participação da organização.                     | Permite ao aplicativo ler a estrutura de escolas e aulas na lista de participação de uma organização e informações específicas de educação sobre todos os usuários a serem lidas.                       | Sim                    |
| _EduRoster.ReadWrite.All_           | Ler e gravar a lista de participação da organização.           | Permite ao aplicativo ler e gravar a estrutura de escolas e aulas na lista de participação de uma organização e informações específicas de educação sobre todos os usuários a serem lidas e gravadas. | Sim                    |

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _EduAssignments.Read_: extrair as informações de atribuição do aluno conectado (`GET /education/classes/{id}/assignments/{id}`)
* _EduAssignments.ReadWriteBasic_: enviar a tarefa do aluno conectado (`GET /education/classes/{id}/assignments/{id}submit`)
* _EduRoster.ReadBasic_: aulas de que um usuário conectado participa como aluno ou professor (`GET /education/classes/{id}/members`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="entitlement-management-permissions"></a>Permissões de gerenciamento de direitos

#### <a name="delegated-permissions"></a>Permissões delegadas

|Permissão|Exibir Cadeia de Caracteres|Descrição|Consentimento Obrigatório do Administrador|
|:----------|:--------------|:-----------|:-------|
|_EntitlementManagement.ReadWrite.All_|Ler e gravar os recursos de gerenciamento de direitos|Permite ao aplicativo solicitar acesso para ler e gerenciar pacotes de acesso e recursos de gerenciamento de direitos relacionados em nome do usuário conectado.|Sim|
|_EntitlementManagement.Read.All_|Ler os recursos de gerenciamento de direitos|Permite ao aplicativo solicitar acesso para ler pacotes de acesso e recursos de gerenciamento de direitos relacionados em nome do usuário conectado.|Sim|

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão|Exibir Cadeia de Caracteres|Descrição|Consentimento Obrigatório do Administrador|
|:----------|:--------------|:-----------|:-------|
|_EntitlementManagement.ReadWrite.All_|Ler e gravar os recursos de gerenciamento de direitos|Permite que o aplicativo leia e gerencie pacotes de acesso e recursos de gerenciamento de direitos relacionados.|Sim|
|_EntitlementManagement.Read.All_|Ler os recursos de gerenciamento de direitos|Permite que o aplicativo leia pacotes de acesso e recursos de gerenciamento de direitos relacionados.|Sim|

## <a name="files-permissions"></a>Permissões de arquivos

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Files.Read_ | Ler arquivos do usuário | Permite que o aplicativo leia todos os arquivos do usuário conectado. | Não | Sim |
| _Files.Read.All_ | Ler todos os arquivos que o usuário pode acessar | Permite que o aplicativo para leia todos os arquivos que o usuário conectado pode acessar. | Não | Sim |
| _Files.ReadWrite_  | Ter acesso total aos arquivos do usuário | Permite que o aplicativo leia, crie, atualize e exclua os arquivos do usuário conectado. | Não| Sim |
| _Files.ReadWrite.All_ | Ter acesso total a todos os arquivos que o usuário pode acessar | Permite que o aplicativo leia, crie, atualize e exclua todos os arquivos que o usuário conectado pode acessar. | Não | Sim |
| _Files.ReadWrite.AppFolder_ | Ter acesso total à pasta do aplicativo (prévia) | (Prévia) Permite que o aplicativo leia, crie, atualize exclua arquivos na pasta do aplicativo. | Não | Sim |
| _Files.Read.Selected_  | Ler arquivos selecionados pelo usuário | **Suporte limitado no Microsoft Graph – confira Comentários** <br/> (Visualização) Permite ao aplicativo ler arquivos selecionados pelo usuário. O aplicativo tem acesso por várias horas depois que o usuário tiver selecionado um arquivo.  | Não | Não |
| _Files.ReadWrite.Selected_ | Ler e gravar arquivos selecionados pelo usuário | **Suporte limitado no Microsoft Graph – confira Comentários** <br/> (Visualização) Permite ao aplicativo ler e gravar arquivos selecionados pelo usuário. O aplicativo tem acesso por várias horas depois que o usuário tiver selecionado um arquivo. | Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão | Exibir Cadeia de Caracteres | Descrição | Consentimento Obrigatório do Administrador |
| :--------- | :------------- | :---------- | :--------------------- |
| _Files.Read.All_ | Ler arquivos em todos os conjuntos de sites | Permite ao aplicativo ler todos os arquivos em todos os conjuntos de sites sem um usuário conectado.  | Sim |
| _Files.ReadWrite.All_ | Ler e gravar arquivos em todos os conjuntos de sites | Permite ao aplicativo ler, criar, atualizar e excluir todos os arquivos em todos os conjuntos de sites sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

> **Observe** que nas contas pessoais,Files.Read e Files.ReadWrite também concedem acesso a arquivos compartilhados com o usuário conectado.

As permissões delegadas Files.Read.Selected e Files.ReadWrite.Selected são válidas apenas em contas corporativas ou de estudante e são expostas apenas para trabalhar com [manipuladores (v1.0) de arquivos do Office 365](/previous-versions/office/office-365-api/). Elas não devem ser usadas para chamar diretamente as APIs do Microsoft Graph.

A permissão delegada Files.ReadWrite.AppFolder só é válida para contas pessoais e é usada para acessar a [pasta especial da Raiz de Aplicativo](https://dev.onedrive.com/misc/appfolder.htm) com a API do Microsoft Graph [Obter pasta especial](/graph/api/drive-get-specialfolder) do OneDrive.


### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Files.Read_: Ler arquivos armazenados no OneDrive do usuário conectado (`GET /me/drive/root/children`)
* _Files.Read.All_: Ler arquivos compartilhados com o usuário conectado (`GET /me/drive/root/sharedWithMe`)
* _Files.ReadWrite_: Gravar um arquivo no OneDrive do usuário conectado (`PUT /me/drive/root/children/filename.txt/content`)
* _Files.ReadWrite.All_: Gravar um arquivo compartilhado com o usuário (`PUT /users/rgregg@contoso.com/drive/root/children/file.txt/content`)
* _Files.ReadWrite.AppFolder_: Gravar arquivos na pasta do aplicativo do OneDrive (`PUT /me/drive/special/approot/children/file.txt/content`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---
## <a name="financials-permissions"></a>Permissões de finanças
#### <a name="delegated-permissions"></a>Permissões delegadas

|Permissão|Exibir Cadeia de Caracteres|Descrição|Consentimento Obrigatório do Administrador|
|:----------|:--------------|:-----------|:-------|
|_Financials.ReadWrite.All_|Ler e gravar dados de finanças|Permite que o aplicativo leia e grave dados de finanças em nome do usuário conectado.|Não|

## <a name="group-permissions"></a>Permissões de grupo

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Group.Read.All_ |    Ler todos os grupos | Permite ao aplicativo listar grupos, e ler suas propriedades e todas as associações do grupo em nome do usuário conectado.  Também permite ao aplicativo ler calendário, conversas, arquivos e outros tipos de conteúdo de todos os grupos que o usuário conectado pode acessar. | Sim | Não |
| _Group.ReadWrite.All_ |    Ler e gravar todos os grupos| Permite ao aplicativo criar grupos e ler todas as propriedades e associações do grupo em nome do usuário conectado.  Também permite ao aplicativo ler calendário, conversas, arquivos e outros tipos de conteúdo de todos os grupos que o usuário conectado pode acessar. Além disso, permite aos proprietários do grupo gerenciar seus grupos, e permite aos membros do grupo atualizar o conteúdo do grupo. | Sim | Não |
| _GroupMember.Read.All_ |    Ler associações de grupo | Permite que o aplicativo liste grupos, leia as propriedades básicas do grupo e leia a associação de todos os grupos aos quais o usuário conectado tenha acesso. | Sim | Não |
| _GroupMember.ReadWrite.All_ |    Ler e gravar associações de grupo | Permite que o aplicativo liste grupos, leia propriedades básicas, leia e atualize a associação dos grupos aos quais o usuário conectado tem acesso. As propriedades e os proprietários do grupo não podem ser atualizados e os grupos não podem ser excluídos. | Sim | Não |
| _UnifiedGroupMember.Read.AsGuest_ |    Leia as associações do grupo unificado (Microsoft 365) como um usuário convidado | Permite que o aplicativo leia as propriedades básicas do grupo unificado, associações e os proprietários do grupo do qual o convidado assinado é um membro. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ | Ler todos os grupos | Permite que o aplicativo leia as associações de todos os grupos sem um usuário conectado. Também permite que o aplicativo leia o calendário, conversas, arquivos e outros conteúdos de grupo para todos os grupos.<br/><br/>**Observação:** nem todas as APIs de grupo oferecem suporte ao acesso usando permissões somente de aplicativo. Confira exemplos nos [problemas conhecidos](known-issues.md). | Sim |
| _Group.ReadWrite.All_ | Ler e gravar todos os grupos | Permite que o aplicativo crie grupos, leia e atualize as associações do grupo e exclua grupos. Também permite ao aplicativo ler e escrever o calendário, as conversas, os arquivos e outros tipos de conteúdo de grupos para todos os grupos. Todas essas operações podem ser executadas pelo aplicativo sem um usuário conectado.<br/><br/>**Observação:** nem todas as APIs de grupo oferecem suporte ao acesso usando permissões somente de aplicativo. Confira exemplos nos [problemas conhecidos](known-issues.md).| Sim |
| _Group.Selected_ |    Acessar grupos selecionados | **Observação: Essa permissão está exposta no portal do Azure para um recurso que não está disponível para uso geral. Não use essa permissão, pois ela está sujeita a alterações.** | Sim |
| _GroupMember.Read.All_ |    Ler associações de grupo | Permite que o aplicativo leia grupos e as propriedades básicas do grupo para todos os grupos sem um usuário conectado. | Sim |
| _GroupMember.ReadWrite.All_ |    Ler e gravar associações de grupo | Permite que o aplicativo liste grupos, leia propriedades básicas, leia e atualize a associação dos grupos sem um usuário conectado. As propriedades e os proprietários do grupo não podem ser atualizados e os grupos não podem ser excluídos. | Sim |
| _Group.Create_ |    Criar grupos | Permite que o aplicativo de chamada crie grupos sem um usuário conectado. Não permite ler, atualizar ou excluir grupos. | Sim |

### <a name="remarks"></a>Comentários

A funcionalidade de grupo não é compatível com contas pessoais da Microsoft.

Para grupos do Microsoft 365, as permissões de grupo concedem ao aplicativo acesso ao conteúdo do grupo. Por exemplo, conversas, arquivos, anotações e assim por diante.

No caso de Permissões de aplicativo, há algumas limitações para APIs com suporte. Confira mais informações em [problemas conhecidos](known-issues.md).

Em alguns casos, um aplicativo pode precisar de [Permissões de diretório](#directory-permissions) para ler algumas propriedades do grupo como `member` e `memberOf`. Por exemplo, se um grupo tiver um ou mais [servicePrincipals](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) como membros, o aplicativo precisará de permissões eficazes para ler as entidades de serviço através do recebimento de uma das _Permissões de diretório\*_, caso contrário, o Microsoft Graph retornará um erro. No caso de Permissões Delegadas, o usuário conectado deve ter privilégios suficientes na organização para ler as entidades de serviço. A mesma orientação se aplica à propriedade `memberOf` que pode retornar [administrativeUnits](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).

Para definir o atributo **preferredDataLocation** de um grupo do Microsoft 365, um aplicativo precisa da permissão Directory.ReadWrite.All. Quando os usuários em um ambiente multigeográfico criam um grupo do Microsoft 365, o valor **preferredDataLocation** para o grupo é definido automaticamente como sendo igual ao do usuário. Para saber mais sobre o local de dados preferencial dos grupos, confira [Criar um grupo do Microsoft 365 com uma PDL específica](/office365/enterprise/multi-geo-add-group-with-pdl).

As permissões de grupo são usadas para controlar o acesso aos recursos e APIs do [Microsoft Teams](/graph/api/resources/teams-api-overview). Não há suporte para as contas pessoais da Microsoft.

As Permissões de grupo também são usadas para controlar o acesso a APIs e recursos do [Microsoft Planner](/graph/api/resources/planner-overview). Somente as permissões delegadas são suportadas pelas APIs do Microsoft Planner; as permissões de aplicativo não são suportadas. Contas pessoais da Microsoft não são suportadas.


### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegado

* _Group.Read.All_: Ler todos os grupos do Microsoft 365 dos quais o usuário conectado é membro (`GET /me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`).
* _Group.Read.All_: Ler todo o conteúdo do grupo do Microsoft 365, como conversas (`GET /groups/{id}/conversations`).
* _Group.ReadWrite.All_: Atualizar propriedades do grupo, como fotografias (`PUT /groups/{id}/photo/$value`).
* _GroupMember.ReadWrite.All_: Atualizar os membros do grupo (`POST /groups/{id}/members/$ref`).
> **Observação:** Isso também requer o _User.ReadBasic.All_ para ler o usuário para adicionar como membro.

#### <a name="application"></a>Aplicativo

* _Group.Read.All_: Localizar todos os grupos com nomes que começam com "Vendas" (`GET /groups?$filter=startswith(displayName,'Sales')`).
* _Group.ReadWrite.All_: O serviço daemon cria novos eventos no calendário de um grupo do Microsoft 365 (`POST /groups/{id}/events`).
* _Group.Create_: Criar um novo grupo (`POST /groups`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---


## <a name="identity-provider-permissions"></a>Permissões do provedor de identidade

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityProvider.Read.All_ |   Leia as informações do provedor de identidade  | Permite que o aplicativo leia os provedores de identidade configurados em seu Azure AD ou no locatário do Azure AD B2C em nome do usuário conectado. | Sim | Não |
| _IdentityProvider.ReadWrite.All_ |   Leia e grave informações do provedor de identidade  |  Permite que o aplicativo leia ou grave provedores de identidade configurados no seu Azure AD ou no locatário do Azure AD B2C em nome do usuário conectado. | Sim | Não |

### <a name="remarks"></a>Comentários

_IdentityProvider.Read.All_ e _IdentityProvider.ReadWrite.All_ são válidos apenas para contas corporativas ou de estudante. Para que um aplicativo leia ou grave provedores de identidade com permissões delegadas, o usuário conectado deve receber a função de Administrador Global. Para obter mais informações sobre funções de administrador, confira [Atribuição de funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado
Os seguintes usos são válidos para permissões delegadas:

* _IdentityProvider.Read.All_: Leia todos os provedores de identidade configurados no locatário (`GET /beta/identityProviders`)
* _IdentityProvider.Read.All_: Leia um provedor de identidade existente (`GET /beta/identityProviders/{id}`)
* _IdentityProvider.ReadWrite.All_ Crie um provedor de identidade (`POST /beta/identityProviders`)
* _IdentityProvider.ReadWrite.All_ Atualize um provedor de identidade existente (`PATCH /beta/identityProviders/{id}`)
* _IdentityProvider.ReadWrite.All_ Exclua um provedor de identidade existente (`DELETE /beta/identityProviders/{id}`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="identity-protection-risk-permissions"></a>Permissões de risco de proteção de identidade

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade  | Permite que o aplicativo para leia as informações de evento de risco de identidade para todos os usuários em sua organização em nome do usuário conectado. | Sim | Não |
| _IdentityRiskyUser.Read.All_ |   Leia as informações de risco de identidade do usuário.  | Permite que o aplicativo para leia as informações de risco de identidade do usuário para todos os usuários em sua organização em nome do usuário conectado. | Sim | Não |
| _IdentityRiskyUser.ReadWrite.All_ |   Ler e atualizar as informações de risco de identidade do usuário.  | Permite que o aplicativo leia as informações de risco de identidade do usuário para todos os usuários em sua organização em nome do usuário conectado. | Sim | Não |
| _IdentityRiskyServicePrincipal.Read.All_ |   Leia todas as informações da entidade de serviço de risco  | Permite que o aplicativo leia todas as informações da entidade de serviço de risco para a sua organização, em nome do usuário conectado. | Sim | Não |
| _IdentityRiskyServicePrincipal.ReadWrite.All_ |   Ler e gravar todas as informações da entidade de serviço de risco  | Permite que o aplicativo leia e atualize informações principais de serviços de risco para todos os diretores de serviços de sua organização, em nome do usuário inscrito. As operações de atualização incluem ignorar entidades de serviços arriscadas.| Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade | Permite que o aplicativo leia as informações do evento de risco de identidade para todos os usuários em sua organização sem um usuário conectado. | Sim |
| _IdentityRiskyUser.Read.All_ |   Leia as informações de risco de identidade do usuário. | Permite que o aplicativo leia as informações de risco de identidade do usuário para todos os usuários em sua organização sem um usuário conectado. | Sim |
| _IdentityRiskyUser.ReadWrite.All_ |   Ler e atualizar as informações de risco de identidade do usuário. | Permite que o aplicativo leia as informações de risco de identidade do usuário para todos os usuários em sua organização sem um usuário conectado. | Sim |
| _IdentityRiskyServicePrincipal.Read.All_ |   Leia todas as informações da entidade de serviço de risco  | Permite que o aplicativo leia todas as informações de entidade de serviço arriscadas para sua organização, sem um usuário conectado. | Sim |
| _IdentityRiskyServicePrincipal.ReadWrite.All_ |   Ler e gravar todas as informações da entidade de serviço de risco  | Permite que o aplicativo leia e atualize as informações de usuário de risco da sua organização sem um usuário conectado.| Sim |

Todas as permissões de risco de identidade são válidas somente para contas corporativas ou de estudante. Para um aplicativo com permissões delegadas para ler informações de risco de identidade, o usuário signatário deve ser um membro de uma das seguintes funções de administrador do [Azure AD funções de administrador](/azure/active-directory/roles/permissions-reference): Administrador Global, Administrador de Segurança, ou Leitor de Segurança.

### <a name="example-usage"></a>Exemplo de uso

Os seguintes usos são válidos para permissões delegadas e permissões de aplicativo:

#### <a name="read-risk-events"></a>Ler eventos de risco

* Ler todos os eventos de risco gerados para todos os usuários do locatário (`GET /identityProtection/riskDetections`)
* Ler os mais recentes 50 eventos de risco (`GET /identityProtection/riskDetections?$orderBy=detectedDateTime desc&top=50`)

#### <a name="read-risky-users"></a>Ler usuários arriscados

* Ler todos os usuários de risco e propriedades no locatário (`GET /identityProtection/riskyUsers`)
* Ler todos os usuários de risco cujo nível de risco agregação é Médio (`GET /identityProtection/riskyUsers?$filter=riskLevel eq 'medium'`)
* Leia as informações de riscos de um usuário específico (`GET /identityProtection/riskyUsers?$filter=id eq 'userId'`)

#### <a name="read-risky-service-principals"></a>Ler entidades de serviço de risco

* Ler todas as entidades de serviço de risco e propriedades no locatário (`GET /identityProtection/riskyServicePrincipals`)
* Ler todas as entidades de serviço de risco cujo nível de risco agregado é Médio (`GET /identityProtection/riskyServicePrincipals?$filter=riskLevel eq 'medium'`)
* Leia as informações de risco para uma entidade de serviço específica (`GET /identityProtection/riskyServicePrincipals?$filter=id eq '{riskyServicePrincipalsId}'`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="identity-user-flow-permissions"></a>Identidade de permissões de fluxo de usuário

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityUserFlow.Read.All_ |   Ler todos os fluxos de usuário de identidade em um locatário  | Permite que o aplicativo leia os fluxos de usuários da sua organização. | Sim | Não |
| _IdentityUserFlow.ReadWrite.All_ |   Ler e gravar todos os fluxos de usuário de identidade em um locatário.    | Permite que o aplicativo leia ou grave os fluxos de usuário da sua organização. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityUserFlow.Read.All_ |   Ler todos os fluxos de usuário de identidade em um locatário  | Permite que o aplicativo leia os fluxos de usuários da sua organização. | Sim | Não |
| _IdentityUserFlow.ReadWrite.All_ |   Ler e gravar todos os fluxos de usuário de identidade em um locatário.    | Permite que o aplicativo leia ou grave os fluxos de usuário da sua organização. | Sim | Não |

### <a name="remarks"></a>Comentários

_IdentityUserFlow.Read.All_ e _IdentityUserFlow.ReadWrite.ALL_ são válidos apenas para contas corporativas ou de estudante.

Para um aplicativo com permissões delegadas para ler fluxos de usuários, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador global, Administrador de Fluxo de usuário de Identidades Externas ou Leitor Global. Para um aplicativo com permissões delegadas para gravar fluxos de usuário, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador global ou Administrador de Fluxo de usuário de Identidades Externas.

Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated-and-application"></a>Permissões delegadas e de aplicativo

Os seguintes usos são válidos para Permissões Delegadas e Permissões de aplicativo:

* _IdentityUserFlow.Read.All_: ler todos os fluxos de usuário em um locatário do Azure AD B2C (`GET beta/identity/b2cUserFlows`)
* _IdentityUserFlow.Read.All_: ler todos os fluxos de usuário em um locatário do Azure Active Directory (Azure AD) (`GET beta/identity/b2xUserFlows`)
* _IdentityUserFlow. Read. All_: ler todas as atribuições de atributo de usuário em um fluxo de usuário do Azure Active Directory B2C (`GET beta/identity/b2cUserFlows/{id}/userAttributeAssignments`)
* _IdentityUserFlow.ReadWrite.All_: criar um novo fluxo de usuário em um locatário do Azure AD B2C (`POST beta/identity/b2cUserFlows`)
* _IdentityUserFlow.ReadWrite.All_: criar um novo fluxo de usuário em um locatário do Azure Active Directory (Azure AD) (`POST beta/identity/b2xUserflows`)
* _IdentitytUserFlow.ReadWrite.All_: adicionar um provedor de identidade a um fluxo de usuário do Azure AD B2C (`PATCH beta/identity/b2cUserFlows/{id}/identityProviders/$ref`)
* _IdentityUserFlow.ReadWrite.All_: remover um provedor de identidade de um usuário do Active Directory B2C (`DELETE beta/identity/b2cUserFlows/{id}/identityProviders/{id}`)
* _IdentityUserFlow. ReadWrite. All_: criar uma atribuição de atributo de usuário em um fluxo de usuário do Azure Active Directory B2C ( `POST beta/identity/b2cUserFlows/{id}/userAttributeAssignments` )

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="information-protection-policy-permissions"></a>Permissões de política de proteção de informações

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _InformationProtectionPolicy. Read_ |   Ler rótulos de confidencialidade do usuário e políticas de rótulos | Permite que um aplicativo leia rótulos de confidencialidade de proteção de informações e configurações de política de rótulo, em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _InformationProtectionPolicy.Read.All_ |   Ler todos os rótulos e políticas de rótulo publicados para uma organização | Permite que um aplicativo leia rótulos de confidencialidade e configurações de política de rótulo publicados de toda a organização ou de um usuário específico, sem um usuário conectado. | Sim |

---


## <a name="intune-device-management-permissions"></a>Permissões de Gerenciamento de Dispositivo do Intune

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_DeviceManagementApps.Read.All_ | Ler aplicativos do Microsoft Intune | Permite que o aplicativo leia as propriedades, as atribuições de grupo, o status de aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementApps.ReadWrite.All_ | Ler e registrar os aplicativos do Microsoft Intune | Permite que aplicativo leia e registre s propriedades, as atribuições de grupo, o status dos aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementConfiguration.Read.All_ | Ler a configuração de dispositivo e as políticas do Microsoft Intune | Permite que o aplicativo leia as propriedades de configuração de dispositivo e as políticas de conformidade de dispositivo do Microsoft Intune e sua atribuição aos grupos. | Sim | Não |
|_DeviceManagementConfiguration.ReadWrite.All_ | Ler e escrever as configurações de dispositivo e as políticas do Microsoft Intune  | Permite que o aplicativo leia e registre as propriedades de configuração de dispositivo e as políticas de conformidade de dispositivo do Microsoft Intune e sua atribuição aos grupos. | Sim | Não |
|_DeviceManagementManagedDevices.PrivilegedOperations.All_ | Executar ações remotas de impacto no usuário nos dispositivos do Microsoft Intune | Permite que o aplicativo execute ações remotas de alto impacto como apagar dispositivo ou redefinir a senha em dispositivos gerenciados pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementManagedDevices.Read.All_ | Ler dispositivos do Microsoft Intune | Permite que o aplicativo leia as propriedades de dispositivos gerenciados pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementManagedDevices.ReadWrite.All_ | Ler e registrar dispositivos do Microsoft Intune | Permite que o aplicativo leia e registre as propriedades de dispositivos gerenciados pelo Microsoft Intune. Não permite operações de alto impacto como apagamento remoto e a redefinição de senha no proprietário do dispositivo. | Sim | Não |
|_DeviceManagementRBAC.Read.All_ | Ler as configurações RBAC (Controle de Acesso com Base em Função) do Microsoft Intune | Permite que o aplicativo leia as propriedades relacionadas às configurações RBAC do Microsoft Intune. | Sim | Não |
|_DeviceManagementRBAC.ReadWrite.All_ | Ler e registrar as configurações RBAC do Microsoft Intune | Permite que o aplicativo leia e registre as propriedades relacionadas às configurações RBAC do Microsoft Intune. | Sim | Não |
|_DeviceManagementServiceConfig.Read.All_ | Configuração de leitura Microsoft Intune | Permite que o aplicativo leia as propriedades do serviço do Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. | Sim | Não |
|_DeviceManagementServiceConfig.ReadWrite.All_ | Ler e registrar o Microsoft Intune | Permite que o aplicativo leia e registre propriedades do serviço do Microsoft Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_DeviceManagementApps.Read.All_ | Ler aplicativos do Microsoft Intune | Permite que o aplicativo leia as propriedades, as atribuições de grupo, o status de aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementApps.ReadWrite.All_ | Ler e registrar os aplicativos do Microsoft Intune | Permite que aplicativo leia e registre s propriedades, as atribuições de grupo, o status dos aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementConfiguration.Read.All_ | Ler a configuração de dispositivo e as políticas do Microsoft Intune | Permite que o aplicativo leia as propriedades de configuração de dispositivo e as políticas de conformidade de dispositivo do Microsoft Intune e sua atribuição aos grupos. | Sim | Não |
|_DeviceManagementConfiguration.ReadWrite.All_ | Ler e escrever as configurações de dispositivo e as políticas do Microsoft Intune  | Permite que o aplicativo leia e registre as propriedades de configuração de dispositivo e as políticas de conformidade de dispositivo do Microsoft Intune e sua atribuição aos grupos. | Sim | Não |
|_DeviceManagementManagedDevices.PrivilegedOperations.All_ | Executar ações remotas de impacto no usuário nos dispositivos do Microsoft Intune | Permite que o aplicativo execute ações remotas de alto impacto como apagar dispositivo ou redefinir a senha em dispositivos gerenciados pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementManagedDevices.Read.All_ | Ler dispositivos do Microsoft Intune | Permite que o aplicativo leia as propriedades de dispositivos gerenciados pelo Microsoft Intune. | Sim | Não |
|_DeviceManagementManagedDevices.ReadWrite.All_ | Ler e registrar dispositivos do Microsoft Intune | Permite que o aplicativo leia e registre as propriedades de dispositivos gerenciados pelo Microsoft Intune. Não permite operações de alto impacto como apagamento remoto e a redefinição de senha no proprietário do dispositivo. | Sim | Não |
|_DeviceManagementRBAC.Read.All_ | Ler as configurações RBAC (Controle de Acesso com Base em Função) do Microsoft Intune | Permite que o aplicativo leia as propriedades relacionadas às configurações RBAC do Microsoft Intune. | Sim | Não |
|_DeviceManagementRBAC.ReadWrite.All_ | Ler e registrar as configurações RBAC do Microsoft Intune | Permite que o aplicativo leia e registre as propriedades relacionadas às configurações RBAC do Microsoft Intune. | Sim | Não |
|_DeviceManagementServiceConfig.Read.All_ | Configuração de leitura Microsoft Intune | Permite que o aplicativo leia as propriedades do serviço do Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. | Sim | Não |
|_DeviceManagementServiceConfig.ReadWrite.All_ | Ler e registrar o Microsoft Intune | Permite que o aplicativo leia e registre propriedades do serviço do Microsoft Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. | Sim | Não |

### <a name="remarks"></a>Comentários

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Essas permissões só são válidas para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _DeviceManagementServiceConfiguration.Read.All_: Verificar o estado atual da assinatura do Intune (`GET /deviceManagement/subscriptionState`).
* _DeviceManagementServiceConfiguration.ReadWrite.All_: Criar novos Termos e Condições (`POST /deviceManagement/termsAndConditions`).
* _DeviceManagementConfiguration.Read.All_: Localizar o status da configuração de um dispositivo (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`).
* _DeviceManagementConfiguration.ReadWrite.All_: Atribuir uma política de conformidade do dispositivo para um grupo (`POST deviceCompliancePolicies/{id}/assign`).
* _DeviceManagementApps.Read.All_: Localizar todos os aplicativos da Windows Store publicados no Intune (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`).
* _DeviceManagementApps.ReadWrite.All_: Publicar um novo aplicativo (`POST /deviceAppManagement/mobileApps`).
* _DeviceManagementRBAC.Read.All_: Localizar uma atribuição de função pelo nome (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`).
* _DeviceManagementRBAC.ReadWrite.All_: Criar uma nova função personalizada (`POST /deviceManagement/roleDefinitions`).
* _DeviceManagementManagedDevices.Read.All_: Localizar um dispositivo gerenciado pelo nome (`GET /managedDevices/?$filter=deviceName eq 'My Device'`).
* _DeviceManagementManagedDevices.ReadWrite.All_: Remover um dispositivo gerenciado (`DELETE /managedDevices/{id}`).
* _DeviceManagementManagedDevices.PrivilegedOperations.All_: Redefinir a senha em um dispositivo gerenciado do usuário (`POST /managedDevices/{id}/resetPasscode`).

#### <a name="application"></a>Aplicativo

* _DeviceManagementServiceConfiguration.Read.All_: Verificar o estado atual da assinatura do Intune (`GET /deviceManagement/subscriptionState`).
* _DeviceManagementServiceConfiguration.ReadWrite.All_: Criar novos Termos e Condições (`POST /deviceManagement/termsAndConditions`).
* _DeviceManagementConfiguration.Read.All_: Localizar o status da configuração de um dispositivo (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`).
* _DeviceManagementConfiguration.ReadWrite.All_: Atribuir uma política de conformidade do dispositivo para um grupo (`POST deviceCompliancePolicies/{id}/assign`).
* _DeviceManagementApps.Read.All_: Localizar todos os aplicativos da Windows Store publicados no Intune (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`).
* _DeviceManagementApps.ReadWrite.All_: Publicar um novo aplicativo (`POST /deviceAppManagement/mobileApps`).
* _DeviceManagementRBAC.Read.All_: Localizar uma atribuição de função pelo nome (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`).
* _DeviceManagementRBAC.ReadWrite.All_: Criar uma nova função personalizada (`POST /deviceManagement/roleDefinitions`).
* _DeviceManagementManagedDevices.Read.All_: Localizar um dispositivo gerenciado pelo nome (`GET /managedDevices/?$filter=deviceName eq 'My Device'`).
* _DeviceManagementManagedDevices.ReadWrite.All_: Remover um dispositivo gerenciado (`DELETE /managedDevices/{id}`).
* _DeviceManagementManagedDevices.PrivilegedOperations.All_: Redefinir a senha em um dispositivo gerenciado do usuário (`POST /managedDevices/{id}/resetPasscode`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="mail-permissions"></a>Permissões de email

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Mail.Read_ |    Ler emails do usuário | Permite ao aplicativo ler emails em caixas de correio do usuário. | Não | Sim
| _Mail.ReadBasic_ |    Ler emails básicos do usuário | Permite que o aplicativo leia o e-mail na caixa de correio do usuário conectado, exceto o **corpo**, **bodyPreview**, **uniqueBody**, **anexos**, **extensões**, e quaisquer propriedades estendidas. Não inclui permissões para pesquisar mensagens. | Não | Não
| _Mail.ReadWrite_ |    Acesso de leitura e gravação aos emails do usuário | Permite ao aplicativo criar, ler, atualizar e excluir emails em caixas de correio do usuário. Não inclui a permissão para enviar emails.| Não | Sim
| _Mail.Read.Shared_ |    Ler email compartilhado e de usuário | Permite que o aplicativo leia os emails que o usuário pode acessar, incluindo os próprios contatos do usuário e os emails compartilhados. | Não | Não
| _Mail.ReadWrite.Shared_ |    Ler e registrar usuário e emails compartilhados | Permite que o aplicativo crie, leia, atualize e exclua emails que o usuário tem permissão de acessar, incluindo os emails compartilhados e os do próprio usuário. Não inclui a permissão para enviar emails. | Não | Não
| _Mail.Send_ |    Enviar email como um usuário | Permite ao aplicativo enviar emails como usuários na organização. | Não | Sim
| _Mail.Send.Shared_ |    Enviar email em nome de outras pessoas | Permite que o aplicativo enviar emails como o usuário conectado no, incluindo o envio de nome de terceiros. | Não | Não
| _MailboxSettings.Read_ |  Ler as configurações da caixa de correio do usuário | Permite ao aplicativo ler as configurações da caixa de correio do usuário. Não inclui a permissão para enviar emails. | Não | Sim
| _MailboxSettings.ReadWrite_ |  Leia e grave as configurações de caixa de correio do usuário | Permite ao aplicativo criar, ler, atualizar e excluir as configurações da caixa de correio do usuário. Não inclui permissão para enviar emails diretamente, mas permite que o aplicativo crie regras que podem encaminhar ou redirecionar mensagens. | Não | Sim
| _IMAP.AccessAsUser.All_ | Acesso de leitura e gravação aos emails do usuário via IMAP | Permite ao aplicativo ler, atualizar, criar e excluir emails das caixas de correio do usuário. Não inclui a permissão para enviar emails. | Não | Sim
| _POP.AccessAsUser.All_ | Acesso de leitura e gravação aos emails do usuário via POP | Permite ao aplicativo ler, atualizar, criar e excluir emails das caixas de correio do usuário. Não inclui a permissão para enviar emails. | Não | Sim
| _SMTP.Send_ | Enviar email como um usuário usando SMTP AUTH | Permite ao aplicativo enviar emails como usuários na organização. | Não | Sim

#### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão                  | Exibir Cadeia de Caracteres                           | Descrição                                                                                                                                                                        | Consentimento Obrigatório do Administrador |
|:----------------------------|:-----------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------|
| _Mail.Read_                 | Ler emails em todas as caixas de correio               | Permite ao aplicativo ler emails em todas as caixas de correio sem um usuário conectado.                                                                                                             | Sim                    |
| _Mail.ReadBasic.All_        | Ler emails básicos de todos usuários                 | Permite que o aplicativo leia as caixas de correio de todos os usuários, exceto Body, BodyPreview, UniqueBody, Attachments, ExtendedProperties e Extensions. Não inclui permissões para pesquisar mensagens. | Sim                    |
| _Mail.ReadWrite_            | Ler e gravar emails em todas as caixas de correio     | Permite ao aplicativo criar, ler, atualizar e excluir emails em todas as caixas de correio sem um usuário conectado. Não inclui a permissão para enviar emails.                                       | Sim                    |
| _Mail.Send_                 | Enviar email como qualquer usuário                    | Permite ao aplicativo enviar emails como qualquer usuário sem um usuário conectado.                                                                                                                  | Sim                    |
| _MailboxSettings.Read_      | Ler as configurações de caixa de correio do usuário           | Permite que o aplicativo leia configurações da caixa de correio do usuário sem um usuário conectado. Não inclui a permissão para enviar emails.                                                                 | Não                     |
| _MailboxSettings.ReadWrite_ | Ler e gravar todas as configurações de caixa de correio do usuário | Permite que o aplicativo crie, leia, atualize e exclua as configurações da caixa de correio sem um usuário conectado. Não inclui a permissão para enviar emails.                                     | Sim                    |

> Os Administradores **Importantes** podem configurar a [política de acesso ao aplicativo](auth-limit-mailbox-access.md) para limitar o acesso do aplicativo às caixas de correio _específicas_ e não a todas as caixas de correio na organização, mesmo que as permissões de aplicativo do Mail.Read, Mail.ReadWrite, Mail.Send, MailboxSettings.Read, ou MailboxSettings.ReadWrite sejam concedidas ao aplicativo. 


### <a name="remarks"></a>Comentários

_Mail.Read.Shared_, _Mail.ReadWrite.Shared_, e _Mail.Send.Shared_ só são válidos para contas corporativas ou de estudante. Todas as demais permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante.

Com a permissão _Mail.Send_ ou _Mail.Send.Shared_, um aplicativo pode enviar emails e salvar uma cópia na pasta Itens Enviados do usuário, mesmo se o aplicativo não usar uma permissão _Mail.ReadWrite_ ou _Mail.ReadWrite.Shared_ correspondente.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Mail.Read_: Listar mensagens na caixa de entrada do usuário classificadas por `receivedDateTime` (`GET /me/mailfolders/inbox/messages?$orderby=receivedDateTime DESC`).
* _Mail.Read.Shared_: Localizar todas as mensagens com anexos na caixa de entrada de um usuário que compartilhou sua caixa de entrada com o usuário conectado (`GET /users{id | userPrincipalName}/mailfolders/inbox/messages?$filter=hasAttachments eq true`).
* _Mail.ReadWrite_: Marcar uma mensagem lida (`PATCH /me/messages/{id}`).
* _Mail.Send_: Enviar uma mensagem (`POST /me/sendmail`).
* _MailboxSettings.ReadWrite_: Atualizar a resposta automática do usuário (`PATCH /me/mailboxSettings`).

#### <a name="application"></a>Aplicativo

* _Mail.Read_: Localizar mensagens de pedro@contoso.com (`GET /users/{id | userPrincipalName}/messages?$filter=from/emailAddress/address eq 'bob@contoso.com'`).
* _Mail.ReadWrite_: Criar uma nova pasta na Caixa de Entrada chamada `Expense Reports` (`POST /users/{id | userPrincipalName}/mailfolders`).
* _Mail.Send_: Enviar uma mensagem (`POST /users/{id | userPrincipalName}/sendmail`).
* _MailboxSettings.Read_: Obter o fuso horário padrão para a caixa de correio do usuário (`GET /users/{id | userPrincipalName}/mailboxSettings/timeZone`)


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="managed-tenant-permissions"></a>Permissões de locatário gerenciado

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ManagedTenants.Read.All_ | Ler todas as informações específicas do locatário gerenciado | Permite que o aplicativo leia todas as informações do locatário gerenciado em nome do usuário conectado. | Sim | Não |
| _ManagedTenants.ReadWrite.All_ | Ler e gravar todas as informações específicas do locatário gerenciado | Permite que o aplicativo leia e grave todas as informações do locatário gerenciado em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

Nenhum.

---

## <a name="member-permissions"></a>Permissões de membro

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Member.Read.Hidden_ | Ler associações ocultas | Permite que o aplicativo leia as associações de grupos e unidades administrativas ocultos em nome do usuário conectado para aqueles grupos e unidades administrativas ocultos aos quais o usuário conectado tem acesso. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _Member.Read.Hidden_ | Ler todas as associações ocultas | Permite que o aplicativo leia as associações de grupos ocultos e unidades administrativas sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários
_Member.Read.Hidden_ é válida somente para contas corporativas ou de estudante.

A associação pode estar oculta em alguns grupos do Office 365. Isso significa que somente os membros do grupo podem exibir seus membros. Esse recurso pode ser usado para ajudar a cumprir regulamentos que exijam que uma organização oculte a associação ao grupo de pessoas externas (por exemplo, um grupo do Microsoft 365 que representa os alunos registrados em uma classe).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Member.Read.Hidden_: Ler os membros de uma unidade administrativa com associação oculta em nome do usuário conectado (`GET /administrativeUnits/{id}/members`).
* _Member.Read.Hidden_: Ler os membros de um grupo com associação oculta em nome do usuário conectado (`GET /groups/{id}/members`).

#### <a name="application"></a>Aplicativo

* _Member.Read.Hidden_: Ler os membros de uma unidade administrativa com associação oculta (`GET /administrativeUnits/{id}/members`).
* _Member.Read.Hidden_: Ler os membros de um grupo com associação oculta (`GET /groups/{id}/members`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="notes-permissions"></a>Permissões de anotações

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Notes.Read_ |    Ler blocos de anotações do OneNote do usuário | Permite ao aplicativo ler os títulos dos blocos de anotações e seções do OneNote e criar novas páginas, blocos de anotações e seções em nome do usuário conectado. | Não | Sim
| _Notes.Create_ |    Criar blocos de anotações do OneNote do usuário | Permite ao aplicativo ler os títulos dos blocos de anotações e seções do OneNote e criar novas páginas, blocos de anotações e seções em nome do usuário conectado.| Não | Sim
| _Notes.ReadWrite_ |    Ler e gravar blocos de anotações do OneNote do usuário | Permite ao aplicativo ler, compartilhar e modificar blocos de anotações do OneNote em nome do usuário conectado. | Não | Sim
| _Notes.Read.All_ |    Ler todos os blocos de anotações do OneNote que o usuário pode acessar | Permite que o aplicativo leia os blocos de anotações do OneNote aos quais o usuário conectado tem acesso dentro da organização. | Não | Não
| _Notes.ReadWrite.All_ |    Ler e gravar todos os blocos de anotações do OneNote que o usuário pode acessar | Permite que o aplicativo leia, compartilhe e modifique blocos de anotações do OneNote aos quais o usuário conectado tem acesso dentro da organização.| Não | Não
| _Notes.ReadWrite.CreatedByApp_ |    Acesso limitado ao bloco de anotações (preterido) | **Preterido** <br/>Não usar. Essa permissão não concede privilégios. | Não | Não

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _Notes.Read.All_ |    Ler todos os blocos de anotações do OneNote | Permite que o aplicativo leia todos os blocos de anotações do OneNote em sua organização sem um usuário conectado. | Sim |
| _Notes.ReadWrite.All_ |    Ler e gravar todos os blocos de anotações do OneNote | Permite que o aplicativo leia, compartilhe e modifique todos os blocos de anotações do OneNote em sua organização sem um usuário conectado.| Sim |


### <a name="remarks"></a>Comentários
_Notes.Read.All_ e _Notes.ReadWrite.All_ só são válidos para contas corporativas ou de estudante. Todas as demais permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante.

Com a permissão _Notes.Create_, um aplicativo pode exibir a hierarquia do bloco de anotações do OneNote do usuário conectado e criar conteúdo do OneNote (blocos de anotações, grupos de seção, seções, páginas, etc.).

_Notes.ReadWrite_ e _Notes.ReadWrite.All_ também permitem que o aplicativo modifique as permissões no conteúdo do OneNote que pode ser acessado pelo usuário conectado.

Para contas corporativas ou de estudante, _Notes.Read.All_ e _Notes.ReadWrite.All_ permitem que o aplicativo acesse o conteúdo do OneNote de outros usuários ao qual o usuário conectado tenha permissão dentro da organização.

### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegado

* _Notes.Create_: Criar novos blocos de anotações para o usuário conectado (`POST /me/onenote/notebooks`).
* _Notes.Read_: Criar blocos de anotações para o usuário conectado (`GET /me/onenote/notebooks`).
* _Notes.Read.All_: Obter todos os blocos de anotações aos quais o usuário conectado tenha acesso dentro da organização (`GET /me/onenote/notebooks?includesharednotebooks=true`).
* _Notes.ReadWrite_: Atualizar a página do usuário conectado (`PATCH /me/onenote/pages/{id}/$value`).
* _Notes.ReadWrite.All_: Criar uma página no bloco de anotações de outro usuário ao qual o usuário conectado tenha acesso dentro da organização (`POST /users/{id}/onenote/pages`).

#### <a name="application"></a>Aplicativo

* _Notes.Read.All_: Ler todos os blocos de anotações de usuários em um grupo (`GET /groups/{id}/onenote/notebooks`).
* _Notes.ReadWrite.All_: Atualizar a página em um bloco de anotações para qualquer usuário da organização (`PATCH /users/{id}/onenote/pages/{id}/$value`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="notifications-permissions"></a>Permissões de notificações
#### <a name="delegated-permissions"></a>Permissões delegadas
|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notifications.ReadWrite.CreatedByApp_ | Exibir e gerenciar notificações para esse aplicativo. | Permitir que o aplicativo forneça notificações em nome de usuários conectados. Também permite que o aplicativo leia, atualize e exclua itens de notificação do usuário para este aplicativo. |Não |
### <a name="remarks"></a>Comentários
*Notifications.ReadWrite.CreatedByApp* é válido para contas Microsoft e contas de trabalho ou estudante. A restrição *CreatedByApp* associada a esta permissão indica que o serviço aplicará a filtragem implícita aos resultados com base na identidade do aplicativo de chamada, seja o ID do aplicativo da conta Microsoft ou um conjunto de IDs do aplicativo configurado para uma plataforma cruzada identidade do aplicativo.
### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegated
* _Notifications.ReadWrite.CreatedByApp_: publica uma notificação centrada no usuário, que pode então ser entregue a vários clientes de aplicativos do usuário em execução em terminais diferentes.(POST/me/notificações/).

---

## <a name="online-meetings-permissions"></a>Permissões de reuniões online

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_OnlineMeetings.Read_|Ler Reunião Online.|Permite que um aplicativo leia detalhes da reunião online em nome do usuário conectado.|Não|Não|
|_OnlineMeetings.ReadWrite_|Leia e Crie Reuniões Online.|Permite que um aplicativo crie e leia as reuniões online em nome do usuário conectado. |Não|Não|
|_OnlineMeetingArtifact.Read.All_|Ler artefatos de Reunião Online.|Permite que o aplicativo leia os artefatos da reunião online em nome do usuário conectado. |Não|Não|

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_OnlineMeetings.Read.All_|Ler detalhes de Reunião Online do aplicativo |Permite que o aplicativo leia os detalhes da Reunião Online em sua organização, sem um usuário conectado.|Sim|
|_OnlineMeetings.ReadWrite.All_|Ler detalhes de Reunião Online a partir do aplicativo|Permite que um aplicativo crie e leia as Reuniões Online sem um usuário conectado.|Sim|
|_OnlineMeetingArtifact.Read.All_|Ler artefatos de Reunião Online do aplicativo |Permite que o aplicativo leia os artefatos da Reunião Online em sua organização, sem um usuário conectado.|Sim|

> **Importante** os administradores podem configurar [política de acesso a aplicativos](cloud-communication-online-meeting-application-access-policy.md) para permitir que os aplicativos acessem as reuniões online em nome de um usuário.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _OnlineMeetings.Read_: recuperar as propriedades e as relações de uma [reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) (`GET /beta/communications/onlinemeetings/{default id}`).
* _OnlineMeetings.ReadWrite_: criar um [reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) (`POST /beta/communications/onlinemeetings`).

#### <a name="application"></a>Aplicativo

* _OnlineMeetings.Read.All_
  * Recuperar as propriedades e os relacionamentos de uma[reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) (`GET /beta/communications/onlinemeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'`).
  * Recuperar uma [reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) em nome de um usuário(`GET /beta/users/{userId}/onlineMeetings/{id})
* _OnlineMeetings.ReadWrite.All_
  * Criar uma [reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) em nome de um usuário (`POST /beta/users/{userId}/onlineMeetings/)
  * Atualizar uma [reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) em nome de um usuário(`PATCH /beta/users/{userId}/onlineMeetings/{id})
  * Excluir uma [reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) em nome de um usuário (`DELETE /beta/users/{userId}/onlineMeetings/{id})
  
> **Observação**: criar uma [reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) cria uma reunião em nome de um usuário, mas não a mostra no Calendário do usuário.

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="on-premises-publishing-profiles-permissions"></a>Permissões de Perfis de Publicações Locais

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| OnPremisesPublishingProfiles.ReadWrite.All |    Acessar Perfis de Publicações Locais| Permite que o aplicativo gerencie a configuração do serviço de identidade híbrida criando, exibindo, atualizando e excluindo recursos de publicações locais, agentes locais e grupos de agentes, em nome do usuário conectado. | Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| OnPremisesPublishingProfiles.ReadWrite.All |    Acessar Perfis de Publicações Locais| Permite que o aplicativo gerencie a configuração do serviço de identidade híbrida criando, exibindo, atualizando e excluindo recursos de publicações locais, agentes locais e grupos de agentes, em nome do usuário conectado. | Não | Não |

---

## <a name="openid-connect-oidc-scopes"></a>Escopos do OpenID Connect (OIDC)

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _email_ |    Exibir o endereço de email do usuário | Permite ao aplicativo ler o endereço de email principal do usuário. | Não | Sim |
| _offline_access_ |    Acessar dados do usuário a qualquer momento | Permite ao aplicativo ler e atualizar dados do usuário, mesmo quando eles não estiver usando o aplicativo.| Não | Sim |
| _openid_ |    Conectar os usuários | Ao usar esta permissão, um aplicativo pode receber um identificador exclusivo para o usuário na forma de uma sub solicitação. A permissão também dá ao aplicativo acesso ao ponto de extremidade UserInfo. O escopo openid pode ser usado no ponto de extremidade da plataforma de identidade da Microsoft token para adquirir tokens de ID. O aplicativo pode usar esses tokens para autenticação.| Não | Sim |
| _profile_ |    Exibir os perfis básicos dos usuários | Permite que o aplicativo veja o perfil básico do usuário (nome, foto, nome de usuário).| Não | Sim |

### <a name="remarks"></a>Comentários
Você pode usar esses escopos para especificar os artefatos que deseja que sejam retornados nas solicitações de token e de autorização do Azure AD. O suporte a elas é oferecido de formas diferentes nos pontos de extremidade v 1.0 e v 2.0. do Azure AD.

Com o ponto de extremidade v 1.0 do Azure AD, somente o escopo _openid_ é usado. Você especifica no parâmetro do *escopo*, em uma solicitação de autorização, para retornar um token de ID quando usar o protocolo OpenID Connect para conectar um usuário ao seu aplicativo. Para saber mais, confira [Autorizar acesso aos aplicativos web usando o OpenID Connect e o Azure Active Directory](/azure/active-directory/develop/active-directory-protocols-openid-connect-code). Para retornar com êxito um token de ID, você também deve garantir que a permissão _User.Read_ esteja configurada quando você registrar seu aplicativo.

Com o ponto de extremidade v 2.0 do Azure AD, você especifica o escopo _offline\_acesso_ no parâmetro _escopo_ para solicitar explicitamente um token de atualização quando estiver usando os protocolos OAuth 2.0 ou OpenID Connect. Com o OpenID Connect, você especifica a permissão _openid_ para solicitar um token de ID. Também é possível especificar o escopo _email_, o escopo _perfil_, ou ambos, para retornar solicitações adicionais no token de ID. Você não precisa especificar a permissão _User.Read_ para retornar um token de ID com o ponto de extremidade v 2.0. Para saber mais, confira [escopos do OpenID Connect](/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes).

> [!IMPORTANT]
> 
> A Biblioteca de Autenticação da Microsoft (MSAL) atualmente especifica _offline\_acesso_, _openid_, _perfil_, e _email_ por padrão nas solicitações de autorização e de token. Isso significa que, para o caso padrão, se você especificar explicitamente esses escopos, o Azure AD pode retornar um erro.

---

## <a name="organization-permissions"></a>Permissões da organização

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Organization.Read.All_ |Ler informações da organização | Permite que o aplicativo leia a organização e os recursos relacionados em nome do usuário conectado.  Os recursos relacionados incluem itens como SKUs inscritos e informações de identidade visual do locatário.|Sim | Não |
| _Organization.ReadWrite.All_ |Ler e gravar informações da organização | Permite que o aplicativo leia e grave a organização e os recursos relacionados em nome do usuário conectado.  Os recursos relacionados incluem itens como SKUs inscritos e informações de identidade visual do locatário. |Sim | Não |

<br/>

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Organization.Read.All_ |Ler informações da organização | Permite que o aplicativo leia a organização e os recursos relacionados sem um usuário conectado.  Os recursos relacionados incluem itens como SKUs inscritos e informações de identidade visual do locatário. | Sim |
| _Organization.ReadWrite.All_ |Ler e gravar informações da organização | Permite que o aplicativo leia e grave a organização e os recursos relacionados sem um usuário conectado.  Os recursos relacionados incluem itens como SKUs inscritos e informações de identidade visual do locatário. |Sim |


### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado	

* _Organization.Read.All_: Obter informações da organização (`GET /organization`).
* _Organization.Read.All_: Obter as SKUs inscritas pela organização (`GET /subscribedSkus`).

#### <a name="application"></a>Aplicação

* _Organization.ReadWrite.All_: Atualizar as informações da organização (como **technicalNotificationMails**) (`PATCH /organization/{id}`).

---

## <a name="organizational-contact-permissions"></a>Permissões de contato organizacional

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _OrgContact.Read.All_ | Contatos organizacionais|Permite ao aplicativo ler todos os contatos organizacionais em nome do usuário conectado. Esses contatos são gerenciados pela organização e são diferentes dos contatos pessoais de um usuário.|Sim | Não |

<br/>

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _OrgContact.Read.All_ |Contatos organizacionais | Permite ao aplicativo ler todos os contatos organizacionais sem um usuário conectado.  Esses contatos são gerenciados pela organização e são diferentes dos contatos pessoais de um usuário. | Sim |

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado	

* _OrgContact.Read.All_: Obter todos os contatos organizacionais (`GET /contacts`).

---

## <a name="people-permissions"></a>Permissões de pessoas

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _People.Read_ |    Ler listas de pessoas relevantes dos usuários | Permite ao aplicativo ler uma lista pontuada de pessoas relevantes para o usuário conectado. A lista pode incluir contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype). | Não | Sim |
| _People.Read.All_ | Ler listas de pessoas relevantes de todos os usuários | Permite ao aplicativo ler uma lista pontuada de pessoas relevantes para o usuário conectado ou para outros usuários da organização do usuário conectado. A lista pode incluir contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype). Também permite que o aplicativo pesquise todo o diretório da organização do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read.All_ | Ler listas de pessoas relevantes de todos os usuários | Permite ao aplicativo ler uma lista pontuada de pessoas relevantes para o usuário conectado ou para outros usuários da organização do usuário conectado. <br/><br/>A lista pode incluir contatos locais, contatos de redes sociais ou do diretório da organização, e pessoas de comunicações recentes (como email e Skype). Também permite que o aplicativo pesquise todo o diretório da organização do usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

A permissão People.Read.All só é válida para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado
* _People.Read_: Ler uma lista de pessoas relevantes (`GET /me/people`)
* _People.Read.All_: Ler uma lista de pessoas relevantes para outro usuário na mesma organização (`GET /users('{id})/people`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="privileged-access-permissions"></a>Permissões de acesso privilegiadas

#### <a name="delegated-permissions"></a>Permissões delegadas

| Permissão | Exibir Cadeia de Caracteres | Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:---------- |:-------------- |:----------- |:---------------------- |:----------------- |
| _PrivilegedAccess.ReadWrite.AzureAD_ |Ler e gravar dados do Privileged Identity Management para diretório  | Permite que o aplicativo tenha acesso de leitura e gravação nas APIs do Privileged Identity Management do Azure AD. | Sim | Não |
| _PrivilegedAccess.ReadWrite.AzureADGroup_ |Leitura e escrita de dados do Privileged Identity Management para grupos de acesso privilegiado | Permite que o aplicativo tenha acesso de leitura e escrita às APIs de Privileged Identity Management para grupos. | Sim | Não |
| _PrivilegedAccess.ReadWrite.AzureResources_ |Ler e gravar dados Privileged Identity Management de recursos do Azure | Permite que o aplicativo tenha acesso de leitura e gravação nas APIs do Privileged Identity Management dos recursos do Azure. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão | Exibir Cadeia de Caracteres | Descrição | Consentimento Obrigatório do Administrador |
|:---------- |:-------------- |:----------- |:---------------------- |
| _PrivilegedAccess.Read.AzureAD_ |Leitura do Privileged Identity Management para Diretório  | Permite que o aplicativo tenha acesso de leitura às APIs do Privileged Identity Management para o Microsoft Azure AD. | Sim |
| _PrivilegedAccess.Read.AzureADGroup_ |Leitura do Privileged Identity Management para grupos de acesso privilegiado | Permite que o aplicativo tenha acesso de leitura às APIs do Privileged Identity Management para grupos. | Sim |
| _PrivilegedAccess.Read.AzureResources_ |Leitura do Privileged Identity Management para recursos do Azure | Permite que o aplicativo tenha acesso de leitura às APIs do Privileged Identity Management para os recursos do Microsoft Azure AD. | Sim |

---

## <a name="places-permissions"></a>Permissões de locais

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Place.Read.All_ |   Ler todos os locais da empresa | Permite que o aplicativo leia os locais da empresa (salas de conferência e listas de salas) que foram configurados pelo locatário no Exchange Online. |Sim | Não |
| _Place.ReadWrite.All_ |   Ler e gravar todos os locais da empresa | Permite que o aplicativo leia e grave os locais da empresa (salas de conferência e listas de salas) que foram configurados pelo locatário no Exchange Online. |Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Place.Read.All_ |   Ler todos os locais da empresa | Permite que o aplicativo leia os locais da empresa (salas de conferência e listas de salas) para eventos de calendário e outros aplicativos.| Sim |

---

## <a name="policy-permissions"></a>Permissões de política

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Policy.Read.All_ | Ler as políticas da sua organização | Permite ao aplicativo ler as políticas da sua organização em nome do usuário conectado. | Sim | Não |
| _Policy.Read.PermissionGrant_ | Ler políticas de concessão de consentimento e permissão | Permite que o aplicativo leia políticas relacionadas a concessões de consentimento e permissão para aplicativos, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.AccessReview_ |   Ler e gravar a política de autorização da sua organização  | Permite ao aplicativo ler e gravar a política de revisão de acesso da sua organização em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.ApplicationConfiguration_ | Leia e escreva as políticas de configuração dos aplicativos da sua organização | Permite que o aplicativo leia e grave as políticas de configuração dos aplicativos da sua organização em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.AuthenticationFlows_ | Ler e gravar as políticas de fluxo de autenticação da sua organização | Permite que o aplicativo leia e grave as políticas de fluxo de autenticação, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.AuthenticationMethod_        | Ler e gravar políticas do método de autenticação       | Permite que o aplicativo leia e grave as políticas do método de autenticação, em nome do usuário conectado. O usuário conectado também deve ser atribuído a função de Administrador Global. | Sim | Não |
| _Policy.ReadWrite.Authorization_ | Ler e gravar a política de autorização da sua organização | Permite que o aplicativo leia e grave a política de autorização da sua organização, em nome do usuário conectado.  Por exemplo, as políticas de autorização podem controlar algumas das permissões que a função do usuário pronto tem por padrão. | Sim | Não |
| _Policy.ReadWrite.ConditionalAccess_ | Ler e gravar as políticas de acesso condicional da sua organização | Permite que o aplicativo leia e grave todas as políticas de acesso condicional em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.ConsentRequest_ | Ler e escrever a política de solicitações de consentimento da sua organização | Permite que o aplicativo leia e grave a política de solicitações de consentimento da sua organização, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.CrossTenantAccess_ | Ler e gravar a política de acesso entre os locatários da sua organização | Permita que o aplicativo leia e grave a política de acesso entre locatários da sua organização em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.FeatureRollout_ | Ler e gravar as políticas de implantação de novos recursos da sua organização | Permite que o aplicativo leia e grave todas as políticas de implantação de novos recursos em nome do usuário conectado. Inclui habilidades para atribuir e remover usuários e grupos para a implantação de um recurso específico. | Sim | Não |
| _Policy.ReadWrite.PermissionGrant_ | Gerenciar as políticas de concessão de consentimento e permissão | Permite que o aplicativo gerencie as políticas relacionadas a concessões de consentimento e permissão para aplicativos, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.TrustFramework_ | Ler e gravar as políticas TrustFramework (Estrutura de Confiança) da sua organização | Permite que o aplicativo leia e grave todas as políticas de TrustFramework da sua organização em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.AuthenticationMethod_ | Ler e gravar as políticas de método de autenticação da sua organização | Permite que o aplicativo leia e grave as políticas do método de autenticação, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.MobilityManagement_ | Ler e gravar as políticas de gerenciamento de mobilidade da sua organização. | Permite ao aplicativo ler e gravar as políticas de gerenciamento de mobilidade da sua organização em nome do usuário conectado. Controlam as configurações para MDM (gerenciamento de dispositivo móvel) e aplicativos de gerenciamento de aplicativo móvel (MAM). | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _Policy.Read.All_ | Leia as políticas da sua organização | Permite que o aplicativo leia todas as políticas da sua organização sem um usuário conectado. | Sim |
| _Policy.Read.PermissionGrant_ | Ler políticas de concessão de consentimento e permissão | Permite que o aplicativo leia políticas relacionadas a concessões de consentimento e permissão para aplicativos, sem um usuário conectado. | Sim |
| _Policy.Read.ApplicationConfiguration_ | Leia as políticas de configuração dos aplicativos da sua organização | Permite que o aplicativo leia todas as políticas de configuração dos aplicativos da sua organização sem um usuário conectado. | Sim |
| _Policy.ReadWrite.AccessReview_ | Ler e gravar a política de autorização da sua organização | Permite ao aplicativo ler e gravar a política de revisão de acesso da sua organização, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.ApplicationConfiguration_ | Leia e escreva as políticas de configuração dos aplicativos da sua organização | Permite que o aplicativo leia e grave as políticas de configuração dos aplicativos da sua organização, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.AuthenticationFlows_ | Ler e gravar as políticas de fluxo de autenticação da sua organização | Permite que o aplicativo leia e grave todas as políticas de fluxo de autenticação do locatário, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.Authorization_ | Ler e gravar a política de autorização da sua organização | Permite que o aplicativo leia e grave a política de autorização da sua organização, em nome do usuário conectado.  Por exemplo, as políticas de autorização podem controlar algumas das permissões que a função do usuário pronto tem por padrão. | Sim | 
| _Policy.ReadWrite.ConsentRequest_ | Ler e escrever a política de solicitações de consentimento da sua organização | Permite que o aplicativo leia e escreva a política de solicitações de consentimento da sua organização sem um usuário conectado. | Sim |
| _Policy.ReadWrite.CrossTenantAccess_ | Ler e gravar a política de acesso entre os locatários da sua organização | Permita que o aplicativo leia e grave a política de acesso entre locatários da sua organização sem um usuário conectado. | Sim |
| _Policy.ReadWrite.AuthenticationMethod_   | Ler e gravar todas as políticas de método de autenticação    | Permite que o aplicativo leia e grave todas as políticas de método de autenticação do locatário, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.FeatureRollout_ | Políticas de distribuição de recursos de leitura e gravação | Permite que o aplicativo leia e grave todas as políticas de distribuição de recursos sem um usuário conectado. Inclui habilidades para atribuir e remover usuários e grupos para a implantação de um recurso específico. | Sim |
| _Policy.ReadWrite.PermissionGrant_ | Gerenciar as políticas de concessão de consentimento e permissão | Permite que o aplicativo gerencie as políticas relacionadas às concessões de consentimento e permissão para aplicativos, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.TrustFramework_ | Ler e gravar as políticas da estrutura de confiança da sua organização | Permite que o aplicativo leia e grave todas as políticas da estrutura de confiança da sua organização sem um usuário conectado. | Sim |

### <a name="example-usage"></a>Exemplo de uso

Os seguintes usos são válidos para permissões delegadas e permissões de aplicativo:

* _Policy.Read.All_: Ler as políticas da sua organização (`GET /policies`)
* _Policy.Read.All_: Ler as políticas da estrutura de confiança da sua organização (`GET /beta/trustFramework/policies`)
* _Policy.Read.All_: Ler as políticas de distribuição de recursos da sua organização (`GET /beta/directory/featureRolloutPolicies`)
* _Policy.ReadWrite.AccessReview_: Ler e gravar as políticas de revisão de acesso da sua organização (`PATCH /beta/policies/accessReviewPolicy`)
* _Policy.ReadWrite.ApplicationConfiguration_: Leia e grave as políticas de configuração dos aplicativos da sua organização (`POST /beta/policies/tokenLifetimePolicies`)
* _Policy.ReadWrite.AuthenticationFlows_: Ler e gravar a política de fluxos de autenticação da sua organização (`PATCH /beta/policies/authenticationFlowsPolicy`)
* _Policy.ReadWrite.AuthenticationMethod_: use as permissões para gerenciar as configurações na política de métodos de autenticação, incluindo habilitar e desabilitar métodos de autenticação, permitir que usuários e grupos usem esses métodos e definir outras configurações relacionadas aos métodos de autenticação que os usuários podem registrar e usar em um locatário.
* _Policy.ReadWrite.ConditionalAccess_: Leia e escreva as políticas de acesso condicional da sua organização (`POST /beta/identity/conditionalAccess/policies`)
* _Policy.ReadWrite.CrossTenantAccessPolicy_: leia e escreva a política de acesso entre locatários da sua organização (`PATCH /beta/policies/crossTenantAccessPolicy`)
* _Policy.ReadWrite.FeatureRollout_: Ler e gravar todas as políticas de distribuição de recursos da sua organização (`POST /beta/directory/featureRolloutPolicies`)
* _Policy.ReadWrite.TrustFramework_: Leitura e gravação de todas as políticas da estrutura de confiança da sua organização (`POST /beta/trustFramework/policies`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="presence-permissions"></a>Permissões de presença

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Presence.Read_ | Ler as informações de presença do usuário | Permite que o aplicativo leia as informações de presença em nome do usuário conectado. As informações de presença incluem atividade, disponibilidade, nota de status, calendário de mensagens de ausência temporária, fuso horário e local. | Não |
| _Presence.Read.All_ |   Ler as informações de presença de todos os usuários em sua organização | Permite que o aplicativo leia as informações de presença de todos os usuário do diretório em nome do usuário conectado. As informações de presença incluem atividade, disponibilidade, nota de status, calendário de mensagens de ausência temporária, fuso horário e local. | Não |
| _Presence.ReadWrite_ | Leia e escreva as informações de presença de um usuário | Permite que o aplicativo leia as informações de presença e grave a atividade e a disponibilidade em nome do usuário conectado. As informações de presença incluem atividade, disponibilidade, nota de status, calendário de mensagens de ausência temporária, fuso horário e local. | Sim |

#### <a name="application-permissions"></a>Permissões de aplicativos
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Presence.ReadWrite.All_ | Ler e escrever informações de presença para todos os usuários | Permite que o aplicativo leia todas as informações de presença e grave a atividade e a disponibilidade de todos os usuários no diretório sem um usuário conectado. As informações de presença incluem atividade, disponibilidade, nota de status, calendário de mensagens de ausência temporária, fuso horário e local. | Sim |

### <a name="example-usage"></a>Exemplo de uso

* _Presence.Read_: se você estiver conectado, recupere a sua própria informação de presença (`GET /me/presence`)
* _Presence.Read.All_: Recupere as informações de presença de outro usuário (`GET /users/{id}/presence`)
* _Presence.Read.All_: Recupere as informações de presença de vários usuários (`POST /communications/getPresencesByUserId`)
* _Presence.ReadWrite_:
  * Se você estiver conectado, defina o estado da sua sessão de presença (`POST /me/presence/setPresence`)
  * Se você estiver conectado, defina sua própria presença preferencial (`POST /me/presence/setUserPreferredPresence`)
* _Presence.ReadWrite.All_:
  * Definir o estado da sessão de presença de um usuário como um aplicativo (`POST /users/{id}/presence/setPresence`)
  * Definir a presença preferencial de um usuário como um aplicativo (`POST /users/{id}/presence/setUserPreferredPresence`)

---

## <a name="programs-and-program-controls-permissions"></a>Permissões de programas e controles de programas

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ProgramControl.Read.All_ |   Ler todos os programas  | Permite que o aplicativo leia programas em nome do usuário conectado. | Sim | Não |
| _ProgramControl.ReadWrite.All_ |   Gerenciar todos os programas  | Permite que o aplicativo leia e escreva programas em nome do usuário conectado. | Sim | Não |


#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _ProgramControl.Read.All_ |   Ler todos os programas | Permite que o aplicativo leia programas sem um usuário conectado. | Sim |
| _ProgramControl.ReadWrite.All_ |   Gerenciar todos os programas | Permite que o aplicativo leia e escreva programas sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

_ProgramControl.Read.All_ e _ProgramControl.ReadWrite.All_ são válidos apenas para contas de trabalho ou escola.

Para um aplicativo com permissões delegadas para ler programas e controles de programas, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador Global, Administrador de Segurança, Leitor de Segurança ou Administrador de Usuário. Para um aplicativo com permissões delegadas para gravar programas e controles de programas, o usuário conectado deve ser membro de uma das seguintes funções de administrador: Administrador Global ou Administrador do Usuário.  Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

---

## <a name="reports-permissions"></a>Permissões de relatórios

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Reports.Read.All_ | Ler todos os relatórios de uso | Permite que um aplicativo leia todos os relatórios de uso de serviço em nome do usuário conectado. Serviços que fornecem relatórios de uso incluem o Microsoft 365 e o Azure Active Directory. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _Reports.Read.All_ | Ler todos os relatórios de uso | Permite que um aplicativo leia todos os relatórios de uso de serviço sem um usuário conectado. Serviços que fornecem relatórios de uso incluem o Microsoft 365 e o Azure Active Directory. | Sim |

### <a name="remarks"></a>Comentários
- As permissões de relatórios só são válidas para contas corporativas ou de estudante.
- Para que as permissões delegadas permitam que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário uma função de administrador limitada do Azure Active Directory. Para obter mais detalhes, confira [Autorização para APIs para ler relatórios de uso do Microsoft 365](reportroot-authorization.md).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="application"></a>Aplicativo

* _Reports.Read.All_: Ler o relatório de detalhes de uso de aplicativos de email com período de 7 dias (`GET /reports/EmailAppUsage(view='Detail',period='D7')/content`).
* _Reports.Read.All_: Ler o relatório de detalhes de atividade de email com data de '2017-01-01' (`GET /reports/EmailActivity(view='Detail',data='2017-01-01')/content`).
* _Reports.Read.All_: Ler o relatório de detalhes de ativações do Microsoft 365 (`GET /reports/Office365Activations(view='Detail')/content`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="role-management-permissions"></a>Permissões do Gerenciamento de Funções

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _RoleAssignmentSchedule.Read.Directory_ | Leia todas as atribuições de funções ativas para o diretório da sua empresa. | Permite que o aplicativo leia as atribuições ativas de controle de acesso baseado em função (RBAC) para o diretório da sua empresa, em nome do usuário conectado. Isso inclui a leitura de modelos de função de diretório e funções de diretório. | Sim | Não |
| _RoleEligibilitySchedule.Read.Directory_ | Leia todas as atribuições de funções elegíveis para o diretório da sua empresa. | Permite que o aplicativo leia as atribuições qualificadas de controle de acesso baseado em função (RBAC) para o diretório da sua empresa, em nome do usuário conectado. Isso inclui a leitura de modelos de função de diretório e funções de diretório. | Sim | Não |
| _RoleManagement.Read.All_ | Leia os dados de gerenciamento de função para todos os provedores RBAC. | Permite que o aplicativo leia as configurações de controle de acesso baseado em função (RBAC) para todos os [provedores RBAC](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) com suporte, em nome do usuário conectado. Isso inclui a leitura de definições de funções e atribuições de funções. | Sim | Não |
| _RoleManagement.Read.Directory_ | Leia os dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de controle de acesso baseado em função (RBAC) da sua empresa, em nome do usuário conectado. Isso inclui a leitura de modelos de função de diretório, funções de diretório e associações. | Sim | Não |
| _RoleManagementPolicy.Read.Directory_ | Leia todas as políticas para tarefas de funções privilegiadas para o diretório da sua empresa. | Permite que o aplicativo leia políticas para tarefas de controle de acesso baseado em função privilegiada (RBAC) para o diretório de sua empresa, em nome do usuário conectado. | Sim | Não |
| _RoleAssignmentSchedule.ReadWrite.Directory_ | Leia, atualize e exclua todas as atribuições de funções ativas para o diretório da sua empresa. | Permite que o aplicativo leia e gerencie as atribuições ativas de controle de acesso baseado em função (RBAC) para o diretório da sua empresa, em nome do usuário conectado. Isso inclui o gerenciamento de associações de função de diretório ativo e leitura de modelos de função de diretório, funções de diretório e associações ativas. | Sim | Não |
| _RoleEligibilitySchedule.ReadWrite.Directory_ | Leia, atualize e exclua  todas as tarefas de funções elegíveis para o diretório da sua empresa. | Permite que o aplicativo leia e gerencie as tarefas de controle de acesso baseado em função (RBAC) qualificadas para o diretório da sua empresa, em nome do usuário conectado. Isso inclui o gerenciamento de associações de funções de diretório elegíveis e a leitura de modelos de funções de diretórios, funções de diretórios e associações elegíveis. | Sim | Não |
| _RoleManagement.ReadWrite.Directory_ | Ler e gravar dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de RBAC (controle de acesso baseado em função) da sua empresa, em nome do usuário conectado. Isso inclui a instanciação das funções de diretório, o gerenciamento de associação da função de diretório, a leitura dos modelos da função de diretório, as associações e as funções de diretório. | Sim | Não |
| _RoleManagementPolicy.ReadWrite.Directory_ | Leia, atualize e exclua todas as políticas para tarefas de funções privilegiadas para o diretório da sua empresa. | Permite que o aplicativo leia, atualize e exclua políticas para tarefas de controle de acesso baseado em função privilegiada (RBAC) para o diretório de sua empresa, em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _RoleManagement.Read.All_ | Leia os dados de gerenciamento de função para todos os provedores RBAC. | Permite que o aplicativo leia as configurações de controle de acesso baseado em função (RBAC) para todos os [provedores RBAC](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) com suporte, sem um usuário conectado. isso inclui a leitura de definições de funções e atribuições de funções. | Sim |
| _RoleManagement.Read.Directory_ | Leia os dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de RBAC (controle de acesso baseado em função) da sua empresa, em nome do usuário conectado. Isso inclui a leitura de modelos da função de diretório, as associações e as funções de diretório. | Sim |
| _RoleManagement.ReadWrite.Directory_ | Ler e gravar dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de controle de acesso baseado em função (RBAC) para o diretório da sua empresa, sem um usuário conectado. Isso inclui instanciar funções de diretório e gerenciamento de associação de função de diretório e leitura de modelos de função de diretório, funções de diretório e associações. | Sim |


### <a name="remarks"></a>Comentários

> [!CAUTION]
> Permissões que permitem a concessão de autorização, como _roleManagement.ReadWrite.Directory_, permitem que um aplicativo conceda a si mesmo, outros aplicativos ou qualquer usuário, privilégios adicionais. Tenha cuidado ao conceder qualquer uma dessas permissões.

Com a permissão _RoleManagement.Read.Directory_ um aplicativo pode ler directoryRoles e directoryRoleTemplates. Isso inclui a leitura de informações de associação para funções de diretório.

Com a permissão _RoleManagement.ReadWrite.Directory_, um aplicativo pode ler e gravar directoryRoles (directoryRoleTemplates são recursos somente leitura). Isso inclui adicionar e remover membros de funções de diretório.

As permissões de relatórios só são válidas para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

- _RoleManagement.Read.Directory_: Ler a lista de modelos de função disponíveis(`GET /directoryRoleTemplates`)
- _RoleManagement.Read.Directory_: Ler a lista de funções ativadas em seu diretório(`GET /directoryRoles`)
- _RoleManagement.Read.Directory_: Ler a lista de membros para uma função (`GET /directoryRoles/<id>/members`)
- _RoleManagement.Read.Directory_: Ler a lista de membros com escopo de unidade administrativa para uma função (`GET /directoryRoles/<id>/scopedMembers`)
- _RoleManagement.ReadWrite.Directory_: Ativar uma função de diretório a partir de um modelo de função (`POST /directoryRoles`)
- _RoleManagement.ReadWrite.Directory_: Adicionar um membro a uma função de diretório (`POST /directoryRoles/<id>/members`)
- _RoleManagement.ReadWrite.Directory_: Adicionar um membro de escopo de unidade administrativa a uma função de diretório(`POST /directoryRoles/<id>/scopedMembers`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="schedule-management-permissions-private-preview"></a>Permissões do gerenciamento de agenda ([visualização privada](#permissions-availability-status))

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Schedule.ReadWrite.All_ (visualização privada)| Dados do serviço de Turnos de Leitura e Gravação (Teams) | Permite que um aplicativo leia e grave a agenda, grupos de agendamento, turnos e entidades associadas em aplicativos de turnos sem um usuário conectado.| Sim | Não |
| _Schedule.Read.All_ (visualização privada)| Dados do serviço de Turnos de Leitura (Teams) | Permite que o aplicativo leia a agenda, grupos de agendamento, turnos e entidades associadas em aplicativos de turnos sem um usuário conectado.  | Sim | Não |

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _Schedule.ReadWrite.All_ | Dados do serviço de Turnos de Leitura e Gravação (Teams) | Permite que um aplicativo leia e escreva agenda, grupos de agendas, turnos e entidades associadas em aplicativos de turnos em nome do usuário conectado.| Não | Não |
| _Schedule.Read.All_ | Dados do serviço de Turnos de Leitura (Teams) | Permite que um aplicativo leia a agenda, grupos de agenda, turnos e entidades associadas em aplicativos de turnos em nome do usuário conectado.  | Não | Não |
| _WorkforceIntegration.ReadWrite.All_ (visualização particular)| Ler e gravar integrações de força de trabalho | Permite que o aplicativo gerencie integrações de força de trabalho, para sincronizar dados do Microsoft Teams, com um sistema integrado, em nome do usuário conectado.  | Sim | Não |
| _WorkforceIntegration.Read.All_ (visualização privada)| Ler e gravar integrações de força de trabalho | Permite que o aplicativo gerencie integrações de força de trabalho, para sincronizar dados do Microsoft Teams, com um sistema integrado, em nome do usuário conectado.  | Sim | Não |

## <a name="search-permissions"></a>Permissões de pesquisa

#### <a name="application-permissions"></a>Permissões de aplicativos
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ExternalConnection.Read.All_ | Ler todas as conexões externas | Permite que o aplicativo leia e grave conexões externas sem um usuário conectado. | Sim | Não |
| _ExternalConnection.ReadWrite.All_ | Ler e gravar todas as conexões externas | Permite que o aplicativo leia e grave todas as conexões externas sem um usuário conectado. | Sim | Não |
| _ExternalConnection.ReadWrite.OwnedBy_ | Leitura e gravação de conexões externas e configurações de conexão | Permite que o aplicativo faça leitura e gravação de conexões externas e suas configurações sem um usuário conectado. O aplicativo somente pode ler e gravar conexões externas às qual está autorizado ou pode criar novas conexões externas. | Sim | Não |
| _ExternalItem.Read.All_ | Ler todos os itens externos | Permite que o aplicativo faça leitura e gravação de todos os itens externos sem um usuário conectado. | Sim | Não |
| _ExternalItem.ReadWrite.All_ | Leitura e gravação de todos os itens externos | Permite que o aplicativo faça leitura e gravação de todos os itens externos sem um usuário conectado. | Sim | Não |
| _ExternalItem.ReadWrite.OwnedBy_ | Ler e gravar itens externos | Permite que o aplicativo leia e grave itens externos sem um usuário conectado. O aplicativo somente pode ler itens externos da conexão à qual está autorizado. | Sim | Não |

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _ExternalConnection.Read.All_ | Ler todas as conexões externas | Permite que o aplicativo leia todas as conexões externas em nome de um usuário conectado. | Sim | Não |
| _ExternalConnection.ReadWrite.All_ | Ler e gravar todas as conexões externas | Permite que o aplicativo leia e grave todas as conexões externas em nome de um usuário conectado. | Sim | Não |
| _ExternalConnection.ReadWrite.OwnedBy_ | Ler e gravar conexões externas | Permite que o aplicativo leia e escreva programas em nome do usuário conectado. O aplicativo somente pode ler e gravar conexões externas às qual está autorizado ou pode criar novas conexões externas. | Sim | Não |
| _ExternalItem.Read.All_ | Ler os dados externos | Permitir que o aplicativo leia conjuntos de dados externos e conteúdo em nome do usuário conectado. | Sim | Não |
| _ExternalItem.ReadWrite.All_ | Leitura e gravação de todos os itens externos | Permite que o aplicativo leia e grave todos os itens externos em nome de um usuário conectado. | Sim | Não |
| _ExternalItem.ReadWrite.OwnedBy_ | Ler e gravar itens externos | Permite que o aplicativo leia e grave itens externos em nome de um usuário conectado. O aplicativo somente pode ler itens externos da conexão à qual está autorizado. | Sim | Não |

### <a name="remarks"></a>Comentários
As permissões de pesquisa só são válidas para contas corporativas ou de estudante.

Esta permissão de pesquisa só se aplica aos dados ingeridos da API de indexação.

O acesso aos dados por meio de pesquisa requer permissão de leitura para o item. Por exemplo, _Files.Read.All_ para acessar arquivos por meio da pesquisa.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _ExternalItem.Read.All_ _: Acessar dados externos da [API de pesquisa](/graph/api/resources/search-api-overview) (`POST /search/query`).

---

## <a name="search-configuration-permissions"></a>Escolher permissões de configuração

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _SearchConfiguration.Read.All_ | Ler a configuração de pesquisa da sua organização | Permite que o aplicativo leia a configuração de pesquisa, em nome do usuário conectado. | Sim | Não |
| _SearchConfiguration.ReadWrite.All_ | Ler e gravar a configuração de pesquisa da sua organização | Permite que o aplicativo leia e grave configurações de pesquisa, em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | 
|:----------------|:------------------|:-------------|:-----------------------|
| _SearchConfiguration.Read.All_ | Ler a configuração de pesquisa da sua organização | Permite que o aplicativo leia as configurações de pesquisa, sem um usuário conectado. | Sim | 
| _SearchConfiguration.ReadWrite.All_ | Ler e gravar a configuração de pesquisa da sua organização | Permite que o aplicativo leia e grave configurações de pesquisa, sem um usuário conectado. | Sim | 


### <a name="remarks"></a>Comentários
As permissões de pesquisa só são válidas para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated-and-application"></a>Permissões delegadas e de aplicativo

- _SearchConfiguration.Read.All_: Leia a lista de todos os indicadores criados para seu locatário (`GET /beta/search/bookmarks`)
- _SearchConfiguration.ReadWrite.All_: Atualize ou leia todos os indicadores criados para seu locatário (`PATCH /beta/search/bookmarks/{id}`)

---

## <a name="security-permissions"></a>Permissões de segurança

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _SecurityEvents.Read.All_        |  Ler os eventos de segurança da organização | Permite ao aplicativo ler os eventos de segurança da sua organização em nome do usuário conectado. | Sim  | Não |
| _SecurityEvents.ReadWrite.All_   | Ler e atualizar os eventos de segurança da organização | Permite ao aplicativo ler os eventos de segurança da sua organização em nome do usuário conectado. Também permite ao aplicativo atualizar as propriedades editáveis em eventos de segurança em nome do usuário conectado. | Sim  | Não |
| _SecurityActions.Read.All_        |  Ler as ações de segurança da organização | Permite que o aplicativo leia as ações de segurança da sua organização em nome do usuário conectado. | Sim  | Não |
| _SecurityActions.ReadWrite.All_   | Ler e atualizar as ações de segurança da organização | Permite que o aplicativo leia ou atualize as ações de segurança da sua organização em nome do usuário conectado.  | Sim  | Não |
| _ThreatIndicators.ReadWrite.OwnedBy_   | Gerenciar indicadores de ameaças que este aplicativo cria ou é proprietário |Permite que o aplicativo crie indicadores de ameaças e gerencie totalmente esses indicadores de ameaças (ler, atualizar e excluir) em nome do usuário conectado.  | Sim  | Não |
| _ThreatIndicators.Read.All_   | Leia os indicadores de ameaças da sua organização | Permite que o aplicativo leia todos os indicadores de ameaça para sua organização, em nome do usuário conectado.  | Sim  | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _SecurityEvents.Read.All_        |  Ler os eventos de segurança da organização | Permite ao aplicativo ler os eventos de segurança da sua organização. | Sim  |
| _SecurityEvents.ReadWrite.All_   | Ler e atualizar os eventos de segurança da organização | Permite ao aplicativo ler os eventos de segurança da sua organização. Também permite ao aplicativo atualizar as propriedades editáveis em eventos de segurança. | Sim  |
| _SecurityActions.Read.All_        |  Ler os eventos de segurança da organização | Permite que o aplicativo leia os eventos de segurança da sua organização. | Sim  |
| _SecurityActions.ReadWrite.All_   | Criar e ler ações de segurança da sua organização | Permite que o aplicativo leia ou crie ações de segurança, sem um usuário ter entrado. | Sim  |
| _ThreatIndicators.ReadWrite.OwnedBy_   | Gerenciar indicadores de ameaças que este aplicativo cria ou é proprietário | Permite que o aplicativo crie indicadores de ameaças e gerencie totalmente esses indicadores de ameaças (ler, atualizar e excluir) sem um usuário ter entrado.  Ele não atualizará os indicadores de ameaças que não possui. | Sim  |
| _ThreatIndicators.Read.All_   | Gerenciar indicadores de ameaças que este aplicativo cria ou é proprietário | Permite que o aplicativo leia todos os indicadores de ameaça para sua organização, sem um usuário assinado. | Sim  |

### <a name="remarks"></a>Comentários

As permissões de segurança só são válidas para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated-and-application"></a>Permissões delegadas e de aplicativo

- _SecurityEvents.Read.All_: Ler a lista de todos os alertas de segurança de todos os provedores de segurança licenciados disponíveis para o seu locatário (`GET /beta/security/alerts`)
- _SecurityEvents.ReadWrite.All_: Atualize ou leia os alertas de segurança de todos os provedores de segurança licenciados disponíveis para o seu locatário (`PATCH /beta/security/alerts/{id}`)

---

## <a name="service-communications-permissions"></a>Permissões de comunicações de serviço

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres  | Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ServiceHealth.Read.All_ | Ler a integridade do serviço | Permite que o aplicativo leia as informações de integridade de serviço do seu locatário em nome do usuário inscrito. As informações de integridade podem incluir os problemas de serviço ou a visão geral de integridade do serviço. | Sim | Sim |
| _ServiceMessage.Read.All_ | Ler mensagens de serviço | Permite que o aplicativo leia as mensagens de anúncio de serviço do seu locatário em nome do usuário conectado. As mensagens podem incluir informações sobre os recursos novos ou alterados. | Sim | Sim |
| _ServiceMessageViewpoint.Write_ | Atualize seu status de usuário nas mensagens de anúncio de serviço | Permite que o aplicativo atualize o status do usuário das mensagens de anúncio de serviço em nome do usuário conectado. O status da mensagem pode ser marcado como lido, arquivo ou favorito. | Sim | Sim |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres  | Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _ServiceHealth.Read.All_ | Ler a integridade do serviço | Permite que o aplicativo leia as informações de integridade do serviço do seu locatário, sem um usuário conectado. As informações de integridade podem incluir os problemas de serviço ou a visão geral de integridade do serviço. | Sim |
| _ServiceMessage.Read.All_ | Ler mensagens de serviço | Permite que o aplicativo leia as mensagens de anúncio de serviço do seu locatário, sem um usuário conectado. As mensagens podem incluir informações sobre os recursos novos ou alterados. | Sim |

---

## <a name="short-notes-permissions-private-preview"></a>Permissões de Anotações Curtas ([visualização privada](#permissions-availability-status))

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres  | Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ShortNotes.Read_ | Ler anotações curtas do usuário conectado | Permite que o aplicativo leia todas as anotações curtas às quais um usuário conectado tenha acesso. | Não | Sim |
| _ShortNotes.ReadWrite_ | Ler, criar, editar e excluir anotações curtas do usuário conectado | Permite que o aplicativo leia, crie, edite e exclua anotações curtas de um usuário conectado. | Não | Sim |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _ShortNotes.Read.All_ | Ler as anotações curtas de todos os usuários | Permite que o aplicativo leia todas as anotações curtas sem um usuário conectado. | Sim |
| _ShortNotes.ReadWrite.All_ | Ler, criar, editar e excluir anotações curtas de todos os usuários | Permite ao aplicativo ler, criar, editar e excluir todas as anotações curtas sem um usuário conectado. | Sim |

---

## <a name="sites-permissions"></a>Permissões de sites

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Sites.Read.All_        | Ler itens em todos os conjuntos de sites | Permite ao aplicativo ler documentos e listar itens em todos os conjuntos de sites em nome do usuário conectado. | Não  | Não |
| _Sites.ReadWrite.All_   | Ler e gravar itens em todos os conjuntos de sites | Permite ao aplicativo editar ou excluir documentos e listar itens em todos os conjuntos de sites em nome do usuário conectado. | Não  | Não |
| _Sites.Manage.All_      | Criar, editar e excluir itens e listas em todos os conjuntos de sites | Permite ao aplicativo gerenciar e criar listas, documentos e listar itens em todos os conjuntos de sites em nome do usuário conectado. | Não | Não |
| _Sites.FullControl.All_ | Ter controle total de todos os conjuntos de sites | Permite ao aplicativo ter controle total nos sites do SharePoint em todos os conjuntos de sites em nome do usuário conectado.  | Sim  | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _Sites.Read.All_        | Ler itens em todos os conjuntos de sites | Permite ao aplicativo ler documentos e listar itens em todos os conjuntos de sites sem um usuário conectado. | Sim |
| _Sites.ReadWrite.All_   | Ler e gravar itens em todos os conjuntos de sites | Permite ao aplicativo criar, ler, atualizar e excluir documentos e listar itens em todos os conjuntos de sites sem um usuário conectado. | Sim |
| _Sites.Manage.All_      | Criar, editar e excluir itens e listas em todos os conjuntos de sites | Permite ao aplicativo gerenciar e criar listas, documentos e listar itens em todos os conjuntos de sites sem um usuário conectado.  | Sim  |
| _Sites.FullControl.All_ | Ter controle total de todos os conjuntos de sites | Permite ao aplicativo ter controle total nos sites do SharePoint em todos os conjuntos de sites sem um usuário conectado.  | Sim  |
| _Sites.Selecionados_ | Acessar conjuntos de sites selecionados | Permitir que o aplicativo acesse um subconjunto de conjuntos de sites sem um usuário conectado.  Os conjuntos de sites específicos e as permissões concedidas serão configurados no SharePoint Online. | Sim  |


### <a name="remarks"></a>Comentários

Essas permissões de sites só são válidas para contas corporativas ou de estudante.
A permissão do aplicativo _Sites.Selected_ está disponível apenas na API do Microsoft Graph.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Sites.Read.All_: Ler as listas no site raiz do SharePoint (`GET /v1.0/sites/root/lists`)
* _Sites.ReadWrite.All_: Criar novos itens de lista em uma lista do SharePoint (`POST /v1.0/sites/root/lists/123/items`)
* _Sites.Manage.All_: Adicionar uma nova lista a um site do SharePoint (`POST /v1.0/sites/root/lists`)
* _Sites.FullControl.All_: Acesso completo a sites e listas do SharePoint.

---

## <a name="subject-rights-request-permissions"></a>Permissões de solicitação de direitos de entidade

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
SubjectRightsRequest.Read.All | Ler solicitações de direitos da entidade | Permite que o aplicativo leia solicitações de direitos de entidade em nome do usuário conectado. | Sim | Não |
SubjectRightsRequest.ReadWrite.All | Ler e gravar solicitações de direitos da entidade | Permite que o aplicativo leia e grave solicitações de direitos de entidade em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos
Nenhuma.

### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegated
- SubjectRightsRequest.Read.All_: obter a lista de solicitações de direitos de entidade disponíveis para o usuário (`GET /privacy/subjectrightsrequests`).
- _SubjectRightsRequest.ReadWrite.All_: criar uma solicitação de direitos de entidade (`POST /privacy/subjectrightsrequests`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

## <a name="tasks-permissions"></a>Permissões de tarefas

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Tasks.Read_ | Ler tarefas e listas de tarefas do usuário (visualização) | Permite ao aplicativo ler as tarefas e listas de tarefas do usuário conectado, incluindo qualquer compartilhamento com o usuário. Não inclui a permissão para criar, excluir ou atualizar qualquer coisa. | Não | Sim |
| _Tasks.Read.Shared_ | Ler as tarefas do usuário e as tarefas compartilhadas (visualização) | Permite que o aplicativo leia as tarefas que o usuário tem permissão de acessar, incluindo as próprias tarefas e as tarefas compartilhadas. | Não | Não |
| _Tasks.ReadWrite_ | Criar, ler, atualizar e excluir tarefas e listas de tarefas do usuário (visualização) | Permite ao aplicativo criar, ler, atualizar, e excluir as tarefas e listas de tarefas do usuário conectado, incluindo qualquer compartilhamento com o usuário. | Não | Sim |
| _Tasks.ReadWrite.Shared_ | Ler e registrar as tarefas do usuário e as tarefas compartilhadas (visualização) | Permite que o aplicativo crie, leia, atualize e exclua as tarefas permitidas para um usuário, incluindo suas próprias tarefas e as compartilhadas. | Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

Nenhum.

### <a name="remarks"></a>Comentários
As permissões de _Tarefas_ são usadas para controlar o acesso a tarefas pendentes e tarefas do Outlook (obsoleto). O acesso às tarefas do Microsoft Planner é controlado pelas permissões de [_Grupo_](#group-permissions).

As permissões _Compartilhadas_ atualmente só são compatíveis com contas corporativas ou de estudante. Mesmo com permissões _Compartilhadas_, as leituras e gravações podem falhar se o usuário que possui o conteúdo compartilhado não tiver concedido as permissões de usuário de acesso para modificar o conteúdo dentro da pasta.

### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegado

* _Tasks.Read_: Obter todas as tarefas na caixa de correio do usuário (`GET /me/outlook/tasks`).
* _Tasks.Read.Shared_: Acessar tarefas em uma pasta compartilhada com você por outro usuário em sua organização (`Get /users{id|userPrincipalName}/outlook/taskfolders/{id}/tasks`).
* _Tasks.ReadWrite_: Adicionar um evento à pasta de tarefas padrão do usuário (`POST /me/outlook/tasks`).
* _Tasks.Read_: Obter todas as tarefas não concluídas na caixa de correio do usuário (`GET /users/{id | userPrincipalName}/outlook/tasks?$filter=status ne 'completed'`).
* _Tasks.ReadWrite_: Atualizar uma tarefa na caixa de correio do usuário (`PATCH /users/{id | userPrincipalName}/outlook/tasks/id`).
* _Tasks.ReadWrite.Shared_: Concluir uma tarefa em nome de outro usuário (`POST /users/{id | userPrincipalName}/outlook/tasks/id/complete`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="taxonomy-permissions"></a>Permissões de taxonomia

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TermStore.Read.All_        | Ler dados do repositório de termos | Permitir que o aplicativo leia vários termos, definições e grupos no repositório de termos | Sim  | Não |
| _TermStore.ReadWrite.All_   | Ler e gravar todos os dados do repositório de termos | Permitir que o aplicativo edite ou exclua termos, definições e grupos no repositório de termos | Sim  | Não |

### <a name="remarks"></a>Comentários

As permissões de taxonomia só são válidas para contas do trabalho ou da escola.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _TermStore.Read.All_: Ler o termstore para o locatário (`GET /termStore`)
* _TermStore.ReadWrite.All_: Criar novos termos no termStore (`POST /termStore/sets/123/children`)

---

## <a name="teams-permissions"></a>Permissões de equipes

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | Ler os nomes e as descrições das equipes | Ler os nomes e as descrições das equipes, em nome do usuário conectado.  | Não | Não |
| _Team.Create_  | Criar equipes | Criar equipes, em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos 

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | Obter uma lista de todas as equipes | Obter uma lista de todas as equipes, sem um usuário conectado.   | Sim | Não |
| _Team.Create_  | Criar equipes | Criar equipes, sem um usuário conectado. | Sim | Não |
| _Teamwork.Migrate.All_|Gerenciar a migração do Microsoft Teams|Criar e gerenciar recursos de migração do Microsoft Teams|Sim|Sim|

## <a name="team-settings-permissions"></a>Permissões de configurações de equipe

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamSettings.Read.All_ | Ler as configurações das equipes | Ler as configurações dessa equipe, em nome do usuário conectado.  | Sim | Não |
| _TeamSettings.ReadWrite.All_ | Ler e alterar configurações das equipes | Ler e alterar as configurações de todas as equipes, em nome do usuário conectado.    | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamSettings.Read.All_ | Ler as configurações de todas as equipes | Ler as configurações dessa equipe, sem um usuário conectado. | Sim | Não |
| _TeamSettings.ReadWrite.All_ | Ler e alterar as configurações de todas as equipes. | Ler e alterar as configurações de todas as equipes, sem um usuário conectado.  | Sim | Não |

## <a name="teams-activity-permissions"></a>Permissões de atividades das equipes

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsActivity.Read_ ([versão prévia privada](#permissions-availability-status)) | Ler o feed de atividades do trabalho em equipe | Permite que o aplicativo leia o feed de atividade em equipe do usuário conectado. | Não | Não |
| _TeamsActivity.Send_ | Enviar uma atividade de trabalho em equipe como o usuário | Permite que o aplicativo crie novas notificações nos feeds de atividades de trabalho em equipe dos usuários em nome do usuário conectado. Essas notificações podem não ser detectáveis ​​ou mantidas, ou controladas por políticas de conformidade. | Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsActivity.Read.All_ ([versão prévia privada](#permissions-availability-status)) | Ler o feed de atividades do trabalho em equipe de todos os usuários. | Permite que o aplicativo leia o feed de atividade em equipe de todos os usuários sem um usuário conectado. | Sim | Não |
| _TeamsActivity.Send_ | Enviar uma atividade de trabalho em equipe para qualquer usuário | Permite que o aplicativo crie novas notificações nos feeds de atividades de trabalho em equipe dos usuários sem um usuário conectado. Essas notificações podem não ser detectáveis ​​ou mantidas, ou controladas por políticas de conformidade. | Sim | Não |

## <a name="teams-app-permissions-deprecated"></a>Permissões do aplicativo do Teams (preteridas)

>[!NOTE]
>Essas permissões foram preteridas. Use o TeamsAppInstallation equivalente.\*. Em vez disso, todas as permissões.

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsApp.Read.All_ (**Preterido**)| Ler todos os aplicativos do Teams instalados | Permite que o aplicativo leia os aplicativos do Teams instalados para o usuário conectado, e em todas as equipes que o usuário é membro. Não dá a capacidade de ler as configurações específicas do aplicativo. | Sim | Não |
| _TeamsApp.ReadWrite.All_ (**Preterido**)| Gerenciar todos os aplicativos do Teams | Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams em nome do usuário conectado, e também das equipes que o usuário é membro. Não dá a capacidade de ler ou gravar as configurações específicas do aplicativo. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsApp.Read.All_ (**Preterido**)| Lê os aplicativos do Teams instalados de todos os usuários | Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo. | Sim | Não |
| _TeamsApp.ReadWrite.All_ (**Preterido**)| Gerencia os aplicativos do Teams de todos os usuários  | Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler ou gravar as configurações específicas do aplicativo.   | Sim | Não |

## <a name="teams-app-installation-permissions"></a>Permissões de instalação do aplicativo do Teams

#### <a name="delegated-permissions"></a>Permissões delegadas
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsAppInstallation.ReadForUser_  | Ler os aplicativos do Teams instalados do usuário| Permite que o aplicativo leia os aplicativos do Teams instalados para o usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Não | Não |
| _TeamsAppInstallation.ReadWriteForUser_ | Gerenciar os aplicativos do Teams instalados do usuário| Permite que o aplicativo leia instale, atualize e desinstale os aplicativos do Teams instalados para o usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteSelfForUser_ | Permitir que o aplicativo se gerencie nas equipes| Permite que um aplicativo do Teams se leia, se instale, se atualize e se desinstale para as equipes as quais o usuário conectado possa acessar.| Não | Não |
| _TeamsAppInstallation.ReadForTeam_ | Ler os seus aplicativos do Teams instalados nas equipes| Permite que o aplicativo leia os aplicativos do Teams instalados nas equipes que o usuário conectado pode acessar. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteForTeam_ | Gerenciar os aplicativos do Teams instalados nas equipes| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams nas equipes que o usuário conectado pode acessar. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteSelfForTeam_ | Permitir que o aplicativo se gerencie nas equipes| Permite que um aplicativo do Teams se leia, se instale, se atualize e se desinstale para as equipes as quais o usuário conectado possa acessar.| Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _TeamsAppInstallation.ReadForUser.All_ | Ler os aplicativos do Teams instalados para todos os usuários| Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteForUser.All_ | Gerenciar aplicativos do Teams para todos os usuários| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteSelfForUser.All_  | Permitir que o aplicativo se gerencie para todos os usuários| Permite que o aplicativo do Teams se leia, se instale, se atualize e se desinstale para qualquer usuário, sem um usuário conectado.| Sim |
| _TeamsAppInstallation.ReadForTeam.All_ | Ler os aplicativos do Teams instalados para todas as equipes| Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer equipe, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteForTeam.All_ | Gerenciar aplicativos de Teams para todas as equipes| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams em qualquer equipe, sem um usuário conectado. Não permite ler configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteSelfForTeam.All_ | Permitir que o aplicativo do Teams se gerencie para todas as equipes| Permite que o aplicativo do Teams se leia, se instale, se atualize e se desinstale em qualquer equipe, sem um usuário conectado.| Sim |

## <a name="teams-device-management-permissions"></a>Permissões de Gerenciamento de Dispositivo do Teams

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkDevice.Read.All_ | Ler dispositivos do Teams. | Permite que o aplicativo leia os dados de gerenciamento de dispositivos do Teams em nome do usuário conectado.   | Sim | Não |
| _TeamworkDevice.ReadWrite.All_ | Ler e gravar dispositivos do Teams. | Permite que o aplicativo leia e grave os dados de gerenciamento de dispositivos do Teams em nome do usuário conectado.  | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkDevice.Read.All_ | Ler dispositivos do Teams. | Permite que o aplicativo leia os dados de gerenciamento de dispositivos do Teams, sem um usuário conectado. | Sim | Não |
| _TeamworkDevice.ReadWrite.All_ | Ler e gravar dispositivos do Teams. | Permite que o aplicativo leia e grave os dados de gerenciamento de dispositivos do Teams, sem um usuário conectado. | Sim | Não |

## <a name="team-member-permissions"></a>Permissões de membro da equipe 

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamMember.Read.All_ | Leia os membros das equipes. | Leia os membros das equipes em nome do usuário conectado. | Sim | Não |
| _TeamMember.ReadWrite.All_ | Adicione e remova membros das equipes. | Adicione e remova membros das equipes em nome do usuário conectado. Também permite alterar a função de um membro. Por exemplo: de proprietário para não proprietário. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamMember.Read.All_ | Leia os membros das equipes. | Leia os membros das equipes sem um usuário conectado. | Sim | Não |
| _TeamMember.ReadWrite.All_ | Adicione e remova membros das equipes. | Adicione e remova membros das equipes sem um usuário conectado. Também permite alterar a função de um membro da equipe. Por exemplo: de proprietário para não proprietário. | Sim | Não |

## <a name="team-resource-specific-consent-permissions"></a>Permissões de consentimento específicas de recursos da equipe

#### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão | Exibir Cadeia de Caracteres | Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamSettings.Read.Group_ | Leia as configurações dessa equipe. | Ler as configurações dessa equipe, sem um usuário conectado. |Não | Não |
| _TeamSettings.ReadWrite.Group_ | Atualizar as configurações para esta equipe. | Leia e grave as configurações desta equipe, sem um usuário está conectado. |Não | Não |
| _ChannelSettings.Read.Group_ | Ler os nomes, descrições e configurações dos canais dessa equipe. | Leia os nomes dos canais, as descrições e as configurações dos canais desta equipe, sem um usuário conectado. |Não | Não |
| _ChannelSettings.ReadWrite.Group_ | Atualize os nomes, descrições e configurações dos canais desta equipe.| Atualize os nomes dos canais, as descrições e as configurações dos canais desta equipe, sem um usuário conectado. |Não | Não |
| _Channel.Create.Group_ | Criar canais nesta equipe. | Crie canais nesta equipe, sem um usuário conectado. |Não | Não |
| _Channel.Delete.Group_ | Excluir os canais dessa equipe. | Exclua os canais desta equipe, sem um usuário conectado. |Não | Não |
| _ChannelMessage.Read.Group_ | Ler as mensagens de canal da equipe. | Permite que um aplicativo leia as mensagens do canal desta equipe, sem um usuário conectado. |Não | Não |
| _TeamsAppInstallation.Read.Group_ | Veja quais aplicativos estão instalados nessa equipe. | Veja quais aplicativos estão instalados nesta equipe, sem um usuário conectado. |Não | Não |
| _TeamsTab.Read.Group_ | Leia as guias dessa equipe. | Leia as guias desta equipe, sem um usuário conectado. |Não | Não |
| _TeamsTab.Create.Group_ | Criar guias nesta equipe. | Crie guias nesta equipe, sem um usuário conectado. |Não | Não |
| _TeamsTab.ReadWrite.Group_ | Atualize as guias desta equipe. | Atualize as guias desta equipe, sem um usuário conectado. |Não | Não |
| _TeamsTab.Delete.Group_ | Excluir as guias dessa equipe. | Exclua as guias desta equipe, sem um usuário conectado. |Não | Não |
| _TeamMember.Read.Group_ | Leia os membros desta equipe. | Leia os membros desta equipe, sem um usuário está conectado. |Não | Não |
| _Member.Read.Group_ | Leia os membros deste grupo.| Excluir os membros desse grupo, sem um usuário conectado. |Não | Não |
| _Owner.Read.Group_| Leia os proprietários deste grupo. | Ler os proprietários desse grupo, sem um usuário conectado. |Não | Não |
| _File.Read.Group_| Leia os arquivos e pastas desta equipe. | **Suporte limitado** <br/> (Visualização) Leia os arquivos e pastas desta equipe, sem usuários conectados. | Não | Não |
| _TeamsActivity.Send.Group_| Envie notificações de feed de atividades aos usuários desta equipe. | Permite que o aplicativo crie novas notificações nos feeds de atividades de trabalho em equipe dos usuários desta equipe, sem um usuário conectado. | Não | Não |

## <a name="teams-settings-permissions"></a>Permissões de configurações do Teams

### <a name="delegated-permissions"></a>Permissões delegadas

| Permissão | Exibir Cadeia de Caracteres | Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | Ler os nomes e as descrições das equipes| Ler os nomes e descrições das equipes, em nome do usuário conectado.|Não| Não |
| _TeamSettings.Read.All_ | Ler as configurações das equipes| Ler as configurações de todas as equipes, em nome do usuário conectado.|Sim| Não |
| _TeamSettings.ReadWrite.All_ | Ler e alterar configurações das equipes.| Ler e alterar as configurações de todas as equipes, em nome do usuário conectado.|Sim| Não |

### <a name="application-permissions"></a>Permissões de aplicativos

| Permissão | Exibir Cadeia de Caracteres | Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | Obter uma lista de todas as equipes.| Obter uma lista de todas as equipes, sem um usuário conectado.|Sim| Não |
| _TeamSettings.Read.All_ | Ler as configurações de todas as equipes| Ler as configurações dessa equipe, sem um usuário conectado.|Sim| Não |
| _TeamSettings.ReadWrite.All_ | Ler e alterar todas as configurações das equipes| Ler e alterar as configurações de todas as equipes, sem um usuário conectado.|Não | Não |

## <a name="teams-tab-permissions"></a>Permissões de guia no Teams

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsTab.Read.All_ | Lê guias no Microsoft Teams. | Permite que o aplicativo leia os aplicativos do Teams instalados para o usuário conectado, e em todas as equipes que o usuário é membro. Não dá a capacidade de ler as configurações específicas do aplicativo. | Sim | Não |
| _TeamsTab.ReadWrite.All_ | Lê e grava guias no Microsoft Teams. | Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams em nome do usuário conectado, e também das equipes que o usuário é membro. Não dá a capacidade de ler ou gravar as configurações específicas do aplicativo.    | Sim | Não |
| _TeamsTab.Create_ | Cria guias no Microsoft Teams. | Permite que o aplicativo crie guias em qualquer equipe do Microsoft Teams, em nome do usuário conectado. Isso não concede a capacidade de ler, modificar ou excluir guias depois de criá-las ou conceder acesso ao conteúdo nas guias. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsTab.Read.All_ | Lê guias no Microsoft Teams. | Lê os nomes e as configurações de guias dentro de qualquer equipe do Microsoft Teams, sem um usuário conectado. Isso não dá acesso ao conteúdo nas guias. | Sim | Não |
| _TeamsTab.ReadWrite.All_ | Lê e grava guias no Microsoft Teams. | Lê e escreve as guias em qualquer equipe do Microsoft Teams, sem um usuário conectado. Isso não dá acesso ao conteúdo nas guias. | Sim | Não |
| _TeamsTab.Create_ | Cria guias no Microsoft Teams. | Permite que o aplicativo crie guias em qualquer equipe do Microsoft Teams, sem um usuário conectado. Isso não concede a capacidade de ler, modificar ou excluir guias depois de criá-las ou conceder acesso ao conteúdo nas guias. | Sim | Não |

## <a name="teams-tag-permissions"></a>Permissões de rótulos do Teams

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkTag.ReadWrite_| Lê e grava rótulos no Microsoft Teams. | Permite que o aplicativo leia e escreva programas em nome do usuário conectado.   | Sim | Não |
| _TeamworkTag.Read_ | Lê rótulos no Microsoft Teams. | Permite que o aplicativo leia programas em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkTag.ReadWrite_| Lê e grava rótulos no Microsoft Teams. | Permite que o aplicativo leia e grave marcas no Teams sem um usuário conectado.   | Sim | Não |
| _TeamworkTag.Read_ | Lê rótulos no Microsoft Teams. | Permite que o aplicativo leia marcas no Teams sem um usuário conectado. | Sim | Não |


## <a name="terms-of-use-permissions"></a>Permissões de termos de uso

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Agreement.Read.All_ | Ler todos os acordos de termos de uso | Permite que o aplicativo leia acordos de termos de uso em nome do usuário conectado. | Sim | Não |
| _Agreement.ReadWrite.All_ | Ler e gravar todos os acordos de termos de uso | Permite que o aplicativo leia e grave acordos de termos de uso em nome do usuário conectado. | Sim | Não |
| _AgreementAcceptance.Read_ | Ler os status de aceitação de termos de uso do usuário | Permite que o aplicativo leia status de aceitação de termos de uso em nome do usuário conectado. | Sim | Não |
| _AgreementAcceptance.Read.All_ | Ler os status de aceitação de termos de uso que o usuário pode acessar | Permite que o aplicativo leia status de aceitação de termos de uso em nome do usuário conectado. | Sim | Não |

### <a name="remarks"></a>Comentários

Todas as permissões acima são válidas apenas para contas corporativas ou de estudante.

Para que um aplicativo leia ou grave todos os contratos ou aceitações de contrato com permissões delegadas, o usuário conectado deve receber a função de Administrador Global, Administrador de Acesso Condicional ou Administrador de Segurança. Para obter mais informações sobre funções de administrador, confira [Atribuição de funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado
Os seguintes usos são válidos para permissões delegadas:

* _Agreement.Read.All_: ler todos os acordos de termos de uso (`GET /beta/agreements`)
* _Agreement.ReadWrite.All_: ler e gravar todos os acordos de termos de uso (`POST /beta/agreements`)
* _AgreementAcceptance.Read_: ler os status de aceitação de termos de uso do usuário (`GET /beta/me/agreementAcceptances`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="threat-assessment-permissions"></a>Permissões de avaliação de ameaças

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ThreatAssessment.ReadWrite.All_ | Solicitações de avaliação de ameaças de leitura e gravação | Permite que o aplicativo leia os eventos de segurança da sua organização em nome do usuário conectado. Também permite que o aplicativo crie novas solicitações para avaliar as ameaças recebidas por sua organização em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _ThreatAssessment.Read.All_ | Solicitações de avaliação de ameaças de leitura | Permite que o aplicativo leia os eventos de segurança da sua organização em nome do usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

Essas permissões só são válidas para contas corporativas ou de estudante.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _ThreatAssessment. ReadWrite.All_: ler e gravar solicitações de avaliação de ameaças (`POST /informationProtection/threatAssessmentRequests`)

#### <a name="application"></a>Aplicativo

* _ThreatAssessment. ReadWrite.All_: ler e gravar solicitações de avaliação de ameaças (`GET /informationProtection/threatAssessmentRequests`)

---

## <a name="universal-print-permissions"></a>Permissões Universais de Impressão

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Printer.Create_ | Impressoras registradas | Permite que o aplicativo crie (cadastre) impressoras em nome do usuário conectado. | Sim | Não |
| _Printer.FullControl.All_ | Registre, leia, atualize e cancele o registro de impressoras | Permite que o aplicativo crie (registre), leia, atualize e exclua (cancele o registro) de impressoras em nome do usuário conectado. | Sim | Não |
| _Printer.Read.All_ | Ler impressoras | Permite que o aplicativo leia impressoras em nome do usuário conectado. | Sim | Não |
| _Printer.ReadWrite.All_ | Ler e atualizar as impressoras | Permite que o aplicativo leia e atualize impressoras em nome do usuário conectado. Não permite a criação (registro) ou a exclusão (cancelamento do registro) de impressoras. | Sim | Não |
| _PrinterShare.ReadBasic.All_ | Leia as informações básicas sobre compartilhamentos de impressoras | Permite que o aplicativo leia informações básicas sobre os compartilhamentos da impressora em nome do usuário conectado. Não permite a leitura de informações de controle de acesso. | Não | Não |
| _PrinterShare.Read.All_ | Ler compartilhamentos de impressora | Permite que o aplicativo leia os compartilhamentos da impressora em nome do usuário conectado. | Não | Não |
| _PrinterShare.ReadWrite.All_ | Ler e gravar compartilhamentos de impressora | Permite que o aplicativo leia e atualize compartilhamentos de impressora em nome do usuário conectado. | Sim | Não |
| _PrintJob.Create_ | Crie trabalhos de impressão | Permite que o aplicativo crie trabalhos de impressão em nome do usuário conectado e carregue o conteúdo do documento para imprimir os trabalhos que o usuário conectado criou. | Não | Não |
| _PrintJob.Read_ | Ler os trabalhos de impressão do usuário | Permite que o aplicativo leia os metadados e o conteúdo do documento dos trabalhos de impressão criados pelo usuário conectado. | Não | Não |
| _PrintJob.Read.All_ | Ler os trabalhos de impressão | Permite que o aplicativo leia os metadados e o conteúdo do documento dos trabalhos de impressão em nome do usuário conectado. | Sim | Não |
| _PrintJob.ReadBasic_ | Ler informações básicas dos trabalhos de impressão do usuário | Permite que o aplicativo leia os metadados dos trabalhos de impressão criados pelo usuário conectado. Não permite acesso ao conteúdo do documento do trabalho de impressão. | Não | Não |
| _PrintJob.ReadBasic.All_ | Ler informações básicas dos trabalhos de impressão | Permite que o aplicativo leia os metadados dos trabalhos de impressão em nome do usuário conectado. Não permite acesso ao conteúdo do documento do trabalho de impressão. | Sim | Não |
| _PrintJob.ReadWrite_ | Ler e gravar os trabalhos de impressão do usuário | Permite que o aplicativo leia e atualize os metadados e o conteúdo do documento dos trabalhos de impressão criados pelos usuário conectado. | Não | Não |
| _PrintJob.ReadWrite.All_ | Ler e gravar trabalhos de impressão | Permite que o aplicativo leia e atualize os metadados e o conteúdo do documento dos trabalhos de impressão em nome do usuário conectado. | Sim | Não |
| _PrintJob.ReadWriteBasic_ | Ler e gravar informações básicas de trabalhos de impressão do usuário | Permite que o aplicativo leia e atualize os metadados dos trabalhos de impressão que o usuário conectado criou. Não permite acesso ao conteúdo do documento do trabalho de impressão. | Não | Não |
| _PrintJob.ReadWriteBasic.All_ | Ler e gravar informações básicas de trabalhos de impressão | Permite que o aplicativo leia e atualize os metadados dos trabalhos de impressão em nome do usuário conectado. Não permite acesso ao conteúdo do documento do trabalho de impressão. | Sim | Não |
| _PrintConnector.Read.All_ | Conectores de leitura | Permite que o aplicativo leia os conectores em nome do usuário conectado. | Sim | Não |
| _PrintConnector.ReadWrite.All_ | Leia e grave os conectores de impressão | Permite que o aplicativo leia e escreva conectores de impressão em nome do usuário conectado. | Sim | Não |
| _PrintSettings.Read.All_ | Leia as configurações de impressão em todo o locatário | Permite que o aplicativo leia os compartilhamentos da impressora em nome do usuário conectado. | Sim | Não |
| _PrintSettings.ReadWrite.All_ | Leia e grave as configurações de impressão em todo o locatário | Permite que o aplicativo leia e atualize impressoras em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _Printer.Read.All_ | Ler impressoras | Permite que o aplicativo leia as impressoras sem um usuário conectado. | Sim |
| _Printer.ReadWrite.All_ | Ler e atualizar as impressoras | Permite que o aplicativo leia e atualize as impressoras sem um usuário conectado. Não permite a criação (registro) ou a exclusão (cancelamento do registro) de impressoras. | Sim |
| _PrintJob.Manage.All_ | Executar operações avançadas nos trabalhos de impressão | Permite que o aplicativo execute operações avançadas, como redirecionar um trabalho de impressão para outra impressora sem um usuário conectado. Também, permite que o aplicativo leia e atualize os metadados dos trabalhos de impressão. | Sim |
| _PrintJob.Read.All_ | Ler os trabalhos de impressão | Permite que o aplicativo leia os metadados e o conteúdo do documento dos trabalhos de impressão sem um usuário conectado. | Sim |
| _PrintJob.ReadBasic.All_ | Ler informações básicas de trabalhos para impressão | Permite que o aplicativo leia os metadados dos trabalhos de impressão sem um usuário conectado. Não permite acesso ao conteúdo do documento do trabalho de impressão. | Sim |
| _PrintJob.ReadWrite.All_ | Ler e gravar trabalhos de impressão | Permite que o aplicativo leia e atualize os metadados e o conteúdo do documento dos trabalhos de impressão sem um usuário conectado. | Sim |
| _PrintJob.ReadWriteBasic.All_ | Ler e gravar informações básicas para trabalhos de impressão | Permite que o aplicativo leia e atualize os metadados dos trabalhos de impressão sem um usuário conectado. Não permite acesso ao conteúdo do documento do trabalho de impressão. | Sim |
| _PrintTaskDefinition.ReadWrite.All_ | Ler, gravar e atualizar definições das tarefas de impressão | Permite que o aplicativo leia e atualize as definições das tarefas de impressão sem um usuário conectado. | Sim |

### <a name="remarks"></a>Comentários

* Para utilizar o serviço Universal Print, o usuário ou locatário do aplicativo deve ter uma assinatura ativa do Universal Print, além das permissões anteriormente listadas.

* Algumas permissões distinguem entre metadados de trabalho de impressão e conteúdo. Os metadados descrevem a configuração de um trabalho de impressão (seu nome e configuração do documento, por exemplo, se ele deve ser grampeado ou impresso em cores). Conteúdo são os próprios dados do documento (o arquivo PDF ou XPS a serem impresso).

* Todas as permissões PrintJob.* Também exigem pelo menos Printer.Read.All (ou uma permissão mais reservada) porque os trabalhos de impressão são armazenados nas impressoras.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Printer.Read.All_: Obtenha uma lista de todas as impressoras do locatário (`GET /print/printers`)
* _PrintJob.Read.All_: Obtenha uma lista de todos os trabalhos de impressão enfileirados em uma impressora (`GET /print/printers/{id}/jobs`)
* _Printer.FullControl.All_: Eliminar uma impressora (sem registro) (`DELETE /print/printers/{id}`)
* _PrintJob.ReadWriteBasic.All_: Atualizar metadados (como o status atual) de trabalhos de impressão (`PATCH /print/printers/{id}/jobs/{id}`)
* _PrintJob.ReadWrite.All_: Crie trabalhos de impressão e carregue os dados de documentos para eles (`POST /print/printers/{id}/jobs`)

#### <a name="application"></a>Aplicativo

* _Printer.Read.All_: Obtenha uma lista de todas as impressoras do locatário (`GET /print/printers`)

---

## <a name="user-permissions"></a>Permissões do usuário

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _User.Read_       |    Entrar e ler o perfil do usuário | Permite aos usuários entrar no aplicativo e permite ao aplicativo ler o perfil de usuários conectados. Também permite que o aplicativo leia as informações básicas da empresa sobre os usuários conectados.| Não | Sim |
| _User.ReadWrite_ |    Acesso de leitura e gravação ao perfil de usuário | Permite que o aplicativo leia o perfil completo do usuário conectado. Também possibilita que o aplicativo atualize as informações de perfil do usuário conectado em seu nome. | Não | Sim |
| _User.ReadBasic.All_ |    Ler os perfis básicos de todos usuários | Permite ao aplicativo ler um conjunto básico de propriedades de perfil de outros usuários em sua organização em nome do usuário conectado. Inclui o nome para exibição, nome e sobrenome, endereço de email, extensões abertas e foto. Também permite que o aplicativo leia o perfil completo do usuário conectado. | Não | Não |
| _User.Read.All_  |     Ler os perfis completos de todos os usuários           | Permite ao aplicativo ler o conjunto completo de propriedades do perfil, relatórios e gerentes de outros usuários em sua organização, em nome do usuário conectado. | Sim | Não |
| _User.ReadWrite.All_ |     Ler e gravar os perfis completos de todos os usuários | Permite ao aplicativo ler e gravar o conjunto completo de propriedades do perfil, relatórios e gerentes de outros usuários na sua organização, em nome do usuário conectado. Também permite que o aplicativo crie e exclua usuários, além de redefinir senhas de usuário em nome do usuário conectado. | Sim | Não |
| _User.Invite.All_  |     Convidar usuários convidados para a organização | Permite que o aplicativo convide usuários para sua organização em nome do usuário conectado. | Sim | Não |
| _User.Export.All_       |    Exportar dados de usuários | Permite que o aplicativo exporte os dados de um usuário organizacional, quando executado por um administrador da empresa.| Sim | Não |
| _User.ManageIdentities.All_       |    Gerenciar identidades de usuário | Permite que um aplicativo leia, atualize e exclua identidades associadas a uma conta de usuário, a qual o usuário conectado tenha acesso. Isso controla com quais identidades seus usuários podem se conectar. | Sim | Não |


#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _User.Read.All_ |    Ler os perfis completos de todos os usuários | Permite ao aplicativo ler o conjunto completo de propriedades do perfil, relatórios e gerenciadores de outros usuários na sua organização, sem um usuário conectado.| Sim |
| _User.ReadWrite.All_ |   Ler e gravar os perfis completos de todos os usuários | Permite ao aplicativo ler e gravar o conjunto completo de propriedades do perfil, relatórios e gerentes de outros usuários na sua organização, sem um usuário conectado.  Também permite que o aplicativo crie e exclua usuários não administrativos. Não permite a redefinição de senhas de usuário. | Sim |
| _User.Invite.All_  |     Convidar usuários convidados para a organização | Permite que o aplicativo convide usuários para sua organização sem um usuário conectado. | Sim |
| _User.Export.All_       |    Exportar dados de usuários | Permite que o aplicativo exporte dados de usuários organizacionais, sem um usuário conectado.| Sim |
| _User.ManageIdentities.All_       |    Gerenciar todas as identidades de usuário | Permite que um aplicativo leia, atualize e exclua identidades associadas a uma conta de usuário, sem um usuário conectado. Isso controla com quais identidades os usuários podem se conectar. |  Sim |

### <a name="remarks"></a>Comentários

Com a permissão _User.Read_, um aplicativo também pode ler as informações básicas da empresa do usuário conectado de uma conta corporativa ou de estudante através do recurso [Organização](/graph/api/resources/organization). As propriedades a seguir estão disponíveis: id, displayName e verifiedDomains.

Para contas corporativas ou de estudante, o perfil completo inclui todas as propriedades declaradas do recurso [Usuário](/graph/api/resources/user). No caso das leituras, somente um número limitado de propriedades é retornado por padrão. Para ler propriedades que não estão no conjunto padrão, use `$select`. As propriedades padrão são:

- displayName
- givenName
- jobTitle
- Email
- mobilePhone
- officeLocation
- preferredLanguage
- surname
- userPrincipalName

 As Permissões Delegadas _User.ReadWrite_ e _User.Readwrite.All_ permitem ao aplicativo atualizar as seguintes propriedades de perfil de contas corporativas ou de estudante:

- aboutMe
- birthday
- hireDate
- interests
- mobilePhone
- mySite
- pastProjects
- photo
- preferredName
- responsibilities
- schools
- skills

Com a Permissão de aplicativo _User.ReadWrite.All_, o aplicativo pode atualizar todas as propriedades declaradas das contas corporativas ou de estudante, com exceção da senha.

Com o _Usuário.ReadWrite.All_ autorização delegada ou de aplicação, atualizar os **BusinessPhones**, **mobilePhone** ou **otherMails** de outro usuário só é permitido em usuários que não sejam administradores ou aos quais tenha sido atribuída uma das seguintes funções: Leitores de Diretório, Convidado, Leitor de Centro de Mensagens e Leitor de Relatórios. Para mais detalhes, consulte o Helpdesk (Senha) Administrador no [Azure AD funções disponíveis](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

Para ler ou gravar os subordinados diretos (`directReports`) ou o gerente (`manager`) de uma conta corporativa ou de estudante, o aplicativo deve ter as permissões _User.Read.All_ (somente leitura) ou _User.ReadWrite.All_.

A permissão _User.ReadBasic.All_ restringe o acesso do aplicativo a um conjunto limitado de propriedades conhecido como o perfil básico. Isso ocorre porque o perfil completo pode conter informações de diretório confidenciais. O perfil básico inclui apenas as seguintes propriedades:

- displayName
- givenName
- Email
- photo
- surname
- userPrincipalName

Para ler as associações de grupos de um usuário (`memberOf`), o aplicativo deve ter o [_Group.Read.All_](#group-permissions) ou o [_Group.ReadWrite.All_](#group-permissions). No entanto, se o usuário também tiver uma associação a um [directoryRole](/graph/api/resources/directoryrole) ou [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true), o aplicativo também precisará de permissões efetivas para ler esses recursos ou o Microsoft Graph retornará um erro. Isso significa que o aplicativo deve ter também [Permissões do diretório](#directory-permissions); para as Permissões Delegadas, o usuário conectado deve ter privilégios suficientes na organização para acessar unidades administrativas e funções de diretório.

Com o _User.ManageIdentities.All_ delegado ou as permissões de aplicativo, é possível atualizar as identidades (`identities`) de um usuário. Isso inclui as identidades federadas (ou identidades sociais) ou as identidades locais com nomes de entrada com base em nome ou email.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _User.Read_: Ler o perfil completo para o usuário conectado (`GET /me`).
* _User.ReadWrite_: Atualizar a foto do usuário conectado (`PUT /me/photo/$value`).
* _User.ReadBasic.All_: Localizar todos os usuários cujos nomes começam com "Davi" (`GET /users?$filter=startswith(displayName,'David')`).
* _User.Read.All_: Ler o gerente de um usuário (`GET /users/{id | userPrincipalName}/manager`).

#### <a name="application"></a>Aplicativo

* _User.Read.All_: Ler todos os usuários e relações usando a consulta delta (`GET /beta/users/delta?$select=displayName,givenName,surname`).
* _User.ReadWrite.All_: Atualizar a foto de qualquer usuário na organização (`PUT /users/{id | userPrincipalName}/photo/$value`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

## <a name="user-activity-permissions"></a>Permissões de Atividades do Usuário

#### <a name="delegated-permissions"></a>Permissões delegadas

|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|:-----------------|
| _UserActivity.ReadWrite.CreatedByApp_ |Ler e gravar a atividades de aplicativos no feed de atividades de usuários |Permite que o aplicativo leia e relate as atividades do usuário conectado no aplicativo. |Não | Sim |

#### <a name="application-permissions"></a>Permissões de aplicativos
Nenhum.

### <a name="remarks"></a>Comentários
*UserActivity.ReadWrite.CreatedByApp* é válida tanto para contas da Microsoft como para contas corporativas e de estudante.

A restrição *CreatedByApp* associada a essa permissão indica que o serviço aplicará filtragem implícita aos resultados com base na identidade aplicativo que realizar a chamada, seja a ID de aplicativo MSA ou um conjunto de IDs de aplicativos configurados para uma identidade de aplicativo de plataformas cruzadas.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado
* _UserActivity.ReadWrite.CreatedByApp_: obtenha uma lista de atividades de usuário exclusivas recentes com base em itens de histórico associados publicados no último dia. (GET /me/activities/recent).
* _UserActivity.ReadWrite.CreatedByApp_: publicar ou atualizar uma atividade do usuário que pode ser retomada pelo usuário do aplicativo. (PUT /me/activities/%2Farticle%3F12345).
*   _UserActivity.ReadWrite.CreatedByApp_: publicar ou atualizar um item de histórico para uma atividade de usuário especificada, a fim de representar o período de engajamento do usuário. (PUT /me/activities/{id}/historyItems/{id}).
*   _UserActivity.ReadWrite.CreatedByApp_: exclua uma atividade do usuário em resposta a uma solicitação iniciada pelo usuário ou para remover dados inválidos. (DELETE /me/activities/{id}).
*   _UserActivity.ReadWrite.CreatedByApp_: exclua um item do histórico em resposta à solicitação iniciada pelo usuário ou para remover dados inválidos. (DELETE /me/activities/{id}/historyItems/{id}).

---

## <a name="user-authentication-method-permissions-preview"></a>Permissões do método de autenticação do usuário ([visualização](#permissions-availability-status))

#### <a name="delegated-permissions"></a>Permissões delegadas

|Permissão                              |Exibir Cadeia de Caracteres                        |Descrição        |Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:---------------------------------------|:-------------------------------------|:------------------|:----------------------|:----------------------------|
|_UserAuthenticationMethod.Read_ (visualização)        |Ler os próprios métodos de autenticação       |Permitir que o aplicativo leia os métodos de autenticação do usuário conectado, incluindo números de telefone e configurações do aplicativo Authenticator. Isso não permite que o aplicativo veja informações secretas, como senhas do usuário conectado, entrar ou usar métodos de autenticação do usuário conectado. |Sim|Não|
|_UserAuthenticationMethod.Read.All_ (visualização)    |Ler os métodos de autenticação dos usuários    |Permite que o aplicativo leia os métodos de autenticação de todos os usuários em sua organização aos quais o usuário têm acesso. Os métodos de autenticação incluem coisas como o número de telefone do usuário e as configurações do aplicativo Authenticator. Isso não permite que o aplicativo veja informações secretas, como senhas, entrar ou usar métodos de autenticação. |Sim|Não|
|_UserAuthenticationMethod.ReadWrite_ (visualização)   |Gerenciar os próprios métodos de autenticação     |Permite que o aplicativo leia e grave os métodos de autenticação do usuário conectado, incluindo números de telefone e as configurações do aplicativo Authenticator. Isso não permite que o aplicativo veja informações secretas, como senhas do usuário conectado, entrar ou usar métodos de autenticação do usuário conectado. |Sim|Não|
|_UserAuthenticationMethod.ReadWrite.All_ (visualização)|Gerenciar os métodos de autenticação dos usuários  |Permite que o aplicativo leia e grave os métodos de autenticação de todos os usuários em sua organização aos quais o usuário conectado têm acesso. Os métodos de autenticação incluem coisas como o número de telefone do usuário e as configurações do aplicativo Authenticator. Isso não permite que o aplicativo veja informações secretas, como senhas, entrar ou usar métodos de autenticação. |Sim|Não|

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão                              |Exibir Cadeia de Caracteres                        |Descrição        |Consentimento Obrigatório do Administrador |
|:---------------------------------------|:-------------------------------------|:------------------|:----------------------|
|_UserAuthenticationMethod.Read.All_ (visualização)   |Ler os métodos de autenticação dos usuários    |Permite que o aplicativo leia os métodos de autenticação de todos os usuários em sua organização sem um usuário conectado. Os métodos de autenticação incluem coisas como o número de telefone do usuário e as configurações do aplicativo Authenticator. Isso não permite que o aplicativo veja informações secretas, como senhas, entrar ou usar métodos de autenticação. |Sim|
|_UserAuthenticationMethod.ReadWrite.All_ (visualização)|Gerenciar os métodos de autenticação dos usuários  |Permite que o aplicativo leia e grave os métodos de autenticação de todos os usuários em sua organização sem um usuário conectado. Os métodos de autenticação incluem coisas como o número de telefone do usuário e as configurações do aplicativo Authenticator. Isso não permite que o aplicativo veja informações secretas, como senhas, entrar ou usar métodos de autenticação. |Sim|

### <a name="remarks"></a>Comentários

As permissões do método de autenticação do usuário são usadas para gerenciar os métodos de autenticação dos usuários. Com essas permissões, um usuário ou aplicativo delegado pode registrar novos métodos de autenticação em um usuário, ler os métodos de autenticação que o usuário já registrou, atualizar estes métodos de autenticação e removê-los do usuário.

Com essas permissões, todos os métodos de autenticação podem ser lidos e gerenciados em um usuário. Isso inclui os métodos usados para:

* Autenticação primária (senha)
* Segundo fator de autenticação multifator/MFA (números de telefone)
* Redefinição de senha de autoatendimento/SSPR (endereço de email)

## <a name="windows-updates-permissions"></a>Permissões de atualizações do Windows

#### <a name="delegated-permissions"></a>Permissões delegadas

|Permissão|Exibir Cadeia de Caracteres|Descrição|Consentimento Obrigatório do Administrador|Conta Microsoft com Suporte|
|:---|:---|:---|:---|:---|
|_WindowsUpdates.ReadWrite.All_|Ler e gravar todas as configurações de implantação de atualização do Windows|Permite ao aplicativo ler e gravar todas as configurações de implantação de atualização do Windows para a organização em nome do usuário que está assinado.|Sim|Não|

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão|Exibir Cadeia de Caracteres|Descrição|Consentimento Obrigatório do Administrador|
|:---|:---|:---|:---|
|_WindowsUpdates.ReadWrite.All_|Ler e gravar todas as configurações de implantação de atualização do Windows|Permite que o aplicativo leia e grave todas as configurações de implantação de atualização do Windows para a organização sem um usuário conectado.|Sim|

### <a name="remarks"></a>Comentários

Todas as permissões acima são válidas apenas para contas corporativas ou de estudante.

Para que um aplicativo leia ou grave todas as configurações de implantação com permissões delegadas, o usuário conectado deve receber a função de Administrador Global, Administrador do Intune ou Administrador de Implantação do Windows Update Para obter mais informações sobre funções de administrador, consulte [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _WindowsUpdates.ReadWrite.All_: crie uma implantação (`POST /beta/admin/windows/updates/deployments`).

#### <a name="application"></a>Aplicativo

* _WindowsUpdates.ReadWrite.All_: crie uma implantação (`POST /beta/admin/windows/updates/deployments`).

## <a name="permission-scenarios"></a>Cenários de permissão

Esta seção mostra alguns cenários comuns direcionados aos recursos [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group) em uma organização. As tabelas mostram as permissões que um aplicativo precisa para conseguir executar operações específicas necessárias para o cenário. Observe que, em alguns casos, a capacidade do aplicativo de executar operações específicas dependerá se uma permissão é uma Permissão de aplicativo ou Permissão Delegada. No caso de Permissões Delegadas, as Permissões Efetivas do aplicativo também dependerão dos privilégios do usuário conectado na organização. Para obter mais informações, confira [Permissões delegadas, Permissões de aplicativo e permissões efetivas](auth/auth-concepts.md#microsoft-graph-permissions).

### <a name="access-scenarios-on-the-user-resource"></a>Cenários de acesso do recurso Usuário

| **Tarefas do aplicativo envolvendo o Usuário**   |  **Permissões necessárias** | **Cadeias de caracteres de permissão** |
|:-------------------------------|:---------------------|:---------------|
| O aplicativo deseja ler as informações básicas de outros usuários (somente o nome para exibição e a imagem), por exemplo, para mostrar uma experiência de seleção de pessoas   | _User.ReadBasic.All_  |  Ler todos os perfis básicos do usuário |
| O aplicativo deseja ler o perfil completo do usuário de um usuário conectado (ver subordinados diretos, gerente etc.)     | _User.Read_ | Habilitar entrada e ler o perfil de usuário|
| O aplicativo deseja ler o perfil completo de todos os usuários  | _User.Read.All_ |  Ler os perfis completos de todos os usuários   |
| O aplicativo deseja ler informações de arquivos, email e calendário do usuário conectado  | _User.Read_, _Files.Read_, _Mail.Read_, _Calendars.Read_ | Habilitar entrada e ler o perfil de usuário, ler arquivos dos usuários, ler email do usuário, ler calendários do usuário |
| O aplicativo deseja ler os arquivos dos usuários (meus) conectados e os arquivos que outros usuários compartilharam com o usuário conectado (eu). | _User.Read_, _Files.Read_, _Sites.Read.All_ | Habilitar entrada e ler o perfil de usuário, ler arquivos dos usuários, ler itens em todos os conjuntos de sites |
| O aplicativo deseja ler e gravar o perfil completo do usuário conectado   | _User.ReadWrite_ | Acesso de leitura e gravação ao perfil de usuário |
| O aplicativo deseja ler e gravar o perfil completo de todos os usuários    | _User.ReadWrite.All_ | Ler e gravar os perfis completos de todos os usuários |
| O aplicativo deseja ler e gravar informações de arquivos, de email e de calendário do usuário conectado    | _User.ReadWrite_, _Files.ReadWrite_, _Mail.ReadWrite_, _Calendars.ReadWrite_  |  Acesso de leitura e gravação ao perfil de usuário, acesso de leitura e gravação ao perfil de usuário, acesso de leitura e gravação ao email do usuário, acesso total a calendários do usuário |
| O aplicativo deseja enviar uma solicitação de operação de política de dados para exportar dados pessoais de um usuário | _User.Export.All_ | Exportar os dados pessoais e de um usuário. |


### <a name="access-scenarios-on-the-group-resource"></a>Cenários de acesso do recurso Grupo

| **Tarefas do aplicativo envolvendo o Grupo**  |  **Permissões necessárias** |  **Cadeias de caracteres de permissão** |
|:-------------------------------|:---------------------|:---------------|
| O aplicativo deseja ler as informações básicas do grupo (somente o nome para exibição e a imagem), por exemplo, para mostrar uma experiência de seleção de um grupo  | _Group.Read.All_  | Ler todos os grupos|
| O aplicativo deseja ler todo o conteúdo em todos os grupos do Microsoft 365, incluindo arquivos, conversas.  Ele também precisa mostrar associações de grupo, conseguir atualizar associações de grupo (caso seja o proprietário).  |  _Group.Read.All_ | Ler itens em todos os conjuntos de sites, ler todos os grupos|
| O aplicativo deseja ler e gravar todo o conteúdo em todos os grupos do Microsoft 365, incluindo arquivos, conversas. Ele também precisa mostrar associações de grupo, conseguir atualizar associações de grupo (caso seja o proprietário).  |    _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  Ler e gravar todos os grupos, editar ou excluir itens em todos os conjuntos de sites |
| O aplicativo deseja descobrir (localizar) um grupo do Microsoft 365. Permite ao usuário procurar um grupo específico e escolher um deles na lista enumerada para permitir a sua entrada no grupo.   | _Group.ReadWrite.All_ | Ler e gravar todos os grupos|
| O aplicativo deseja criar um grupo por meio do AAD Graph |   _Group.ReadWrite.All_ | Ler e gravar todos os grupos|


## <a name="all-permissions-and-ids"></a>Todas as permissões e IDs

| Permissão                                              | Tipo        | ID                                   |
|---------------------------------------------------------|-------------|--------------------------------------|
| AccessReview.Read.All                                   | Delegado   | ebfcd32b-babb-40f4-a14b-42706e83bd28 |
| AccessReview.Read.All                                   | Aplicativo | d07a8cc0-3d51-4b77-b3b0-32704d1f69fa |
| AccessReview.ReadWrite.All                              | Delegado   | e4aa47b9-9a69-4109-82ed-36ec70d85ff1 |
| AccessReview.ReadWrite.All                              | Aplicativo | ef5f7d5c-338f-44b0-86c3-351f46c8bb5f |
| AccessReview.ReadWrite.Membership                       | Delegado   | 5af8c3f5-baca-439a-97b0-ea58a435e269 |
| AccessReview.ReadWrite.Membership                       | Aplicativo | 18228521-a591-40f1-b215-5fad4488c117 |
| AdministrativeUnit.Read.All                             | Delegado   | 3361d15d-be43-4de6-b441-3c746d05163d |
| AdministrativeUnit.Read.All                             | Aplicativo | 134fd756-38ce-4afd-ba33-e9623dbe66c2 |
| AdministrativeUnit.ReadWrite.All                        | Delegado   | 7b8a2d34-6b3f-4542-a343-54651608ad81 |
| AdministrativeUnit.ReadWrite.All                        | Aplicativo | 5eb59dd3-1da2-4329-8733-9dabdc435916 |
| Agreement.Read.All                                      | Delegado   | af2819c9-df71-4dd3-ade7-4d7c9dc653b7 |
| Agreement.Read.All                                      | Aplicativo | 2f3e6f8c-093b-4c57-a58b-ba5ce494a169 |
| Agreement.ReadWrite.All                                 | Delegado   | ef4b5d93-3104-4664-9053-a5c49ab44218 |
| Agreement.ReadWrite.All                                 | Aplicativo | c9090d00-6101-42f0-a729-c41074260d47 |
| AgreementAcceptance.Read                                | Delegado   | 0b7643bb-5336-476f-80b5-18fbfbc91806 |
| AgreementAcceptance.Read.All                            | Delegado   | a66a5341-e66e-4897-9d52-c2df58c2bfb9 |
| AgreementAcceptance.Read.All                            | Aplicativo | d8e4ec18-f6c0-4620-8122-c8b1f2bf400e |
| Analytics.Read                                          | Delegado   | e03cf23f-8056-446a-8994-7d93dfc8b50e |
| APIConnectors.Read.All                                  | Delegado   | 1b6ff35f-31df-4332-8571-d31ea5a4893f |
| APIConnectors.Read.All                                  | Aplicativo | b86848a7-d5b1-41eb-a9b4-54a4e6306e97 |
| APIConnectors.ReadWrite.All                             | Delegado   | c67b52c5-7c69-48b6-9d48-7b3af3ded914 |
| APIConnectors.ReadWrite.All                             | Aplicativo | 1dfe531a-24a6-4f1b-80f4-7a0dc5a0a171 |
| AppCatalog.Read.All                                     | Delegado   | 88e58d74-d3df-44f3-ad47-e89edf4472e4 |
| AppCatalog.Read.All                                     | Aplicativo | e12dae10-5a57-4817-b79d-dfbec5348930 |
| AppCatalog.ReadWrite.All                                | Delegado   | 1ca167d5-1655-44a1-8adf-1414072e1ef9 |
| AppCatalog.ReadWrite.All                                | Aplicativo | dc149144-f292-421e-b185-5953f2e98d7f |
| AppCatalog.Submit                                       | Delegado   | 3db89e36-7fa6-4012-b281-85f3d9d9fd2e |
| Application.Read.All                                    | Delegado   | c79f8feb-a9db-4090-85f9-90d820caa0eb |
| Application.Read.All                                    | Aplicativo | 9a5d68dd-52b0-4cc2-bd40-abcf44ac3a30 |
| Application.ReadWrite.All                               | Delegado   | bdfbf15f-ee85-4955-8675-146e8e5296b5 |
| Application.ReadWrite.All                               | Aplicativo | 1bfefb4e-e0b5-418b-a88f-73c46d2cc8e9 |
| Application.ReadWrite.OwnedBy                           | Aplicativo | 18a4783c-866b-4cc7-a460-3d5e5662c884 |
| AppRoleAssignment.ReadWrite.All                         | Delegado   | 84bccea3-f856-4a8a-967b-dbe0a3d53a64 |
| AppRoleAssignment.ReadWrite.All                         | Aplicativo | 06b708a9-e830-4db3-a914-8e69da51d44f |
| Approval.Read.All                                       | Delegado   | 1196552e-b226-4363-b01e-b8901fe10a11 |
| Approval.ReadWrite.All                                  | Delegado   | 1d3d0bc7-4b3a-427a-ae9f-6de4e1edc95f |
| AuditLog.Read.All                                       | Delegado   | e4c9e354-4dc5-45b8-9e7c-e1393b0b1a20 |
| AuditLog.Read.All                                       | Aplicativo | b0afded3-3588-46d8-8b3d-9842eff778da |
| BitlockerKey.Read.All                                   | Delegado   | b27a61ec-b99c-4d6a-b126-c4375d08ae30 |
| BitlockerKey.Read.All                                   | Aplicativo | 57f1cf28-c0c4-4ec3-9a30-19a2eaaf2f6e |
| BitlockerKey.ReadBasic.All                              | Delegado   | 5a107bfc-4f00-4e1a-b67e-66451267bc68 |
| BitlockerKey.ReadBasic.All                              | Aplicativo | f690d423-6b29-4d04-98c6-694c42282419 |
| Bookings.Manage.All                                     | Delegado   | 7f36b48e-542f-4d3b-9bcb-8406f0ab9fdb |
| Bookings.Read.All                                       | Delegado   | 33b1df99-4b29-4548-9339-7a7b83eaeebc |
| Bookings.ReadWrite.All                                  | Delegado   | 948eb538-f19d-4ec5-9ccc-f059e1ea4c72 |
| BookingsAppointment.ReadWrite.All                       | Delegado   | 02a5a114-36a6-46ff-a102-954d89d9ab02 |
| Calendars.Read                                          | Delegado   | 465a38f9-76ea-45b9-9f34-9e8b0d4b0b42 |
| Calendars.Read                                          | Aplicativo | 798ee544-9d2d-430c-a058-570e29e34338 |
| Calendars.Read.Shared                                   | Delegado   | 2b9c4092-424d-4249-948d-b43879977640 |
| Calendars.ReadWrite                                     | Delegado   | 1ec239c2-d7c9-4623-a91a-a9775856bb36 |
| Calendars.ReadWrite                                     | Aplicativo | ef54d2bf-783f-4e0f-bca1-3210c0444d99 |
| Calendars.ReadWrite.Shared                              | Delegado   | 12466101-c9b8-439a-8589-dd09ee67e8e9 |
| CallRecord-PstnCalls.Read.All                           | Aplicativo | a2611786-80b3-417e-adaa-707d4261a5f0 |
| CallRecords.Read.All                                    | Aplicativo | 45bbb07e-7321-4fd7-a8f6-3ff27e6a81c8 |
| Calls.AccessMedia.All                                   | Aplicativo | a7a681dc-756e-4909-b988-f160edc6655f |
| Calls.Initiate.All                                      | Aplicativo | 284383ee-7f6e-4e40-a2a8-e85dcb029101 |
| Calls.InitiateGroupCall.All                             | Aplicativo | 4c277553-8a09-487b-8023-29ee378d8324 |
| Calls.JoinGroupCall.All                                 | Aplicativo | f6b49018-60ab-4f81-83bd-22caeabfed2d |
| Calls.JoinGroupCallAsGuest.All                          | Aplicativo | fd7ccf6b-3d28-418b-9701-cd10f5cd2fd4 |
| Channel.Create                                          | Delegado   | 101147cf-4178-4455-9d58-02b5c164e759 |
| Channel.Create                                          | Aplicativo | f3a65bd4-b703-46df-8f7e-0174fea562aa |
| Channel.Delete.All                                      | Delegado   | cc83893a-e232-4723-b5af-bd0b01bcfe65 |
| Channel.Delete.All                                      | Aplicativo | 6a118a39-1227-45d4-af0c-ea7b40d210bc |
| Channel.ReadBasic.All                                   | Delegado   | 9d8982ae-4365-4f57-95e9-d6032a4c0b87 |
| Channel.ReadBasic.All                                   | Aplicativo | 59a6b24b-4225-4393-8165-ebaec5f55d7a |
| ChannelMember.Read.All                                  | Delegado   | 2eadaff8-0bce-4198-a6b9-2cfc35a30075 |
| ChannelMember.Read.All                                  | Aplicativo | 3b55498e-47ec-484f-8136-9013221c06a9 |
| ChannelMember.ReadWrite.All                             | Delegado   | 0c3e411a-ce45-4cd1-8f30-f99a3efa7b11 |
| ChannelMember.ReadWrite.All                             | Aplicativo | 35930dcf-aceb-4bd1-b99a-8ffed403c974 |
| ChannelMessage.Edit                                     | Delegado   | 2b61aa8a-6d36-4b2f-ac7b-f29867937c53 |
| ChannelMessage.Read.All                                 | Delegado   | 767156cb-16ae-4d10-8f8b-41b657c8c8c8c8 |
| ChannelMessage.Read.All                                 | Aplicativo | 7b2449af-6ccd-4f4d-9f78-e550c193f0d1 |
| ChannelMessage.Send                                     | Delegado   | ebf0f66e-9fb1-49e4-a278-222f76911cf4 |
| ChannelMessage.UpdatePolicyViolation.All                | Aplicativo | 4d02b0cc-d90b-441f-8d82-4fb55c34d6bb |
| ChannelSettings.Read.All                                | Delegado   | 233e0cf1-dd62-48bc-b65b-b38fe87fcf8e |
| ChannelSettings.Read.All                                | Aplicativo | c97b873f-f59f-49aa-8a0e-52b32d762124 |
| ChannelSettings.ReadWrite.All                           | Delegado   | d649fb7c-72b4-4eec-b2b4-b15acf79e378 |
| ChannelSettings.ReadWrite.All                           | Aplicativo | 243cded2-bd16-4fd6-a953-ff8177894c3d |
| Chat.Create                                             | Delegado   | 38826093-1258-4dea-98f0-00003be2b8d0 |
| Chat.Create                                             | Aplicativo | d9c48af6-9ad9-47ad-82c3-63757137b9af |
| Chat.Read                                               | Delegado   | f501c180-9344-439a-bca0-6cbf209fd270 |
| Chat.Read.All                                           | Aplicativo | 6b7d71a-70aa-4810-a8d9-5d9fb2830017 |
| Chat.ReadBasic                                          | Delegado   | 9547fcb5-d03f-419d-9948-5928bbf71b0f |
| Chat.ReadBasic.All                                      | Aplicativo | b2e060da-3baf-4687-9611-f4ebc0f0cbde |
| Chat.ReadWrite                                          | Delegado   | 9ff7295e-131b-4d94-90e1-69fde507ac11 |
| Chat.ReadWrite.All                                      | Aplicativo | 294ce7c9-31ba-490a-ad7d-97a7d075e4ed |
| Chat.UpdatePolicyViolation.All                          | Aplicativo | 7e847308-e030-4183-9899-5235d7270f58 |
| ChatMember.Read                                         | Delegado   | c5a9e2b1-faf6-41d4-8875-d381aa549b24 |
| ChatMember.Read.All                                     | Aplicativo | a3410be2-8e48-4f32-8454-c29a7465209d |
| ChatMember.ReadWrite                                    | Delegado   | dea13482-7ea6-488f-8b98-eb5bbecf033d |
| ChatMember.ReadWrite.All                                | Aplicativo | 57257249-34ce-4810-a8a2-a03adf0c5693 |
| ChatMessage.Read                                        | Delegado   | cdcdac3a-fd45-410d-83ef-554db620e5c7 |
| ChatMessage.Read.All                                    | Aplicativo | b9bb2381-47a4-46cd-aafb-00cb12f68504 |
| ChatMessage.Send                                        | Delegado   | 116b7235-7cc6-461e-b163-8e55691d839e |
| CloudPC.Read.All                                        | Delegado   | 5252ec4e-fd40-4d92-8c68-89dd1d3c6110 |
| CloudPC.Read.All                                        | Aplicativo | a9e09520-8ed4-4cde-838e-4fdea192c227 |
| CloudPC.ReadWrite.All                                   | Delegado   | 9d77138f-f0e2-47ba-ab33-cd246c8b79d1 |
| CloudPC.ReadWrite.All                                   | Aplicativo | 3b4349e1-8cf5-45a3-95b7-69d1751d3e6a |
| ConsentRequest.Read.All                                 | Delegado   | f3bfad56-966e-4590-a536-82ecf548ac1e |
| ConsentRequest.Read.All                                 | Aplicativo | 1260ad83-98fb-4785-abbb-d6cc1806fd41 |
| ConsentRequest.ReadWrite.All                            | Delegado   | 497d9dfa-3bd1-481a-baab-90895e54568c |
| ConsentRequest.ReadWrite.All                            | Aplicativo | 9f1b81a7-0223-4428-bfa4-0bcb5535f27d |
| Contacts.Read                                           | Delegado   | ff74d97f-43af-4b68-9f2a-b77ee6968c5d |
| Contacts.Read                                           | Aplicativo | 089fe4d0-434a-44c5-8827-41ba8a0b17f5 |
| Contacts.Read.Shared                                    | Delegado   | 242b9d9e-ed24-4d09-9a52-f43769beb9d4 |
| Contacts.ReadWrite                                      | Delegado   | d56682ec-c09e-4743-aaf4-1a3aac4caa21 |
| Contacts.ReadWrite                                      | Aplicativo | 6918b873-d17a-4dc1-b314-35f528134491 |
| Contacts.ReadWrite.Shared                               | Delegado   | afb6c84b-06be-49af-80bb-8f3f77004eab |
| CrossTenantInformation.ReadBasic.All                    | Delegado   | 81594d25-e88e-49cf-ac8c-fecbff49f994 |
| CrossTenantInformation.ReadBasic.All                    | Aplicativo | cac88765-0581-4025-9725-5ebc13f729ee |
| CrossTenantUserProfileSharing.Read                      | Delegado   | cb1ba48f-d22b-4325-a07f-74135a62ee41 |
| CrossTenantUserProfileSharing.Read.All                  | Delegado   | 759dcd16-3c90-463c-937e-abf89f991c18 |
| CrossTenantUserProfileSharing.Read.All                  | Aplicativo | 8b919d44-6192-4f3d-8a3b-f86f8069ae3c |
| CrossTenantUserProfileSharing.ReadWrite                 | Delegado   | eed0129d-dc60-4f30-8641-daf337a39ffd |
| CrossTenantUserProfileSharing.ReadWrite.All             | Delegado   | 64dfa325-cbf8-48e3-938d-51224a0cac01 |
| CrossTenantUserProfileSharing.ReadWrite.All             | Aplicativo | 306785c5-c09b-4ba0-a4ee-023f3da165cb |
| CustomSecAttributeAssignment.Read.All                   | Delegado   | b46ffa80-fe3d-4822-9a1a-c200932d54d0 |
| CustomSecAttributeAssignment.Read.All                   | Aplicativo | 3b37c5a4-1226-493d-bec3-5d6c6b866f3f3f |
| CustomSecAttributeAssignment.ReadWrite.All              | Delegado   | ca46335e-8453-47cd-a001-8459884efeae |
| CustomSecAttributeAssignment.ReadWrite.All              | Aplicativo | de89b5e4-5b8f-48eb-8925-29c2b33bd8bd |
| CustomSecAttributeDefinition.Read.All                   | Delegado   | ce026878-a0ff-4745-a728-d4fedd086c07 |
| CustomSecAttributeDefinition.Read.All                   | Aplicativo | b185aa14-d8d2-42c1-a685-0f5596613624 |
| CustomSecAttributeDefinition.ReadWrite.All              | Delegado   | 8b0160d4-5743-482b-bb27-efc0a485ca4a |
| CustomSecAttributeDefinition.ReadWrite.All              | Aplicativo | 12338004-21f4-4896-bf5e-b75dfaf1016d |
| DelegatedAdminRelationship.Read.All                     | Delegado   | 0c0064ea-477b-4130-82a5-4c2cc4ff68aa |
| DelegatedAdminRelationship.Read.All                     | Aplicativo | f6e9e124-4586-492f-adc0-c6f96e4823fd |
| DelegatedAdminRelationship.ReadWrite.All                | Delegado   | 885f682f-a990-4bad-a642-36736a74b0c7 |
| DelegatedAdminRelationship.ReadWrite.All                | Aplicativo | cc13eba4-8cd8-44c6-b4d4-f93237adce58 |
| DelegatedPermissionGrant.ReadWrite.All                  | Delegado   | 41ce6ca6-6826-4807-84f1-1c82854f7ee5 |
| DelegatedPermissionGrant.ReadWrite.All                  | Aplicativo | 8e8e4742-1d95-4f68-9d56-6ee75648c72a |
| Device.Command                                          | Delegado   | bac3b9c2-b516-4ef4-bd3b-c2ef73d8d804 |
| Device.Read                                             | Delegado   | 11d4cd79-5ba5-460f-803f-e22c8ab85ccd |
| Device.Read.All                                         | Delegado   | 951183d1-1a61-466f-a6d1-1fde911bfd95 |
| Device.Read.All                                         | Aplicativo | 7438b122-aefc-4978-80ed-43db9fcc7715 |
| Device.ReadWrite.All                                    | Aplicativo | 1138cb37-bd11-4084-a2b7-9f71582aeddb |
| DeviceManagementApps.Read.All                           | Delegado   | 4edf5f54-4666-44af-9de9-0144fb4b6e8c |
| DeviceManagementApps.Read.All                           | Aplicativo | 7a6ee1e7-141e-4cec-ae74-d9db155731ff |
| DeviceManagementApps.ReadWrite.All                      | Delegado   | 7b3f05d5-f68c-4b8d-8c59-a2ecd12f24af |
| DeviceManagementApps.ReadWrite.All                      | Aplicativo | 78145de6-330d-4800-a6ce-494ff2d33d07 |
| DeviceManagementConfiguration.Read.All                  | Delegado   | f1493658-876a-4c87-8fa7-edb559b3476a |
| DeviceManagementConfiguration.Read.All                  | Aplicativo | dc377aa6-52d8-4e23-b271-2a7ae04cedf3 |
| DeviceManagementConfiguration.ReadWrite.All             | Delegado   | 0883f392-0a7a-443d-8c76-16a6d39c7b63 |
| DeviceManagementConfiguration.ReadWrite.All             | Aplicativo | 9241abd9-d0e6-425a-bd4f-47ba86e767a4 |
| DeviceManagementManagedDevices.PrivilegedOperations.All | Delegado   | 3404d2bf-2b13-457e-a330-c24615765193 |
| DeviceManagementManagedDevices.PrivilegedOperations.All | Aplicativo | 5b07b0dd-2377-4e44-a38d-703f09a0dc3c |
| DeviceManagementManagedDevices.Read.All                 | Delegado   | 314874da-47d6-4978-88dc-cf0d37f0bb82 |
| DeviceManagementManagedDevices.Read.All                 | Aplicativo | 2f51be20-0bb4-4fed-bf7b-db946066c75e |
| DeviceManagementManagedDevices.ReadWrite.All            | Delegado   | 44642bfe-8385-4adc-8fc6-fe3cb2c375c3 |
| DeviceManagementManagedDevices.ReadWrite.All            | Aplicativo | 243333ab-4d21-40cb-a475-36241daa0842 |
| DeviceManagementRBAC.Read.All                           | Delegado   | 49f0cc30-024c-4dfd-ab3e-82e137ee5431 |
| DeviceManagementRBAC.Read.All                           | Aplicativo | 58ca0d9a-1575-47e1-a3cb-007ef2e4583b |
| DeviceManagementRBAC.ReadWrite.All                      | Delegado   | 0c5e8a55-87a6-4556-93ab-adc52c4d862d |
| DeviceManagementRBAC.ReadWrite.All                      | Aplicativo | e330c4f0-4170-414e-a55a-2f022ec2b57b |
| DeviceManagementServiceConfig.Read.All                  | Delegado   | 8696daa5-bce5-4b2e-83f9-51b6defc4e1e1e |
| DeviceManagementServiceConfig.Read.All                  | Aplicativo | 06a5fe6d-c49d-46a7-b082-56b1b14103c7 |
| DeviceManagementServiceConfig.ReadWrite.All             | Delegado   | 662ed50a-ac44-4eef-ad86-62eed9be2a29 |
| DeviceManagementServiceConfig.ReadWrite.All             | Aplicativo | 5ac13192-7ace-4fcf-b828-1a26f28068ee |
| Directory.AccessAsUser.All                              | Delegado   | 0e263e50-5827-48a4-b97c-d940288653c7 |
| Directory.Read.All                                      | Delegado   | 06da0dbc-49e2-44d2-8312-53f166ab848a |
| Directory.Read.All                                      | Aplicativo | 7ab1d382-f21e-4acd-a863-ba3e13f7da61 |
| Directory.ReadWrite.All                                 | Delegado   | c5366453-9fb0-48a5-a156-24f0c49a4b84 |
| Directory.ReadWrite.All                                 | Aplicativo | 19dbc75e-c2e2-444c-a770-ec69d8559fc7 |
| Directory.Write.Restricted                              | Delegado   | cba5390f-ed6a-4b7f-b657-0efc2210ed20 |
| Directory.Write.Restricted                              | Aplicativo | f20584af-9290-4153-9280-ff8bb2c0ea7f |
| DirectoryRecommendations.Read.All                       | Delegado   | 34d3bd24-f6a6-468c-b67c-0c365c1d6410 |
| DirectoryRecommendations.Read.All                       | Aplicativo | ae73097b-cb2a-4447-b064-5d80f6093921 |
| DirectoryRecommendations.ReadWrite.All                  | Delegado   | f37235e8-90a0-4189-93e2-e55b53867ccd |
| DirectoryRecommendations.ReadWrite.All                  | Aplicativo | 0e9eea12-4f01-45f6-9b8d-3ea4c8144158 |
| Domain.Read.All                                         | Delegado   | 2f9ee017-59c1-4f1d-9472-bd5529a7b311 |
| Domain.Read.All                                         | Aplicativo | dbb9058a-0e50-45d7-ae91-66909b5d4664 |
| Domain.ReadWrite.All                                    | Delegado   | 0b5d694c-a244-4bde-86e6-eb5cd07730fe |
| Domain.ReadWrite.All                                    | Aplicativo | 7e05723c-0bb0-42da-be95-ae9f08a6e53c |
| EAS.AccessAsUser.All                                    | Delegado   | ff91d191-45a0-43fd-b837-bd682c4a0b0f |
| eDiscovery.Read.All                                     | Delegado   | 99201db3-7652-4d5a-809a-bdb94f85fe3c |
| eDiscovery.Read.All                                     | Aplicativo | 50180013-6191-4d1e-a373-e590ff4e66af |
| eDiscovery.ReadWrite.All                                | Delegado   | acb8f680-0834-4146-b69e-4ab1b39745ad |
| eDiscovery.ReadWrite.All                                | Aplicativo | b2620db1-3bf7-4c5b-9cb9-576d29eac736 |
| EduAdministration.Read                                  | Delegado   | 8523895c-6081-45bf-8a5d-f062a2f12c9f |
| EduAdministration.Read.All                              | Aplicativo | 7c9db06a-ec2d-4e7b-a592-5a1e30992566 |
| EduAdministration.ReadWrite                             | Delegado   | 63589852-04e3-46b4-bae9-15d5b1050748 |
| EduAdministration.ReadWrite.All                         | Aplicativo | 9bc431c3-b8bc-4a8d-a219-40f10f92eff6 |
| EduAssignments.Read                                     | Delegado   | 091460c9-9c4a-49b2-81ef-1f3d852acce2 |
| EduAssignments.Read.All                                 | Aplicativo | 4c37e1b6-35a1-43bf-926a-6f30f2cdf585 |
| EduAssignments.ReadBasic                                | Delegado   | c0b0103b-c053-4b2e-9973-9f3a544ec9b8 |
| EduAssignments.ReadBasic.All                            | Aplicativo | 6e0a958b-b7fc-4348-b7c4-a6ab9fd3dd0e |
| EduAssignments.ReadWrite                                | Delegado   | 2f233e90-164b-4501-8bce-31af2559a2d3 |
| EduAssignments.ReadWrite.All                            | Aplicativo | 0d22204b-6cad-4dd0-8362-3e3f2ae699d9 |
| EduAssignments.ReadWriteBasic                           | Delegado   | 2ef770a1-622a-47c4-93ee-28d6adbed3a0 |
| EduAssignments.ReadWriteBasic.All                       | Aplicativo | f431cc63-a2de-48c4-8054-a34bc093af84 |
| EduRoster. Read                                          | Delegado   | a4389601-22d9-4096-ac18-36a927199112 |
| EduRoster.Read.All                                      | Aplicativo | e0ac9e1b-cb65-4fc5-87c5-1a8bc181f648 |
| EduRoster.ReadBasic                                     | Delegado   | 5d186531-d1bf-4f07-8cea-7c42119e1bd9 |
| EduRoster.ReadBasic.All                                 | Aplicativo | 0d412a8c-a06c-439f-b3ec-8abcf54d2f96 |
| EduRoster.ReadWrite                                     | Delegado   | 359e19a6-e3fa-4d7f-bcab-d28ec592b51e |
| EduRoster.ReadWrite.All                                 | Aplicativo | d1808e82-ce13-47af-ae0d-f9b254e6d58a |
| email                                                   | Delegado   | 64a6cdd6-aab1-4aaf-94b8-3cc8405e90d0 |
| EntitlementManagement.Read.All                          | Delegado   | 5449aa12-1393-4ea2-a7c7-d0e06c1a56b2 |
| EntitlementManagement.Read.All                          | Aplicativo | c74fd47d-ed3c-45c3-9a9e-b8676de685d2 |
| EntitlementManagement.ReadWrite.All                     | Delegado   | ae7a573d-81d7-432b-ad44-4ed5c9d89038 |
| EntitlementManagement.ReadWrite.All                     | Aplicativo | 9acd699f-1e81-4958-b001-93b1d2506e19 |
| EWS.AccessAsUser.All                                    | Delegado   | 9769c687-087d-48ac-9cb3-c37dde652038 |
| ExternalConnection.Read.All                             | Delegado   | a38267a5-26b6-4d76-9493-935b7599116b |
| ExternalConnection.Read.All                             | Aplicativo | 1914711b-a1cb-4793-b019-c2ce0ed21b8c |
| ExternalConnection.ReadWrite.All                        | Delegado   | bbbbd9b3-3566-4931-ac37-2b2180d9e334 |
| ExternalConnection.ReadWrite.All                        | Aplicativo | 34c37bc0-2b40-4d5e-85e1-2365cd256d79 |
| ExternalConnection.ReadWrite.OwnedBy                    | Delegado   | 4082ad95-c812-4f02-be92-780c4c4f1830 |
| ExternalConnection.ReadWrite.OwnedBy                    | Aplicativo | f431331c-49a6-499f-be1c-62af19c34a9d |
| ExternalItem.Read.All                                   | Delegado   | 922f9392-b1b7-483c-a4be-0089be7704fb |
| ExternalItem.Read.All                                   | Aplicativo | 7a7cffad-37d2-4f48-afa4-c6ab129adcc2 |
| ExternalItem.ReadWrite.All                              | Delegado   | b02c54f8-eb48-4c50-a9f0-a149e5a2012f |
| ExternalItem.ReadWrite.All                              | Aplicativo | 38c3d6ee-69ee-422f-b954-e17819665354 |
| ExternalItem.ReadWrite.OwnedBy                          | Delegado   | 4367b9d7-cee7-4995-853c-a0bdfe95c1f9 |
| ExternalItem.ReadWrite.OwnedBy                          | Aplicativo | 8116ae0f-55c2-452d-9944-d18420f5b2c8 |
| Family.Read                                             | Delegado   | 3a1e4806-a744-4c70-80fc-223bf8582c46 |
| Files.Read                                              | Delegado   | 10465720-29dd-4523-a11a-6a75c743c9d9 |
| Files.Read.All                                          | Delegado   | df85f4d6-205c-4ac5-a5ea-6bf408dba283 |
| Files.Read.All                                          | Aplicativo | 01d4889c-1287-42c6-ac1f-5d1e02578ef6 |
| Files.Read.Selected                                     | Delegado   | 5447fe39-cb82-4c1a-b977-520e67e724eb |
| Files.ReadWrite                                         | Delegado   | 5c28f0bf-8a70-41f1-8ab2-9032436ddb65 |
| Files.ReadWrite.All                                     | Delegado   | 863451e7-0667-486c-a5d6-d135439485f0 |
| Files.ReadWrite.All                                     | Aplicativo | 75359482-378d-4052-8f01-80520e7db3cd |
| Files.ReadWrite.AppFolder                               | Delegado   | 8019c312-3263-48e6-825e-2b833497195b |
| Files.ReadWrite.Selected                                | Delegado   | 17dde5bd-8c17-420f-a486-969730c1b827 |
| Financials.ReadWrite.All                                | Delegado   | f534bf13-55d4-45a9-8f3c-c92fe64d6131 |
| Group.Create                                            | Aplicativo | bf7b1a76-6e77-406b-b258-bf5c7720e98f |
| Group.Read.All                                          | Delegado   | 5f8c59db-677d-491f-a6b8-5f174b11ec1d |
| Group.Read.All                                          | Aplicativo | 5b567255-7703-4780-807c-7be8301ae99b |
| Group.ReadWrite.All                                     | Delegado   | 4e46008b-f24c-477d-8fff-7bb4ec7aafe0 |
| Group.ReadWrite.All                                     | Aplicativo | 62a82d76-70ea-41e2-9197-370581804d09 |
| GroupMember.Read.All                                    | Delegado   | bc024368-1153-4739-b217-4326f2e966d0 |
| GroupMember.Read.All                                    | Aplicativo | 98830695-27a2-44f7-8c18-0c3ebc9698f6 |
| GroupMember.ReadWrite.All                               | Delegado   | f81125ac-d3b7-4573-a3b2-7099cc39df9e |
| GroupMember.ReadWrite.All                               | Aplicativo | dbaae8cf-10b5-4b86-a4a1-f871c94c6695 |
| IdentityProvider.Read.All                               | Delegado   | 43781733-b5a7-4d1b-98f4-e8edff23e1a9 |
| IdentityProvider.Read.All                               | Aplicativo | e321f0bb-e7f7-481e-bb28-e3b0b32d4bd0 |
| IdentityProvider.ReadWrite.All                          | Delegado   | f13ce604-1677-429f-90bd-8a10b9f01325 |
| IdentityProvider.ReadWrite.All                          | Aplicativo | 90db2b9a-d928-4d33-a4dd-8442ae3d41e4 |
| IdentityRiskEvent.Read.All                              | Delegado   | 8f6a01e7-0391-4ee5-aa22-a3af122cef27 |
| IdentityRiskEvent.Read.All                              | Aplicativo | 6e472fd1-ad78-48da-a0f0-97ab2c6b769e |
| IdentityRiskEvent.ReadWrite.All                         | Delegado   | 9e4862a5-b68f-479e-848a-4e07e25c9916 |
| IdentityRiskEvent.ReadWrite.All                         | Aplicativo | db06fb33-1953-4b7b-a2ac-f1e2c854f7ae |
| IdentityRiskyServicePrincipal.Read.All                  | Delegado   | ea5c4ab0-5a73-4f35-8272-5d5337884e5d |
| IdentityRiskyServicePrincipal.Read.All                  | Aplicativo | 607c7344-0eed-41e5-823a-9695ebe1b7b0 |
| IdentityRiskyServicePrincipal.ReadWrite.All             | Delegado   | bb6f654c-d7fd-4ae3-85c3-fc380934f515 |
| IdentityRiskyServicePrincipal.ReadWrite.All             | Aplicativo | cb8d6980-6bcb-4507-afec-ed6de3a2d798 |
| IdentityRiskyUser.Read.All                              | Delegado   | d04bb851-cb7c-4146-97c7-ca3e71baf56c |
| IdentityRiskyUser.Read.All                              | Aplicativo | dc5007c0-2d7d-4c42-879c-2dab87571379 |
| IdentityRiskyUser.ReadWrite.All                         | Delegado   | e0a7cdbb-08b0-4697-8264-0069786e9674 |
| IdentityRiskyUser.ReadWrite.All                         | Aplicativo | 656f6061-f9fe-4807-9708-6a2e0934df76 |
| IdentityUserFlow.Read.All                               | Delegado   | 2903d63d-4611-4d43-99ce-a33f3f52e343 |
| IdentityUserFlow.Read.All                               | Aplicativo | 1b0c317f-dd31-4305-9932-259a8b6e8099 |
| IdentityUserFlow.ReadWrite.All                          | Delegado   | 281892cc-4dbf-4e3a-b6cc-b21029bb4e82 |
| IdentityUserFlow.ReadWrite.All                          | Aplicativo | 65319a09-a2be-469d-8782-f6b07debf789 |
| IMAP.AccessAsUser.All                                   | Delegado   | 652390e4-393a-48de-9484-05f9b1212954 |
| InformationProtectionContent.Sign.All                   | Aplicativo | cbe6c7e4-09aa-4b8d-b3c3-2dbb59af4b54 |
| InformationProtectionContent.Write.All                  | Aplicativo | 287bd98c-e865-4e8c-bade-1a85523195b9 |
| InformationProtectionPolicy. Read                        | Delegado   | 4ad84827-5578-4e18-ad7a-86530b12f884 |
| InformationProtectionPolicy.Read.All                    | Aplicativo | 19da66cb-0fb0-4390-b071-ebc76a349482 |
| LicenseAssignment.ReadWrite.All                         | Delegado   | f55016cc-149c-447e-8f21-7cf3ec1d6350 |
| LicenseAssignment.ReadWrite.All                         | Aplicativo | 5facf0c1-8979-4e95-abcf-ff3d079771c0 |
| Mail.Read                                               | Delegado   | 570282fd-fa5c-430d-a7fd-fc8dc98a9dca |
| Mail.Read                                               | Aplicativo | 810c84a8-4a9e-49e6-bf7d-12d183f40d01 |
| Mail.Read.Shared                                        | Delegado   | 7b9103a5-4610-446b-9670-80643382c1fa |
| Mail.ReadBasic                                          | Delegado   | a4b8392a-d8d1-4954-a029-8e668a39a170 |
| Mail.ReadBasic                                          | Aplicativo | 6be147d2-ea4f-4b5a-a3fa-3eab6f3c140a |
| Mail.ReadBasic.All                                      | Aplicativo | 693c5e45-0940-467d-9b8a-1022fb9d42ef |
| Mail.ReadWrite                                          | Delegado   | 024d486e-b451-40bb-833d-3e66d98c5c73 |
| Mail.ReadWrite                                          | Aplicativo | e2a3a72e-5f79-4c64-b1b1-878b674786c9 |
| Mail.ReadWrite.Shared                                   | Delegado   | 5df07973-7d5d-46ed-9847-1271055cbd51 |
| Mail.Send                                               | Delegado   | e383f46e-2787-4529-855e-0e479a3ffac0 |
| Mail.Send                                               | Aplicativo | b633e1c5-b582-4048-a93e-9f11b44c7e96 |
| Mail.Send.Shared                                        | Delegado   | a367ab51-6b49-43bf-a716-a1fb06d2a174 |
| MailboxSettings.Read                                    | Delegado   | 87f447af-9fa4-4c32-9dfa-4a57a73d18ce |
| MailboxSettings.Read                                    | Aplicativo | 40f97065-369a-49f4-947c-6a255697ae91 |
| MailboxSettings.ReadWrite                               | Delegado   | 818c620a-27a9-40bd-a6a5-d96f7d610b4b |
| MailboxSettings.ReadWrite                               | Aplicativo | 6931bccd-447a-43d1-b442-00a195474933 |
| ManagedTenants.Read.All                                 | Delegado   | dc34164e-6c4a-41a0-be89-3ae2fbad7cd3 |
| ManagedTenants.ReadWrite.All                            | Delegado   | b31fa710-c9b3-4d9e-8f5e-8036eecddab9 |
| Member.Read.Hidden                                      | Delegado   | f6a3db3e-f7e8-4ed2-a414-557c8c9830be |
| Member.Read.Hidden                                      | Aplicativo | 658aa5d8-239f-45c4-aa12-864f4fc7e490 |
| Notes.Create                                            | Delegado   | 9d822255-d64d-4b7a-afdb-833b9a97ed02 |
| Notes.Read                                              | Delegado   | 371361e4-b9e2-4a3f-8315-2a301a3b0a3d |
| Notes.Read.All                                          | Delegado   | dfabfca6-ee36-4db2-8208-7a28381419b3 |
| Notes.Read.All                                          | Aplicativo | 3aeca27b-ee3a-4c2b-8ded-80376e2134a4 |
| Notes.ReadWrite                                         | Delegado   | 615e26af-c38a-4150-ae3e-c3b0d4cb1d6a |
| Notes.ReadWrite.All                                     | Delegado   | 64ac0503-b4fa-45d9-b544-71a463f05da0 |
| Notes.ReadWrite.All                                     | Aplicativo | 0c458cef-11f3-48c2-a568-c66751c238c0 |
| Notes.ReadWrite.CreatedByApp                            | Delegado   | ed68249d-017c-4df5-9113-e684c7f8760b |
| Notifications.ReadWrite.CreatedByApp                    | Delegado   | 89497502-6e42-46a2-8cb2-427fd3df970a |
| offline_access                                          | Delegado   | 7427e0e9-2fba-42fe-b0c0-848c9e6a8182 |
| OnlineMeetingArtifact.Read.All                          | Delegado   | 110e5abb-a10c-4b59-8b55-9b4daa4ef743 |
| OnlineMeetingArtifact.Read.All                          | Aplicativo | df01ed3b-eb61-4eca-9965-6b3d789751b2 |
| OnlineMeetingRecording.Read.All                         | Delegado   | 190c2bb6-1fdd-4fec-9aa2-7d571b5e1fe3 |
| OnlineMeetingRecording.Read.All                         | Aplicativo | a4a08342-c95d-476b-b943-97e100569c8d |
| OnlineMeetings.Read                                     | Delegado   | 9be106e1-f4e3-4df5-bdff-e4bc531cbe43 |
| OnlineMeetings.Read.All                                 | Aplicativo | c1684f21-1984-47fa-9d61-2dc8c296bb70 |
| OnlineMeetings.ReadWrite                                | Delegado   | a65f2972-a4f8-4f5e-afd7-69ccb046d5dc |
| OnlineMeetings.ReadWrite.All                            | Aplicativo | b8bb2037-6e08-44ac-a4ea-4674e010e2a4 |
| OnlineMeetingTranscript.Read.All                        | Delegado   | 30b87d18-ebb1-45db-97f8-82ccb1f0190c |
| OnlineMeetingTranscript.Read.All                        | Aplicativo | a4a80d8d-d283-4bd8-8504-555ec3870630 |
| OnPremisesPublishingProfiles.ReadWrite.All              | Delegado   | 8c4d5184-71c2-4bf8-bb9d-bc3378c9ad42 |
| OnPremisesPublishingProfiles.ReadWrite.All              | Aplicativo | 0b57845e-aa49-4e6f-8109-ce654fffa618 |
| openid                                                  | Delegado   | 37f7f235-527c-4136-accd-4a02d197296e |
| Organization.Read.All                                   | Delegado   | 4908d5b9-3fb2-4b1e-9336-1888b7937185 |
| Organization.Read.All                                   | Aplicativo | 498476ce-e0fe-48b0-b801-37ba7e2685c6 |
| Organization.ReadWrite.All                              | Delegado   | 46ca0847-7e6b-426e-9775-ea810a948356 |
| Organization.ReadWrite.All                              | Aplicativo | 292d869f-3427-49a8-9dab-8c70152b74e9 |
| OrgContact.Read.All                                     | Delegado   | 08432d1b-5911-483c-86df-7980af5cdee0 |
| OrgContact.Read.All                                     | Aplicativo | e1a88a34-94c4-4418-be12-c87b00e26bea |
| People.Read                                             | Delegado   | ba47897c-39ec-4d83-8086-ee8256fa737d |
| People.Read.All                                         | Delegado   | b89f9189-71a5-4e70-b041-9887f0bc7e4a |
| People.Read.All                                         | Aplicativo | b528084d-ad10-4598-8b93-929746b4d7d6 |
| Place.Read.All                                          | Delegado   | cb8f45a0-5c2e-4ea1-b803-84b870a7d7ec |
| Place.Read.All                                          | Aplicativo | 913b9306-0ce1-42b8-9137-6a7df690a760 |
| Place.ReadWrite.All                                     | Delegado   | 4c06a06a-098a-4063-868e-5dfee3827264 |
| Policy.Read.All                                         | Delegado   | 572fea84-0151-49b2-9301-11cb16974376 |
| Policy.Read.All                                         | Aplicativo | 246dd0d5-5bd0-4def-940b-0421030a5b68 |
| Policy.Read.ConditionalAccess                           | Delegado   | 633e0fce-8c58-4cfb-9495-12bbd5a24f7c |
| Policy.Read.ConditionalAccess                           | Aplicativo | 37730810-e9ba-4e46-b07e-8ca78d182097 |
| Policy.Read.PermissionGrant                             | Delegado   | 414de6ea-2d92-462f-b120-6e2a809a6d01 |
| Policy.Read.PermissionGrant                             | Aplicativo | 9e640839-a198-48fb-8b9a-013fd6f6cbcd |
| Policy.ReadWrite.ApplicationConfiguration               | Delegado   | b27add92-efb2-4f16-84f5-8108ba77985c |
| Policy.ReadWrite.ApplicationConfiguration               | Aplicativo | be74164b-cff1-491c-8741-e671cb536e13 |
| Policy.ReadWrite.AuthenticationFlows                    | Delegado   | edb72de9-4252-4d03-a925-451deef99db7 |
| Policy.ReadWrite.AuthenticationFlows                    | Aplicativo | 25f85f3c-f66c-4205-8cd5-de92dd7f0cec |
| Policy.ReadWrite.AuthenticationMethod                   | Delegado   | 7e823077-d88e-468f-a337-e18f1f0e6c7c |
| Policy.ReadWrite.AuthenticationMethod                   | Aplicativo | 29c18626-4985-4dcd-85c0-193eef327366 |
| Policy.ReadWrite.Authorization                          | Delegado   | edd3c878-b384-41fd-95ad-e7407dd775be |
| Policy.ReadWrite.Authorization                          | Aplicativo | fb221be6-99f2-473f-bd32-01c6a0e9ca3b |
| Policy.ReadWrite.ConditionalAccess                      | Delegado   | ad902697-1014-4ef5-81ef-2b4301988e8c |
| Policy.ReadWrite.ConditionalAccess                      | Aplicativo | 01c0a623-fc9b-48e9-b794-0756f8e8f067 |
| Policy.ReadWrite.ConsentRequest                         | Delegado   | 4d135e65-66b8-41a8-9f8b-081452c91774 |
| Policy.ReadWrite.ConsentRequest                         | Aplicativo | 999f8c63-0a38-4f1b-91fd-ed1947bdd1a9 |
| Policy.ReadWrite.CrossTenantAccess                      | Delegado   | 014b43d0-6ed4-4fc6-84dc-4b6f7bae7d85 |
| Policy.ReadWrite.CrossTenantAccess                      | Aplicativo | 338163d7-f101-4c92-94ba-ca46fe52447c |
| Policy.ReadWrite.DeviceConfiguration                    | Delegado   | 40b534c3-9552-4550-901b-23879c90bcf9 |
| Policy.ReadWrite.FeatureRollout                         | Delegado   | 92a38652-f13b-4875-bc77-6e1dbb63e1b2 |
| Policy.ReadWrite.FeatureRollout                         | Aplicativo | 2044e4f1-e56c-435b-925c-44cd8f6ba89a |
| Policy.ReadWrite.MobilityManagement                     | Delegado   | a8ead177-1889-4546-9387-f25e658e2a79 |
| Policy.ReadWrite.PermissionGrant                        | Delegado   | 2672f8bb-fd5e-42e0-85e1-ec764ddd2614e |
| Policy.ReadWrite.PermissionGrant                        | Aplicativo | a402ca1c-2696-4531-972d-6e5ee4aa11ea |
| Policy.ReadWrite.TrustFramework                         | Delegado   | cefba324-1a70-4a6e-9c1d-fd670b7ae392 |
| Policy.ReadWrite.TrustFramework                         | Aplicativo | 79a677f7-b79d-40d0-a36a-3e6f8688dd7a |
| POP.AccessAsUser.All                                    | Delegado   | d7b7f2d9-0f45-4ea1-9d42-e50810c06991 |
| Presence.Read                                           | Delegado   | 76bc735e-aecd-4a1d-8b4c-2b915deabb79 |
| Presence.Read.All                                       | Delegado   | 9c7a330d-35b3-4aa1-963d-cb2b9f927841 |
| Presence.ReadWrite                                      | Delegado   | 8d3c54a7-cf58-4773-bf81-c0cd6ad522bb |
| Presence.ReadWrite.All                                  | Aplicativo | 83cded22-8297-4ff6-a7fa-e97e9545a259 |
| PrintConnector.Read.All                                 | Delegado   | d69c2d6d-4f72-4f99-a6b9-663e32f8cf68 |
| PrintConnector.ReadWrite.All                            | Delegado   | 79ef9967-7d59-4213-9c64-4b10687637d8 |
| Printer.Create                                          | Delegado   | 90c30bed-6fd1-4279-bf39-714069619721 |
| Printer.FullControl.All                                 | Delegado   | 93dae4bd-43a1-4a23-9a1a-92957e1d9121 |
| Printer.Read.All                                        | Delegado   | 3a736c8a-018e-460a-b60c-863b2683e8bf |
| Printer.Read.All                                        | Aplicativo | 9709bb33-4549-49d4-8ed9-a8f65e45bb0f |
| Printer.ReadWrite.All                                   | Delegado   | 89f66824-725f-4b8f-928e-e1c5258dc565 |
| Printer.ReadWrite.All                                   | Aplicativo | f5b3f73d-6247-44df-a74c-866173fddab0 |
| PrinterShare.Read.All                                   | Delegado   | ed11134d-2f3f-440d-a2e1-411efada2502 |
| PrinterShare.ReadBasic.All                              | Delegado   | 5fa075e9-b951-4165-947b-c63396ff0a37 |
| PrinterShare.ReadWrite.All                              | Delegado   | 06ceea37-85e2-40d7-bec3-91337a46038f |
| PrintJob.Create                                         | Delegado   | 21f0d9c0-9f13-48b3-94e0-b6b231c7d320 |
| PrintJob.Manage.All                                     | Aplicativo | 58a52f47-9e36-4b17-9ebe-ce4ef7f3e6c8 |
| PrintJob.Read                                           | Delegado   | 248f5528-65c0-4c88-8326-876c7236df5e |
| PrintJob.Read.All                                       | Delegado   | afdd6933-a0d8-40f7-bd1a-b5d778e8624b |
| PrintJob.Read.All                                       | Aplicativo | ac6f956c-edea-44e4-bd06-64b1b4b9aec9 |
| PrintJob.ReadBasic                                      | Delegado   | 6a71a747-280f-4670-9ca0-a9cbf882b274 |
| PrintJob.ReadBasic.All                                  | Delegado   | 04ce8d60-72ce-4867-85cf-6d82f36922f3 |
| PrintJob.ReadBasic.All                                  | Aplicativo | fbf67eee-e074-4ef7-b965-ab5ce1c1f689 |
| PrintJob.ReadWrite                                      | Delegado   | b81dd597-8abb-4b3f-a07a-820b0316ed04 |
| PrintJob.ReadWrite.All                                  | Delegado   | 036b9544-e8c5-46ef-900a-0646cc42b271 |
| PrintJob.ReadWrite.All                                  | Aplicativo | 5114b07b-2898-4de7-a541-53b0004e2e13 |
| PrintJob.ReadWriteBasic                                 | Delegado   | 6f2d22f2-1cb6-412c-a17c-3336817eaa82 |
| PrintJob.ReadWriteBasic.All                             | Delegado   | 3a0db2f6-0d2a-4c19-971b-49109b19ad3d |
| PrintJob.ReadWriteBasic.All                             | Aplicativo | 57878358-37f4-4d3a-8c20-4816e0d457b1 |
| PrintSettings.Read.All                                  | Delegado   | 490f32fd-d90f-4dd7-a601-ff6cdc1a3f6c |
| PrintSettings.Read.All                                  | Aplicativo | b5991872-94cf-4652-9765-29535087c6d8 |
| PrintSettings.ReadWrite.All                             | Delegado   | 9ccc526a-c51c-4e5c-a1fd-74726ef50b8f |
| PrintTaskDefinition.ReadWrite.All                       | Aplicativo | 456b71a7-0ee0-4588-9842-c123fcc8f664 |
| PrivilegedAccess.Read.AzureAD                           | Delegado   | b3a539c9-59cb-4ad5-825a-041ddbdc2bdb |
| PrivilegedAccess.Read.AzureAD                           | Aplicativo | 4cdc2547-9148-4295-8d11-be0db1391d6b |
| PrivilegedAccess.Read.AzureADGroup                      | Delegado   | d329c81c-20ad-4772-abf9-3f6fdb7e5988 |
| PrivilegedAccess.Read.AzureADGroup                      | Aplicativo | 01e37dc9-c035-40bd-b438-b2879c4870a6 |
| PrivilegedAccess.Read.AzureResources                    | Delegado   | 1d89d70c-dcac-4248-b214-903c457af83a |
| PrivilegedAccess.Read.AzureResources                    | Aplicativo | 5df6fe86-1be0-44eb-b916-7bd443a71236 |
| PrivilegedAccess.ReadWrite.AzureAD                      | Delegado   | 3c3c74f5-cdaa-4a97-b7e0-4e788bfcfb37 |
| PrivilegedAccess.ReadWrite.AzureAD                      | Aplicativo | 854d9ab1-6657-4ec8-be45-823027bcd009 |
| PrivilegedAccess.ReadWrite.AzureADGroup                 | Delegado   | 32531c59-1f32-461f-b8df-6f8a3b89f73b |
| PrivilegedAccess.ReadWrite.AzureADGroup                 | Aplicativo | 2f6817f8-7b12-4f0f-bc18-eeaf60705a9e |
| PrivilegedAccess.ReadWrite.AzureResources               | Delegado   | a84a9652-ffd3-496e-a991-22ba5529156a |
| PrivilegedAccess.ReadWrite.AzureResources               | Aplicativo | 6f9d5abc-2db6-400b-a267-7de22a40fb87 |
| perfil                                                 | Delegado   | 14dad69e-099b-42c9-810b-d002981feec1 |
| ProgramControl.Read.All                                 | Delegado   | c492a2e1-2f8f-4caa-b076-99bbf6e40fe4 |
| ProgramControl.Read.All                                 | Aplicativo | eedb7fdd-7539-4345-a38b-4839e4a84cbd |
| ProgramControl.ReadWrite.All                            | Delegado   | 50fd364f-9d93-4ae1-b170-300e87cccf84 |
| ProgramControl.ReadWrite.All                            | Aplicativo | 60a901ed-09f7-4aa5-a16e-7dd3d6f9de36 |
| RecordsManagement.Read.All                              | Delegado   | 07f995eb-fc67-4522-ad66-2b8ca8ea3efd |
| RecordsManagement.Read.All                              | Aplicativo | ac3a2b8e-03a3-4da9-9ce0-cbe28bf1accd |
| RecordsManagement.ReadWrite.All                         | Delegado   | f2833d75-a4e6-40ab-86d4-6dfe73c97605 |
| RecordsManagement.ReadWrite.All                         | Aplicativo | eb158f57-df43-4751-8b21-b8932adb3d34 |
| Reports.Read.All                                        | Delegado   | 02e97553-ed7b-43d0-ab3c-f8bace0d040c |
| Reports.Read.All                                        | Aplicativo | 230c1aed-a721-4c5d-9cb4-a90514e508ef |
| RoleAssignmentSchedule.Read.Directory                   | Delegado   | 344a729c-0285-42c6-9014-f12b9b8d6129 |
| RoleAssignmentSchedule.ReadWrite.Directory              | Delegado   | 8c026be3-8e26-4774-9372-8d5d6f21daff |
| RoleEligibilitySchedule.Read.Directory                  | Delegado   | eb0788c2-6d4e-4658-8c9e-c0fb8053f03d |
| RoleEligibilitySchedule.ReadWrite.Directory             | Delegado   | 62ade113-f8e0-4bf9-a6ba-5acb31db32fd |
| RoleManagement.Read.All                                 | Delegado   | 48fec646-b2ba-4019-8681-8eb31435aded |
| RoleManagement.Read.All                                 | Aplicativo | c7fbd983-d9aa-4fa7-84b8-17382c103bc4 |
| RoleManagement.Read.CloudPC                             | Delegado   | 9619b88a-8a25-48a7-9571-d23be0337a79 |
| RoleManagement.Read.CloudPC                             | Aplicativo | 031a549a-bb80-49b6-8032-2068448c6a3c |
| RoleManagement.Read.Directory                           | Delegado   | 741c54c3-0c1e-44a1-818b-3f97ab4e8c83 |
| RoleManagement.Read.Directory                           | Aplicativo | 483bed4a-2ad3-4361-a73b-c83ccdbdc53c |
| RoleManagement.ReadWrite.CloudPC                        | Delegado   | 501d06f8-07b8-4f18-b5c6-c191a4af7a82 |
| RoleManagement.ReadWrite.CloudPC                        | Aplicativo | 274d0592-d1b6-44bd-af1d-26d259bcb43a |
| RoleManagement.ReadWrite.Directory                      | Delegado   | d01b97e9-cbc0-49fe-810a-750afd5527a3 |
| RoleManagement.ReadWrite.Directory                      | Aplicativo | 9e3f62cf-ca93-4989-b6ce-bf83c28f9fe8 |
| RoleManagementPolicy.Read.Directory                     | Delegado   | 3de2cdbe-0ff5-47d5-bdee-7f45b4749ead |
| RoleManagementPolicy.ReadWrite.Directory                | Delegado   | 1ff1be21-34eb-448c-9ac9-ce1f506b2a68 |
| Schedule.Read.All                                       | Delegado   | fccf6dd8-5706-49fa-811f-69e2e1b585d0 |
| Schedule.Read.All                                       | Aplicativo | 7b2ebf90-d836-437f-b90d-7b62722c4456 |
| Schedule.ReadWrite.All                                  | Delegado   | 63f27281-c9d9-4f29-94dd-6942f7f1feb0 |
| Schedule.ReadWrite.All                                  | Aplicativo | b7760610-0545-4e8a-9ec3-cce9e63db01c |
| SearchConfiguration.Read.All                            | Delegado   | 7d307522-aa38-4cd0-bd60-90c6f0ac50bd |
| SearchConfiguration.Read.All                            | Aplicativo | ada977a5-b8b1-493b-9a91-66c206d76ecf |
| SearchConfiguration.ReadWrite.All                       | Delegado   | b1a7d408-cab0-47d2-a2a5-a74a3733600d |
| SearchConfiguration.ReadWrite.All                       | Aplicativo | 0e778b85-fefa-466d-9eec-750569d92122 |
| SecurityActions.Read.All                                | Delegado   | 1638cddf-07a4-4de2-8645-69c96cacad73 |
| SecurityActions.Read.All                                | Aplicativo | 5e0edab9-c148-49d0-b423-ac253e121825 |
| SecurityActions.ReadWrite.All                           | Delegado   | dc38509c-b87d-4da0-bd92-6bec988bac4a |
| SecurityActions.ReadWrite.All                           | Aplicativo | f2bf083f-0179-402a-bedb-b2784de8a49b |
| SecurityAlert.Read.All                                  | Delegado   | bc257fb8-46b4-4b15-8713-01e91bfbe4ea |
| SecurityAlert.Read.All                                  | Aplicativo | 472e4a4d-bb4a-4026-98d1-0b0d74cb74a5 |
| SecurityAlert.ReadWrite.All                             | Delegado   | 471f2a7f-2a42-4d45-a2bf-594d0838070d |
| SecurityAlert.ReadWrite.All                             | Aplicativo | ed4fca05-be46-441f-9803-1873825f8fdb |
| SecurityEvents.Read.All                                 | Delegado   | 64733abd-851e-478a-bffb-e47a14b18235 |
| SecurityEvents.Read.All                                 | Aplicativo | bf394140-e372-4bf9-a898-299cfc7564e5 |
| SecurityEvents.ReadWrite.All                            | Delegado   | 6aedf524-7e1c-45a7-bd76-ded8cab8d0fc |
| SecurityEvents.ReadWrite.All                            | Aplicativo | d903a879-88e0-4c09-b0c9-82f6a1333f84 |
| SecurityIncident.Read.All                               | Delegado   | b9abcc4f-94fc-4457-9141-d20ce80ec952 |
| SecurityIncident.Read.All                               | Aplicativo | 45cc0394-e837-488b-a098-1918f48d186c |
| SecurityIncident.ReadWrite.All                          | Delegado   | 128ca929-1a19-45e6-a3b8-435ec44a36ba |
| SecurityIncident.ReadWrite.All                          | Aplicativo | 34bf0e97-1971-4929-b999-9e2442d941d7 |
| ServiceHealth.Read.All                                  | Delegado   | 55896846-df78-47a7-aa94-8d3d4442ca7f |
| ServiceHealth.Read.All                                  | Aplicativo | 79c261e0-fe76-4144-aad5-bdc68fbe4037 |
| ServiceMessage.Read.All                                 | Delegado   | eda39fa6-f8cf-4c3c-a909-432c683e4c9b |
| ServiceMessage.Read.All                                 | Aplicativo | 1b620472-6534-4fe6-9df2-4680e8aa28ec |
| ServiceMessageViewpoint.Write                           | Delegado   | 636e1b0b-1cc2-4b1c-9aa9-4eeed9b9761b |
| ServicePrincipalEndpoint.Read.All                       | Delegado   | 9f9ce928-e038-4e3b-8faf-7b59049a8ddc |
| ServicePrincipalEndpoint.Read.All                       | Aplicativo | 5256681e-b7f6-40c0-8447-2d9db68797a0 |
| ServicePrincipalEndpoint.ReadWrite.All                  | Delegado   | 7297d82c-9546-4aed-91df-3d4f0a9b3ff0 |
| ServicePrincipalEndpoint.ReadWrite.All                  | Aplicativo | 89c8469c-83ad-45f7-8ff2-6e3d4285709e |
| SharePointTenantSettings.Read.All                       | Delegado   | 2ef70e10-5bfd-4ede-a5f6-67720500b258 |
| SharePointTenantSettings.Read.All                       | Aplicativo | 83d4163d-a2d8-4d3b-9695-4ae3ca98f888 |
| SharePointTenantSettings.ReadWrite.All                  | Delegado   | aa07f155-3612-49b8-a147-6c590df35536 |
| SharePointTenantSettings.ReadWrite.All                  | Aplicativo | 19b94e34-907c-4f43-bde9-38b1909ed408 |
| ShortNotes.Read                                         | Delegado   | 50f66e47-eb56-45b7-aaa2-75057d9afe08 |
| ShortNotes.Read.All                                     | Aplicativo | 0c7d31ec-31ca-4f58-b6ec-9950b6b0de69 |
| ShortNotes.ReadWrite                                    | Delegado   | 328438b7-4c01-4c07-a840-e625a749bb89 |
| ShortNotes.ReadWrite.All                                | Aplicativo | 842c284c-763d-4a97-838d-79787d129bab |
| Sites.FullControl.All                                   | Delegado   | 5a54b8b3-347c-476d-8f8e-42d5c7424d29 |
| Sites.FullControl.All                                   | Aplicativo | a82116e5-55eb-4c41-a434-62fe8a61c773 |
| Sites.Manage.All                                        | Delegado   | 65e50fdc-43b7-4915-933e-e8138f11f40a |
| Sites.Manage.All                                        | Aplicativo | 0c0bf378-bf22-4481-8f81-9e89a9b4960a |
| Sites.Read.All                                          | Delegado   | 205e70e5-aba6-4c52-a976-6d2d46c48043 |
| Sites.Read.All                                          | Aplicativo | 332a536c-c7ef-4017-ab91-336970924f0d |
| Sites.ReadWrite.All                                     | Delegado   | 89fe6a52-be36-487e-b7d8-d061c450a026 |
| Sites.ReadWrite.All                                     | Aplicativo | 9492366f-7969-46a4-8d15-ed1a20078fff |
| Sites.Selecionados                                          | Aplicativo | 883ea226-0bf2-4a8f-9f9d-92c9162a727d |
| SMTP.Send                                               | Delegado   | 258f6531-6087-4cc4-bb90-092c5fb3ed3f |
| SubjectRightsRequest.Read.All                           | Delegado   | 9c3af74c-fd0f-4db4-b17a-71939e2a9d77 |
| SubjectRightsRequest.ReadWrite.All                      | Delegado   | 2b8fcc74-bce1-4ae3-a0e8-60c53739299d |
| Subscription.Read.All                                   | Delegado   | 5f88184c-80bb-4d52-9ff2-757288b2e9b7 |
| Tasks.Read                                              | Delegado   | f45671fb-e0fe-4b4b-be20-3d3ce43f1bcb |
| Tasks.Read.All                                          | Aplicativo | f10e1f91-74ed-437f-a6fd-d6ae88e26c1f |
| Tasks.Read.Shared                                       | Delegado   | 88d21fd4-8e5a-4c32-b5e2-4a1c95f34f72 |
| Tasks.ReadWrite                                         | Delegado   | 2219042f-cab5-40cc-b0d2-16b1540b4c5f |
| Tasks.ReadWrite.All                                     | Aplicativo | 44e666d1-d276-445b-a5fc-8815eeb81d55 |
| Tasks.ReadWrite.Shared                                  | Delegado   | c5ddf11b-c114-4886-8558-8a4e557cd52b |
| Team.Create                                             | Delegado   | 7825d5d6-6049-4ce7-bdf6-3b8d53f4bcd0 |
| Team.Create                                             | Aplicativo | 23fc2474-f741-46ce-8465-674744c5c361 |
| Team.ReadBasic.All                                      | Delegado   | 485be79e-c497-4b35-9400-0e3fa7f2a5d4 |
| Team.ReadBasic.All                                      | Aplicativo | 2280dda6-0bfd-44ee-a2f4-cb867cfc4c1e |
| TeamMember.Read.All                                     | Delegado   | 2497278c-d82d-46a2-b1ce-39d4cdde5570 |
| TeamMember.Read.All                                     | Aplicativo | 660b7406-55f1-41ca-a0ed-0b035e182f3e |
| TeamMember.ReadWrite.All                                | Delegado   | 4a06efd2-f825-4e34-813e-82a57b03d1ee |
| TeamMember.ReadWrite.All                                | Aplicativo | 0121dc95-1b9f-4aed-8bac-58c5ac466691 |
| TeamMember.ReadWriteNonOwnerRole.All                    | Delegado   | 2104a4db-3a2f-4ea0-9dba-143d457dc666 |
| TeamMember.ReadWriteNonOwnerRole.All                    | Aplicativo | 4437522e-9a86-4a41-a7da-e380edd4a97d |
| TeamsActivity.Read                                      | Delegado   | 0e755559-83fb-4b44-91d0-4cc721b9323e |
| TeamsActivity.Read.All                                  | Aplicativo | 70dec828-f620-4914-aa83-a29117306807 |
| TeamsActivity.Send                                      | Delegado   | 7ab1d787-bae7-4d5d-8db6-37ea32df9186 |
| TeamsActivity.Send                                      | Aplicativo | a267235f-af13-44dc-8385-c1dc93023186 |
| TeamsAppInstallation.ReadForChat                        | Delegado   | bf3fbf03-f35f-4e93-963e-47e4d874c37a |
| TeamsAppInstallation.ReadForChat.All                    | Aplicativo | cc7e7635-2586-41d6-adaa-a8d3bcad5ee5 |
| TeamsAppInstallation.ReadForTeam                        | Delegado   | 5248dcb1-f83b-4ec3-9f4d-a4428a961a72 |
| TeamsAppInstallation.ReadForTeam.All                    | Aplicativo | 1f615aea-6bf9-4b05-84bd-46388e138537 |
| TeamsAppInstallation.ReadForUser                        | Delegado   | c395395c-ff9a-4dba-bc1f-8372ba9dca84 |
| TeamsAppInstallation.ReadForUser.All                    | Aplicativo | 9ce09611-f4f7-4abd-a629-a05450422a97 |
| TeamsAppInstallation.ReadWriteForChat                   | Delegado   | aa85bf13-d771-4d5d-a9e6-bca04ce44edf |
| TeamsAppInstallation.ReadWriteForChat.All               | Aplicativo | 9e19bae1-2623-4c4f-ab6e-2664615ff9a0 |
| TeamsAppInstallation.ReadWriteForTeam                   | Delegado   | 2e25a044-2580-450d-8859-42eeb6e996c0 |
| TeamsAppInstallation.ReadWriteForTeam.All               | Aplicativo | 5dad17ba-f6cc-4954-a5a2-a0dcc95154f0 |
| TeamsAppInstallation.ReadWriteForUser                   | Delegado   | 093f8818-d05f-49b8-95bc-9d2a73e9a43c |
| TeamsAppInstallation.ReadWriteForUser.All               | Aplicativo | 74ef0291-ca83-4d02-8c7e-d2391e6a444f |
| TeamsAppInstallation.ReadWriteSelfForChat               | Delegado   | 0ce33576-30e8-43b7-99e5-62f8569a4002 |
| TeamsAppInstallation.ReadWriteSelfForChat.All           | Aplicativo | 73a45059-f39c-4baf-9182-4954ac0e55cf |
| TeamsAppInstallation.ReadWriteSelfForTeam               | Delegado   | 0f4595f7-64b1-4e13-81bc-11a249df07a9 |
| TeamsAppInstallation.ReadWriteSelfForTeam.All           | Aplicativo | 9f67436c-5415-4e7f-8ac1-3014a7132630 |
| TeamsAppInstallation.ReadWriteSelfForUser               | Delegado   | 207e0cb1-3ce7-4922-b991-5a760c346ebc |
| TeamsAppInstallation.ReadWriteSelfForUser.All           | Aplicativo | 908de74d-f8b2-4d6b-a9ed-2a17b3b78179 |
| TeamSettings.Read.All                                   | Delegado   | 48638b3c-ad68-4383-8ac4-e6880ee6ca57 |
| TeamSettings.Read.All                                   | Aplicativo | 242607bd-1d2c-432c-82eb-bdb27baa23ab |
| TeamSettings.ReadWrite.All                              | Delegado   | 39d65650-9d3e-4223-80db-a335590d027e |
| TeamSettings.ReadWrite.All                              | Aplicativo | bdd80a03-d9bc-451d-b7c4-ce7c63fe3c8f |
| TeamsTab.Create                                         | Delegado   | a9ff19c2-f369-4a95-9a25-ba9d460efc8e |
| TeamsTab.Create                                         | Aplicativo | 49981c42-fd7b-4530-be03-e77b21aed25e |
| TeamsTab.Read.All                                       | Delegado   | 59dacb05-e88d-4c13-a684-59f1afc8cc98 |
| TeamsTab.Read.All                                       | Aplicativo | 46890524-499a-4bb2-ad64-1476b4f3e1cf |
| TeamsTab.ReadWrite.All                                  | Delegado   | b98bfd41-87c6-45cc-b104-e2de4f0dafb9 |
| TeamsTab.ReadWrite.All                                  | Aplicativo | a96d855f-016b-47d7-b51c-1218a98d791c |
| TeamsTab.ReadWriteForChat                               | Delegado   | ee928332-e9c2-4747-b4a0-f8c164b68de6 |
| TeamsTab.ReadWriteForChat.All                           | Aplicativo | fd9ce730-a250-40dc-bd44-8dc8d20f39ea |
| TeamsTab.ReadWriteForTeam                               | Delegado   | c975dd04-a06e-4fbb-9704-62daad77bb49 |
| TeamsTab.ReadWriteForTeam.All                           | Aplicativo | 6163d4f4-fbf8-43da-a7b4-060fe85ed148 |
| TeamsTab.ReadWriteForUser                               | Delegado   | c37c9b61-7762-4bff-a156-afc0005847a0 |
| TeamsTab.ReadWriteForUser.All                           | Aplicativo | 425b4b59-d5af-45c8-832f-bb0b7402348a |
| TeamsTab.ReadWriteSelfForChat                           | Delegado   | 0c219d04-3abf-47f7-912d-5cca239e90e6 |
| TeamsTab.ReadWriteSelfForChat.All                       | Aplicativo | 9f62e4a2-a2d6-4350-b28b-d244728c4f86 |
| TeamsTab.ReadWriteSelfForTeam                           | Delegado   | f266662f-120a-4314-b26a-99b08617c7ef |
| TeamsTab.ReadWriteSelfForTeam.All                       | Aplicativo | 91c32b81-0ef0-453f-a5c7-4ce2e562f449 |
| TeamsTab.ReadWriteSelfForUser                           | Delegado   | 395dfec1-a0b9-465f-a783-8250a430cb8c |
| TeamsTab.ReadWriteSelfForUser.All                       | Aplicativo | 3c42dec6-49e8-4a0a-b469-36cff0d9da93 |
| Teamwork.Migrate.All                                    | Aplicativo | dfb0dd15-61de-45b2-be36-d6a69fba3c79 |
| TeamworkDevice.Read.All                                 | Delegado   | b659488b-9d28-4208-b2be-1c6652b3c970 |
| TeamworkDevice.Read.All                                 | Aplicativo | 0591bafd-7c1c-4c30-a2a5-2b9aacb1dfe8 |
| TeamworkDevice.ReadWrite.All                            | Delegado   | ddd97ecb-5c31-43db-a235-0ee20e635c40 |
| TeamworkDevice.ReadWrite.All                            | Aplicativo | 79c02f5b-bd4f-4713-bc2c-a8a4a66e127b |
| TeamworkTag.Read                                        | Delegado   | 57587d0b-8399-45be-b207-8050cec54575 |
| TeamworkTag.Read                                    | Aplicativo | b74fd6c4-4bde-488e-9695-eeb100e4907f |
| TeamworkTag.ReadWrite                                   | Delegado   | 539dabd7-b5b6-4117-b164-d60cd15a8671 |
| TeamworkTag.ReadWrite                               | Aplicativo | a3371ca5-911d-46d6-901c-42c8c7a937d8 |
| TermStore.Read.All                                      | Delegado   | 297f747b-0005-475b-8fef-c890f5152b38 |
| TermStore.Read.All                                      | Aplicativo | ea047cc2-df29-4f3e-83a3-205de61501ca |
| TermStore.ReadWrite.All                                 | Delegado   | 6c37c71d-f50f-4bff-8fd3-8a41da390140 |
| TermStore.ReadWrite.All                                 | Aplicativo | f12eb8d6-28e3-46e6-b2c0-b7e4dc69fc95 |
| ThreatAssessment.Read.All                               | Aplicativo | f8f035bb-2cce-47fb-8bf5-7baf3ecbee48 |
| ThreatAssessment.ReadWrite.All                          | Delegado   | cac97e40-6730-457d-ad8d-4852fddab7ad |
| ThreatHunting.Read.All                                  | Delegado   | b152eca8-ea73-4a48-8c98-1a6742673d99 |
| ThreatHunting.Read.All                                  | Aplicativo | dd98c7f5-2d42-42d3-a0e4-633161547251 |
| ThreatIndicators.Read.All                               | Delegado   | 9cc427b4-2004-41c5-aa22-757b755e9796 |
| ThreatIndicators.Read.All                               | Aplicativo | 197ee4e9-b993-4066-898f-d6aecc55125b |
| ThreatIndicators.ReadWrite.OwnedBy                      | Delegado   | 91e7d36d-022a-490f-a748-f8e011357b42 |
| ThreatIndicators.ReadWrite.OwnedBy                      | Aplicativo | 21792b6c-c986-4ffc-85de-df9da54b52fa |
| TrustFrameworkKeySet.Read.All                           | Delegado   | 7ad34336-f5b1-44ce-8682-31d7dfcd9ab9 |
| TrustFrameworkKeySet.Read.All                           | Aplicativo | fff194f1-7dce-4428-8301-1badb5518201 |
| TrustFrameworkKeySet.ReadWrite.All                      | Delegado   | 39244520-1e7d-4b4a-aee0-57c65826e427 |
| TrustFrameworkKeySet.ReadWrite.All                      | Aplicativo | 4a771c9a-1cf2-4609-b88e-3d3e02d539cd |
| UnifiedGroupMember.Read.AsGuest                         | Delegado   | 73e75199-7c3e-41bb-9357-167164dbb415 |
| User.Export.All                                         | Delegado   | 405a51b5-8d8d-430b-9842-8be4b0e9f324 |
| User.Export.All                                         | Aplicativo | 405a51b5-8d8d-430b-9842-8be4b0e9f324 |
| User.Invite.All                                         | Delegado   | 63dd7cd9-b489-4adf-a28c-ac38b9a0f962 |
| User.Invite.All                                         | Aplicativo | 09850681-111b-4a89-9bed-3f2cae46d706 |
| User.ManageIdentities.All                               | Delegado   | 637d7bec-b31e-4deb-acc9-24275642a2c9 |
| User.ManageIdentities.All                               | Aplicativo | c529cfca-c91b-489c-af2b-d92990b66ce6 |
| User.Read                                               | Delegado   | e1fe6dd8-ba31-4d61-89e7-88639da4683d |
| User.Read.All                                           | Delegado   | a154be20-db9c-4678-8ab7-66f6cc099a59 |
| User.Read.All                                           | Aplicativo | df021288-bdef-4463-88db-98f22de89214 |
| User.ReadBasic.All                                      | Delegado   | b340eb25-3456-403f-be2f-af7a0d370277 |
| User.ReadWrite                                          | Delegado   | b4e74841-8e56-480b-be8b-910348b18b4c |
| User.ReadWrite.All                                      | Delegado   | 204e0828-b5ca-4ad8-b9f3-f32a958e7cc4 |
| User.ReadWrite.All                                      | Aplicativo | 741f803b-c850-494e-b5df-cde7c675a1ca |
| UserActivity.ReadWrite.CreatedByApp                     | Delegado   | 47607519-5fb1-47d9-99c7-da4b48f369b1 |
| UserAuthenticationMethod.Read                           | Delegado   | 1f6b61c5-2f65-4135-9c9f-31c0f8d32b52 |
| UserAuthenticationMethod.Read.All                       | Delegado   | aec28ec7-4d02-4e8c-b864-50163aea77eb |
| UserAuthenticationMethod.Read.All                       | Aplicativo | 38d9df27-64da-44fd-b7c5-a6fbac20248f |
| UserAuthenticationMethod.ReadWrite                      | Delegado   | 48971fc1-70d7-4245-af77-0beb29b53ee2 |
| UserAuthenticationMethod.ReadWrite.All                  | Delegado   | b7887744-6746-4312-813d-72daeaee7e2d |
| UserAuthenticationMethod.ReadWrite.All                  | Aplicativo | 50483e42-d915-4231-9639-7fdb7fd190e5 |
| UserNotification.ReadWrite.CreatedByApp                 | Delegado   | 26e2f3e8-b2a1-47fc-9620-89bb5b042024 |
| UserNotification.ReadWrite.CreatedByApp                 | Aplicativo | 4e774092-a092-48d1-90bd-baad67c7eb47 |
| UserShiftPreferences.Read.All                           | Aplicativo | de023814-96df-4f53-9376-1e2891ef5a18 |
| UserShiftPreferences.ReadWrite.All                      | Aplicativo | d1eec298-80f3-49b0-9efb-d90e224798ac |
| UserTimelineActivity.Write.CreatedByApp                 | Delegado   | 367492fc-594d-4972-a9b5-0d58c622c91c |
| WindowsUpdates.ReadWrite.All                            | Delegado   | 11776c0c-6138-4db3-a668-ee621bea2555 |
| WindowsUpdates.ReadWrite.All                            | Aplicativo | 7dd1be58-6e76-4401-bf8d-31d1e8180d5b |
| WorkforceIntegration.Read.All                           | Delegado   | f1ccd5a7-6383-466a-8db8-1a656f7d06fa |
| WorkforceIntegration.ReadWrite.All                      | Delegado   | 08c4b377-0d23-4a8b-be2a-23c1c1d88545 |
| WorkforceIntegration.ReadWrite.All                      | Aplicativo | 202bf709-e8e6-478e-bcfd-5d63c50b68e3 |
