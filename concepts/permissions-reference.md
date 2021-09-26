---
title: 'Referência de permissões do Microsoft Graph '
description: O Microsoft Graph expõe as permissões granulares que controlam o acesso que os aplicativos têm aos recursos, como email, grupos e usuários. Como desenvolvedor, você decide quais permissões para o Microsoft Graph seu aplicativo deverá solicitar.
author: jackson-woods
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: eb6644eae1f41f3eb5422a385720f22d88b0aa19
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763328"
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

> **Observação**: Em cenários delegados, as permissões efetivas concedidas ao aplicativo podem ser limitadas pelos privilégios do usuário conectado na organização.

## <a name="microsoft-accounts-and-work-or-school-accounts"></a>Contas da Microsoft e contas corporativas e de estudante

Nem todas as permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante. Você pode escolher **Conta de suporte da Microsoft** para cada grupo de permissão para determinar se uma permissão específica é válida para contas da Microsoft, contas corporativas ou de estudante ou ambas.

## <a name="permissions-availability-status"></a>Status de disponibilidade de permissões

As permissões do Microsoft Graph no [portal do Azure](https://portal.azure.com/) geralmente estão disponíveis e no status DG para todos os aplicativos usarem, exceto alguns conjuntos que estão no status de visualização ou visualização privada. As permissões na visualização estão disponíveis para o público; elas podem mudar e podem não ser promovidas ao status DG. As permissões no status de visualização privada não estão disponíveis e talvez nunca sejam disponibilizadas ao público. Não use as permissões no status de visualização ou visualização privada em aplicativos de produção.

## <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>Limitações de pesquisa de usuário e grupo para usuários convidados em organizações

Os recursos de pesquisa de usuário e grupo permitem que o aplicativo pesquise usuários ou grupos em um diretório da organização executando consultas no conjunto de recursos `/users` ou `/groups` (por exemplo, `https://graph.microsoft.com/v1.0/users`). Os administradores e os usuários têm esse recurso. No entanto, os usuários convidados não.

Se o usuário conectado for um usuário convidado, dependendo das permissões que recebeu um aplicativo, ele pode ler o perfil de um usuário específico ou grupo (por exemplo, `https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`). No entanto, o usuário não pode executar consultas no conjunto de recursos `/users` ou `/groups` que, potencialmente, retornam mais de um recurso.

Com as permissões apropriadas, o aplicativo pode ler os perfis de usuários ou grupos que ele obtém seguindo os links nas propriedades de navegação. Por exemplo, `/users/{id}/directReports` ou `/groups/{id}/members`.

## <a name="limited-information-returned-for-inaccessible-member-objects"></a>Informações limitadas retornadas para objetos membro inacessíveis

Objetos de contêiner, como grupos, oferecem suporte a membros de vários tipos; por exemplo, usuários e dispositivos. Quando um aplicativo consulta a associação de um objeto contêiner e não tem permissão para ler um determinado tipo, os membros desse tipo são retornados, mas com informações limitadas.  O aplicativo recebe umas 200 respostas e uma coleção de objetos.  Informações completas são retornadas para os tipos de objetos que o aplicativo tem permissões para ler.  Para os tipos de objetos que o aplicativo não tem permissão para ler, apenas o tipo e a ID do objeto são retornados.

Isso é aplicado a todos as relações que são do tipo [directoryObject](/graph/api/resources/directoryobject) (não apenas aos links de membro). Os exemplos incluem `/groups/{id}/members`, `/users/{id}/memberOf` ou `me/ownedObjects`.

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

## <a name="retrieving-permission-ids"></a>Recuperando as IDs de permissão

Se precisar definir permissões usando a CLI do Azure, PowerShell ou infraestrutura como estruturas de código, talvez seja necessário o identificador da permissão que deseja usar em vez do nome. Você pode usar a CLI do Azure para recuperar o identificador executando `az ad sp list`. No entanto, isso gera uma lista muito longa e pode ser difícil encontrar a permissão específica desejada. Se você já sabe o nome da permissão de que precisa, pode executar o seguinte comando usando a CLI do Azure:

```bash
az ad sp list --query "[?appDisplayName=='Microsoft Graph'].{permissions:oauth2Permissions}[0].permissions[?value=='<NAME OF PERMISSION>'].{id: id, value: value, adminConsentDisplayName: adminConsentDisplayName, adminConsentDescription: adminConsentDescription}[0]" --all
```

A resposta deve ser semelhante ao exemplo a seguir, que contém a descrição, identificador, nome de exibição e nome da permissão:

```json
{
  "adminConsentDescription": "Allows the app to list groups, and to read their properties and all group memberships on behalf of the signed-in user.  Also allows the app to read calendar, conversations, files, and other group content for all groups the signed-in user can access. ",
  "adminConsentDisplayName": "Read all groups",
  "id": "5f8c59db-677d-491f-a6b8-5f174b11ec1d",
  "value": "Group.Read.All"
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

Nenhum.

### <a name="remarks"></a>Comentários

No momento o único catálogo é a lista de aplicativos no [Microsoft Teams](teams-concept-overview.md).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegated
* _AppCatalog.ReadWrite.All_: [Lista todos os aplicativos no catálogo](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true) (`GET /beta/appCatalogs/teamsApps`)
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

A permissão _Application.ReadWrite.OwnedBy_ admite as mesmas operações que _Application.ReadWrite.All_, exceto que a anterior só permite essas operações em aplicativos e entidades de serviço que pertencem ao aplicativo de chamada. O proprietário é indicado pela propriedade de navegação `owners` no recurso do [aplicativo](/graph/api/application-list-owners?view=graph-rest-beta&preserve-view=true) ou da [entidade de serviço](/graph/api/serviceprincipal-list-owners?view=graph-rest-beta&preserve-view=true) de destino.
> OBSERVAÇÃO: o uso da permissão _Application.ReadWrite.OwnedBy_ para chamar `GET /applications` para listar aplicativos falhará com um erro 403.  Use `GET servicePrincipals/{id}/ownedObjects` para listar os aplicativos que pertencem ao aplicativo da chamada.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _Application.Read.All_: listar todos os aplicativos (`GET /beta/applications`)
* _Application.ReadWrite.All_: atualizar uma entidade de serviço (`PATCH /beta/servicePrincipals/{id}`)

#### <a name="application"></a>Aplicativo

* _Application.Read.All_: listar todos os aplicativos (`GET /beta/applications`)
* _Application.ReadWrite.All_: excluir uma entidade de serviço (`DELETE /beta/servicePrincipals/{id}`)
* _Application.ReadWrite.OwnedBy_: criar um aplicativo (`POST /beta/applications`)
* _Application.ReadWrite.OwnedBy_: Listar todos os aplicativos pertencentes ao aplicativo da chamada (`GET /beta/servicePrincipals/{id}/ownedObjects`)
* _Application.ReadWrite.OwnedBy_: adicionar outro proprietário a um aplicativo próprio (`POST /applications/{id}/owners/$ref`).
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
| _BitlockerKey.ReadBasic.All_ | Ler as informações básicas das chaves do BitLocker | Permite que um aplicativo leia as propriedades da chave do BitLocker para todos os dispositivos no locatário. A chave de recuperação não será retornada. | Sim | Não |
| _BitlockerKey.Read.All_ | Ler a chave do BitLocker | Permite que um aplicativo leia as chaves do BitLocker para todos os dispositivos no locatário. A chave de recuperação será retornada. | Sim | Não |

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

Nenhuma.

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
|_Calls.Initiate.All_|Iniciar chamadas de saída 1:1 do aplicativo (visualização)|Permite que o aplicativo faça chamadas de saída para um único usuário e transfira chamadas para usuários no diretório da sua organização, sem um usuário conectado.|Sim|
|_Calls.InitiateGroupCall.All_|Iniciar a saída de chamadas de grupo do aplicativo (visualização)|Permite que o aplicativo faça chamadas para vários usuários e adicione participantes a reuniões em sua organização, sem um usuário conectado.|Sim|
|_Calls.JoinGroupCall.All_|Ingressar em reuniões e chamadas de grupo como um aplicativo (visualização)|Permite que o aplicativo ingresse em reuniões agendadas e chamadas de grupo em sua organização, sem um usuário conectado. O aplicativo será associado aos privilégios de um usuário do diretório para reuniões em seu locatário.|Sim|
|_Calls.JoinGroupCallasGuest.All_|Ingressar em reuniões e chamadas de grupo como um convidado (visualização)|Permite que o aplicativo ingresse anonimamente no grupo chamadas e em reuniões agendadas em sua organização, sem um usuário conectado. O aplicativo ingressará como convidado para reuniões em seu locatário.|Sim|
|_Calls.AccessMedia.All_\*|Acessar fluxos de mídia em uma chamada como um aplicativo (visualização)|Permite que o aplicativo obtenha acesso direto aos fluxos de mídia em uma chamada sem um usuário conectado.|Sim|

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
|_ChannelMessage.Delete_ (visualização privada)|Excluir mensagens de canal do usuário |Permite que um aplicativo exclua mensagens de canal no Microsoft Teams, em nome do usuário conectado. |Sim | Não |
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

## <a name="chatmessage-permissions-private-preview"></a>ChatMessage permissions ([visualização privada](#permissions-availability-status))

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChatMessage.Send_ (visualização privada) | Enviar mensagens de chat do usuário | Permite que o aplicativo envie mensagens de chat individuais e de grupo no Microsoft Teams, em nome do usuário conectado. | Não | Não |

---

## <a name="cloud-pc-permissions"></a>Permissões do PC na nuvem

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_CloudPC.Read.All_ | Leia PCs na Internet | Permite que o aplicativo leia objetos do PC na Internet, como políticas de provisionamento, em nome do usuário conectado. | Não | Não |
|_CloudPC.ReadWrite.All_ | Ler e escrever PCs na Internet | Permite que o aplicativo crie, leia, atualize e exclua objetos do PC na Internet, como conexões locais, políticas de provisionamento e imagens do dispositivo, em nome do usuário. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_CloudPC.Read.All_ | Leia PCs na Internet | Permite que o aplicativo leia objetos do PC na Internet, como políticas de provisionamento, sem um usuário conectado. | Não | Não |
|_CloudPC.ReadWrite.All_ | Ler e escrever PCs na Internet | Permite que o aplicativo crie, leia, atualize e exclua objetos do PC na Internet, como conexões locais, políticas de provisionamento e imagens de dispositivo, sem um usuário conectado. | Sim | Não |

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

Elas também controlam exclusivamente o acesso a outros recursos de diretório como: [contatos organizacionais](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true), [APIs de extensão de esquema](/graph/api/resources/schemaextension?view=graph-rest-beta&preserve-view=true), [APIs de PIM (Privileged Identity Management)](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) e muitos dos recursos e APIs listados no nó **Azure Active Directory** na documentação de referência da API beta e v1.0. Isso inclui unidades administrativas, funções de diretório, configurações de diretório, política e muito mais.

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

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Domain.ReadWrite.All_ | Ler e registrar domínios | Permite que o aplicativo leia e escreva domínios sem um usuário conectado. | Sim |

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
| _EduRoster.ReadBasic_           | Ler um subconjunto limitado do modo de exibição dos usuários da lista de participantes               | Permite que o aplicativo leia um subconjunto limitado das propriedades da estrutura de escolas e classes da lista de participantes de uma organização e um subconjunto limitado das propriedades dos usuários a serem lidos em nome do usuário. Inclui nome, status, função de formação, endereço de email e foto. | Sim                    | Não                          |
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

_IdentityProvider.Read.All_ e _IdentityProvider.ReadWrite.All_ são válidos apenas para contas corporativas ou de estudantes. Para que um aplicativo leia ou grave provedores de identidade com permissões delegadas, o usuário conectado deve ter a função de Administrador Global. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

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

## <a name="identity-risk-event-permissions"></a>Permissões de eventos de risco de identidade

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade  | Permite que o aplicativo para leia as informações de evento de risco de identidade para todos os usuários em sua organização em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade | Permite que o aplicativo leia as informações do evento de risco de identidade para todos os usuários em sua organização sem um usuário conectado. | Sim |


### <a name="remarks"></a>Comentários

_IdentityRiskEvent.Read.All_ é válido apenas para contas corporativas ou de estudante. No caso de um aplicativo com permissões delegadas para ler as informações de risco de identidade, o usuário conectado deve ser um membro de uma das seguintes funções de administrador: Administrador Global, Administrador de Segurança ou funções do Leitor de Segurança. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated-and-application"></a>Permissões delegadas e de aplicativo

Os seguintes usos são válidos para Permissões Delegadas e Permissões de aplicativo:

* Ler todos os eventos de risco gerados para todos os usuários do locatário (`GET /beta/identityRiskEvents`)
* Ler todos os eventos de risco de malware gerados pelo botnet Dorknet (`GET /beta/malwareRiskEvents?$filter=malwareName eq 'Dorkbot'`)
* Ler os mais recentes 50 eventos de risco (`GET /beta/identityRiskEvents?$orderBy=riskEventDateTime desc&top=50`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---


## <a name="identity-risky-user-permissions"></a>Permissões de usuário com risco de identidade

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityRiskyUser.Read.All_ |   Leia as informações de risco de identidade do usuário.  | Permite que o aplicativo para leia as informações de risco de identidade do usuário para todos os usuários em sua organização em nome do usuário conectado. | Sim | Não |
| _IdentityRiskyUser.ReadWrite.All_ |   Ler e atualizar as informações de risco de identidade do usuário.  | Permite que o aplicativo leia as informações de risco de identidade do usuário para todos os usuários em sua organização em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskyUser.Read.All_ |   Leia as informações de risco de identidade do usuário. | Permite que o aplicativo leia as informações de risco de identidade do usuário para todos os usuários em sua organização sem um usuário conectado. | Sim |
| _IdentityRiskyUser.ReadWrite.All_ |   Ler e atualizar as informações de risco de identidade do usuário. | Permite que o aplicativo leia as informações de risco de identidade do usuário para todos os usuários em sua organização sem um usuário conectado. | Sim |


### <a name="remarks"></a>Comentários

_IdentityRiskUser.Read.All_ e _IdentityRiskyUser.ReadWrite.ALL_ são válidos apenas para contas corporativas ou de estudante. No caso de um aplicativo com permissões delegadas para ler as informações de risco de identidade do usuário, o usuário conectado deve ser um membro de uma das seguintes funções de administrador: Administrador Global, Administrador de Segurança ou funções do Leitor de Segurança. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated-and-application"></a>Permissões delegadas e de aplicativo

Os seguintes usos são válidos para Permissões Delegadas e Permissões de aplicativo:

* Ler todos os usuários de risco e propriedades no locatário (`GET /beta/riskyUsers`)
* Ler todos os usuários de risco cujo nível de risco agregação é Médio (`GET /beta/riskyUsers?$filter=risk/riskLevelAggregated eq microsoft.graph.riskLevel'medium'`)
* Leia as informações de riscos de um usuário específico (`GET /beta/riskyUsers/$filter=id eq ‘{userObjectId}’`)

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
| _Mail.ReadBasic_ |    Ler emails básicos do usuário | Permite que o aplicativo leia e-mails na caixa de correio do usuário conectado, exceto **body**, **bodyPreview**, **uniqueBody**, **anexos**, **extensões**, e quaisquer propriedades estendidas. Não inclui permissões para pesquisar mensagens. | Não | Não
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

## <a name="notifications-permissions"></a>Permissões de notificações
#### <a name="delegated-permissions"></a>Permissões delegadas
|Permissão    |Exibir Cadeia de Caracteres   |Descrição |Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notifications.ReadWrite.CreatedByApp_ | Exibir e gerenciar notificações para esse aplicativo. | Permitir que o aplicativo forneça notificações em nome de usuários conectados. Também permite que o aplicativo leia, atualize e exclua itens de notificação do usuário para este aplicativo. |Não |
### <a name="remarks"></a>Comentários
*Notifications.ReadWrite.CreatedByApp* é válida tanto para contas da Microsoft como para contas corporativas e de estudante.
A restrição *CreatedByApp* associada a essa permissão indica que o serviço aplicará filtragem implícita aos resultados com base na identidade aplicativo que realizar a chamada, seja a ID de aplicativo da conta  Microsoft ou um conjunto de IDs de aplicativos configurados para uma identidade de aplicativo de plataformas cruzadas.
### <a name="example-usage"></a>Exemplo de uso
#### <a name="delegated"></a>Delegated
* _Notifications.ReadWrite.CreatedByApp_: 
Publique uma notificação centrada no usuário, que pode ser entregue aos vários clientes do aplicativo em execução em pontos de extremidade diferentes. (POSTAGEM/me/notificações /).

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

## <a name="openid-permissions"></a>Permissões do OpenID

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _email_ |    Exibir o endereço de email do usuário | Permite ao aplicativo ler o endereço de email principal do usuário. | Não | Não |
| _offline_access_ |    Acessar dados do usuário a qualquer momento | Permite ao aplicativo ler e atualizar dados do usuário, mesmo quando eles não estiver usando o aplicativo.| Não | Não |
| _openid_ |    Conectar os usuários | Permite aos usuários entrar no aplicativo com contas corporativas ou de estudante e permite ao aplicativo ver informações básicas do perfil do usuário.| Não | Não |
| _profile_ |    Exibir os perfis básicos dos usuários | Permite que o aplicativo veja o perfil básico do usuário (nome, foto, nome de usuário).| Não | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

Nenhum.

### <a name="remarks"></a>Comentários
Você pode usar essas permissões para especificar os artefatos que deseja que sejam retornados nas solicitações de token e de autorização do Azure AD. O suporte a elas é oferecido de formas diferentes nos pontos de extremidade v 1.0 e v 2.0. do Azure AD.

Com o ponto de extremidade (v 1.0) do Azure AD, somente a permissão _openid_ é usada. Você especifica no parâmetro *scope*, na solicitação de autorização, para retornar um token de ID quando usar o protocolo OpenID Connect para conectar um usuário ao seu aplicativo. Para saber mais, confira o artigo [Autorizar o acesso aos aplicativos web usando o OpenID Connect e o Azure Active Directory](/azure/active-directory/develop/active-directory-protocols-openid-connect-code). Para retornar com êxito um token de ID, você também deve garantir que a permissão _User.Read_ esteja configurada quando você registrar seu aplicativo.

Com o ponto de extremidade v 2.0 do Azure AD, você especifica a permissão _offline\_access_ no parâmetro _scope_ para solicitar explicitamente um token de atualização quando estiver usando os protocolos OAuth 2.0 ou OpenID Connect. Com o OpenID Connect, você especifica a permissão _openid_ para solicitar um token de ID. Também é possível especificar a permissão _email_, a permissão _profile_, ou ambas, para retornar declarações adicionais no token de ID. Você não precisa especificar a _User.Read_ para retornar um token de ID com o ponto de extremidade v 2.0. Para saber mais, confira os [escopos do OpenID Connect](/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes).

> **Importante** A Biblioteca de Autenticação da Microsoft (MSAL) atualmente especifica as permissões _offline\_access_, _openid_, _profile_ e _email_ por padrão nas solicitações de autorização e de token. Isso significa que, para o caso padrão, se você especificar explicitamente essas permissões, o Azure AD pode retornar um erro.

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
| _Policy.ReadWrite.Authorization_ | Ler e gravar a política de autorização da sua organização | Permite que o aplicativo leia e grave a política de autorização da sua organização, em nome do usuário conectado.  Por exemplo, as políticas de autorização podem controlar algumas das permissões que a função do usuário pronto tem por padrão. | Sim | Não |
| _Policy.ReadWrite.ConditionalAccess_ | Ler e gravar as políticas de acesso condicional da sua organização | Permite que o aplicativo leia e grave todas as políticas de acesso condicional em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.ConsentRequest_ | Ler e escrever a política de solicitações de consentimento da sua organização | Permite que o aplicativo leia e grave a política de solicitações de consentimento da sua organização, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.FeatureRollout_ | Ler e gravar as políticas de implantação de novos recursos da sua organização | Permite que o aplicativo leia e grave todas as políticas de implantação de novos recursos em nome do usuário conectado. Inclui habilidades para atribuir e remover usuários e grupos para a implantação de um recurso específico. | Sim | Não |
| _Policy.ReadWrite.PermissionGrant_ | Gerenciar as políticas de concessão de consentimento e permissão | Permite que o aplicativo gerencie as políticas relacionadas a concessões de consentimento e permissão para aplicativos, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.TrustFramework_ | Ler e gravar as políticas TrustFramework (Estrutura de Confiança) da sua organização | Permite que o aplicativo leia e grave todas as políticas de TrustFramework da sua organização em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.AuthenticationMethod_ | Ler e gravar as políticas de método de autenticação da sua organização | Permite que o aplicativo leia e grave as políticas do método de autenticação, em nome do usuário conectado. | Sim | Não |
| _Policy.ReadWrite.MobilityManagement_ | Ler e gravar as políticas de gerenciamento de mobilidade da sua organização. | Permite ao aplicativo ler e gravar as políticas de gerenciamento de mobilidade da sua organização em nome do usuário conectado. Controlam as configurações para MDM (gerenciamento de dispositivo móvel) e aplicativos de gerenciamento de aplicativo móvel (MAM). | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:----------------------------|
| _Policy.Read.All_ | Leia as políticas da sua organização | Permite que o aplicativo leia todas as políticas da sua organização sem um usuário conectado. | Sim |
| _Policy.Read.PermissionGrant_ | Ler políticas de concessão de consentimento e permissão | Permite que o aplicativo leia políticas relacionadas a concessões de consentimento e permissão para aplicativos, sem um usuário conectado. | Sim |
| _Policy.Read.ApplicationConfiguration_ | Leia as políticas de configuração dos aplicativos da sua organização | Permite que o aplicativo leia todas as políticas de configuração dos aplicativos da sua organização sem um usuário conectado. | Sim |
| _Policy.ReadWrite.AccessReview_ | Ler e gravar a política de autorização da sua organização | Permite ao aplicativo ler e gravar a política de revisão de acesso da sua organização, sem um usuário conectado. | Sim | Não |
| _Policy.ReadWrite.ApplicationConfiguration_ | Leia e escreva as políticas de configuração dos aplicativos da sua organização | Permite que o aplicativo leia e grave as políticas de configuração dos aplicativos da sua organização, sem um usuário conectado. | Sim | Não |
| _Policy.ReadWrite.AuthenticationFlows_ | Ler e gravar as políticas de fluxo de autenticação da sua organização | Permite que o aplicativo leia e grave todas as políticas de fluxo de autenticação do locatário, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.Authorization_ | Ler e gravar a política de autorização da sua organização | Permite que o aplicativo leia e grave a política de autorização da sua organização, em nome do usuário conectado.  Por exemplo, as políticas de autorização podem controlar algumas das permissões que a função do usuário pronto tem por padrão. | Sim | Não |
| _Policy.ReadWrite.ConsentRequest_ | Ler e escrever a política de solicitações de consentimento da sua organização | Permite que o aplicativo leia e escreva a política de solicitações de consentimento da sua organização sem um usuário conectado. | Sim | Não |
| _Policy.ReadWrite.FeatureRollout_ | Políticas de distribuição de recursos de leitura e gravação | Permite que o aplicativo leia e grave todas as políticas de distribuição de recursos sem um usuário conectado. Inclui habilidades para atribuir e remover usuários e grupos para a implantação de um recurso específico. | Sim |
| _Policy.ReadWrite.PermissionGrant_ | Gerenciar as políticas de concessão de consentimento e permissão | Permite que o aplicativo gerencie as políticas relacionadas às concessões de consentimento e permissão para aplicativos, sem um usuário conectado. | Sim |
| _Policy.ReadWrite.TrustFramework_ | Ler e gravar as políticas da estrutura de confiança da sua organização | Permite que o aplicativo leia e grave todas as políticas da estrutura de confiança da sua organização sem um usuário conectado. | Sim |
| _Policy.ReadWrite.AuthenticationMethod_ | Ler e gravar as políticas de método de autenticação da sua organização | Permite que o aplicativo leia e grave as políticas do método de autenticação, sem um usuário conectado. | Sim |

### <a name="example-usage"></a>Exemplo de uso

Os seguintes usos são válidos para permissões delegadas e permissões de aplicativo:

* _Policy.Read.All_: Ler as políticas da sua organização (`GET /policies`)
* _Policy.Read.All_: Ler as políticas da estrutura de confiança da sua organização (`GET /beta/trustFramework/policies`)
* _Policy.Read.All_: Ler as políticas de distribuição de recursos da sua organização (`GET /beta/directory/featureRolloutPolicies`)
* _Policy.ReadWrite.AccessReview_: Ler e gravar as políticas de revisão de acesso da sua organização (`PATCH /beta/policies/accessReviewPolicy`)
* _Policy.ReadWrite.ApplicationConfiguration_: Leia e grave as políticas de configuração dos aplicativos da sua organização (`POST /beta/policies/tokenLifetimePolicies`)
* _Policy.ReadWrite.AuthenticationFlows_: Ler e gravar a política de fluxos de autenticação da sua organização (`PATCH /beta/policies/authenticationFlowsPolicy`)
* _Policy.ReadWrite.ConditionalAccess_: Leia e escreva as políticas de acesso condicional da sua organização (`POST /beta/identity/conditionalAccess/policies`)
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

### <a name="example-usage"></a>Exemplo de uso

* _Presence.Read_: se você estiver conectado, recupere a sua própria informação de presença (`GET /me/presence`)
* _Presence.Read.All_: Recupere as informações de presença de outro usuário (`GET /users/{id}/presence`)
* _Presence.Read.All_: Recupere as informações de presença de vários usuários (`POST /communications/getPresencesByUserId`)

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
- Para as permissões delegadas permitirem que aplicativos leiam relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir ao usuário uma função de administrador limitada do Azure AD. Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](reportroot-authorization.md).

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
| _RoleManagement.Read.All_ | Leia os dados de gerenciamento de função para todos os provedores RBAC. | Permite que o aplicativo leia as configurações de controle de acesso baseado na função (RBAC) de todos os [provedores RBAC](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true), em nome do usuário conectado. Isso inclui as definições de leitura e as atribuições de função. | Sim | Não |
| _RoleManagement.Read.Directory_ | Leia os dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de controle de acesso baseado em função (RBAC) da sua empresa, em nome do usuário conectado. Isso inclui a leitura de modelos de função de diretório, funções de diretório e associações. | Sim | Não |
| _RoleManagementPolicy.Read.Directory_ | Leia todas as políticas para tarefas de funções privilegiadas para o diretório da sua empresa. | Permite que o aplicativo leia políticas para tarefas de controle de acesso baseado em função privilegiada (RBAC) para o diretório de sua empresa, em nome do usuário conectado. | Sim | Não |
| _RoleAssignmentSchedule.ReadWrite.Directory_ | Leia, atualize e exclua todas as atribuições de funções ativas para o diretório da sua empresa. | Permite que o aplicativo leia e gerencie as atribuições ativas de controle de acesso baseado em função (RBAC) para o diretório da sua empresa, em nome do usuário conectado. Isso inclui o gerenciamento de associações de função de diretório ativo e leitura de modelos de função de diretório, funções de diretório e associações ativas. | Sim | Não |
| _RoleEligibilitySchedule.ReadWrite.Directory_ | Leia, atualize e exclua  todas as tarefas de funções elegíveis para o diretório da sua empresa. | Permite que o aplicativo leia e gerencie as tarefas de controle de acesso baseado em função (RBAC) qualificadas para o diretório da sua empresa, em nome do usuário conectado. Isso inclui o gerenciamento de associações de funções de diretório elegíveis e a leitura de modelos de funções de diretórios, funções de diretórios e associações elegíveis. | Sim | Não |
| _RoleManagement.ReadWrite.Directory_ | Ler e gravar dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de RBAC (controle de acesso baseado em função) da sua empresa, em nome do usuário conectado. Isso inclui a instanciação das funções de diretório, o gerenciamento de associação da função de diretório, a leitura dos modelos da função de diretório, as associações e as funções de diretório. | Sim | Não |
| _RoleManagementPolicy.ReadWrite.Directory_ | Leia, atualize e exclua todas as políticas para tarefas de funções privilegiadas para o diretório da sua empresa. | Permite que o aplicativo leia, atualize e exclua políticas para tarefas de controle de acesso baseado em função privilegiada (RBAC) para o diretório de sua empresa, em nome do usuário conectado. | Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _RoleManagement.Read.All_ | Leia os dados de gerenciamento de função para todos os provedores RBAC. | Permite que o aplicativo leia as configurações de controle de acesso baseado na função (RBAC) de todos os [provedores RBAC](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true), sem um usuário conectado. Isso inclui as definições de leitura e as atribuições de função. | Sim |
| _RoleManagement.Read.Directory_ | Leia os dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de RBAC (controle de acesso baseado em função) da sua empresa, em nome do usuário conectado. Isso inclui a leitura de modelos da função de diretório, as associações e as funções de diretório. | Sim |
| _RoleManagement.ReadWrite.Directory_ | Ler e gravar dados de gerenciamento de função para o Azure Active Directory. | Permite que o aplicativo leia e gerencie as configurações de controle de acesso baseado em função (RBAC) para o diretório da sua empresa, sem um usuário conectado. Isso inclui instanciar funções de diretório e gerenciamento de associação de função de diretório e leitura de modelos de função de diretório, funções de diretório e associações. | Sim |


### <a name="remarks"></a>Comentários
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
| _ExternalConnection.ReadWrite.OwnedBy_ | Leitura e gravação de conexões externas e configurações de conexão | Permite que o aplicativo faça leitura e gravação de conexões externas e suas configurações sem um usuário conectado. O aplicativo somente pode ler e gravar conexões externas às qual está autorizado ou pode criar novas conexões externas. | Sim | Não |
| _ExternalItem.ReadWrite.OwnedBy_ | Ler e gravar itens externos | Permite que o aplicativo leia e grave itens externos sem um usuário conectado. O aplicativo somente pode ler itens externos da conexão à qual está autorizado. | Sim | Não |
| _ExternalItem.ReadWrite.All_ | Leitura e gravação de todos os itens externos | Permite que o aplicativo faça leitura e gravação de todos os itens externos sem um usuário conectado. | Sim | Não |

#### <a name="delegated-permissions"></a>Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _ExternalItem.Read.All_ | Ler os dados externos | Permite que um aplicativo consulte dados ingeridos com conectores Microsoft Graph| Sim | Não |

### <a name="remarks"></a>Comentários
As permissões de pesquisa só são válidas para contas corporativas ou de estudante.

Esta permissão de pesquisa só se aplica aos dados ingeridos da API de indexação.

O acesso aos dados por meio de pesquisa requer permissão de leitura para o item. Por exemplo, _Files.Read.All_ para acessar arquivos por meio da pesquisa.

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _ExternalItem.Read.All_ _: Acessar dados externos da [API de pesquisa](/graph/api/resources/search-api-overview) (`POST /search/query`).

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
As permissões de _Tarefas_ são usadas para controlar o acesso das tarefas To Do e tarefas do Outlook(preterido). O acesso a tarefas do Microsoft Planner é controlado pelas [permissões _do_ Grupo](#group-permissions).

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
| _TeamsAppInstallation.ReadWriteSelfForUser_ (visualização privada) | Permitir que o aplicativo se gerencie nas equipes| Permite que um aplicativo do Teams se leia, se instale, se atualize e se desinstale para as equipes as quais o usuário conectado possa acessar.| Não | Não |
| _TeamsAppInstallation.ReadForTeam_ | Ler os seus aplicativos do Teams instalados nas equipes| Permite que o aplicativo leia os aplicativos do Teams instalados nas equipes que o usuário conectado pode acessar. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteForTeam_ | Gerenciar os aplicativos do Teams instalados nas equipes| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams nas equipes que o usuário conectado pode acessar. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteSelfForTeam_ (visualização privada) | Permitir que o aplicativo se gerencie nas equipes| Permite que um aplicativo do Teams se leia, se instale, se atualize e se desinstale para as equipes as quais o usuário conectado possa acessar.| Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _TeamsAppInstallation.ReadForUser.All_ | Ler os aplicativos do Teams instalados para todos os usuários| Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteForUser.All_ | Gerenciar aplicativos do Teams para todos os usuários| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteSelfForUser.All_ (visualização privada) | Permitir que o aplicativo se gerencie para todos os usuários| Permite que o aplicativo do Teams se leia, se instale, se atualize e se desinstale para qualquer usuário, sem um usuário conectado.| Sim |
| _TeamsAppInstallation.ReadForTeam.All_ | Ler os aplicativos do Teams instalados para todas as equipes| Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer equipe, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteForTeam.All_ | Gerenciar aplicativos de Teams para todas as equipes| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams em qualquer equipe, sem um usuário conectado. Não permite ler configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteSelfForTeam.All_ (visualização privada) | Permitir que o aplicativo do Teams se gerencie para todas as equipes| Permite que o aplicativo do Teams se leia, se instale, se atualize e se desinstale em qualquer equipe, sem um usuário conectado.| Sim |

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
| _TeamworkTag.ReadWrite_| Lê e grava rótulos no Microsoft Teams. | Lê e escreve os rótulos em qualquer equipe do Microsoft Teams, sem um usuário conectado.  | Sim | Não |
| _TeamworkTag.Read_ | Lê rótulos no Microsoft Teams. | Lê os rótulos em qualquer equipe do Microsoft Teams, sem um usuário conectado. | Sim | Não |

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

Para que um aplicativo leia ou grave todos os acordos ou aceitações de acordos com permissões delegadas, o usuário conectado deve ter a função Administrador Global, Administrador de Acesso Condicional ou Administrador de Segurança. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado
Os seguintes usos são válidos para permissões delegadas:

* _Agreement.Read.All_: ler todos os acordos de termos de uso (`GET /beta/agreements`)
* _Agreement.ReadWrite.All_: ler e gravar todos os acordos de termos de uso (`POST /beta/agreements`)
* _AgreementAcceptance.Read_: ler os status de aceitação de termos de uso do usuário (`GET /beta/me/agreementAcceptances`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

## <a name="teams-app-installation-permissions-private-preview"></a>Permissões de aplicativos do Teams([visualização privada](#permissions-availability-status))

#### <a name="delegated-permissions"></a>Permissões delegadas
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsAppInstallation.ReadForUser_ (visualização privada) | Ler os aplicativos do Teams instalados do usuário| Permite que o aplicativo leia os aplicativos do Teams instalados para o usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteForUser_ (visualização privada) | Gerenciar os aplicativos do Teams instalados do usuário| Permite que o aplicativo leia instale, atualize e desinstale os aplicativos do Teams instalados para o usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Não | Não |
| _TeamsAppInstallation.ReadWriteSelfForUser_ (visualização privada) | Permitir que o aplicativo se gerencie nas equipes| Permite que um aplicativo do Teams se leia, se instale, se atualize e se desinstale para as equipes as quais o usuário conectado possa acessar.| Sim | Não |
| _TeamsAppInstallation.ReadForTeam_ (visualização privada) | Ler os seus aplicativos do Teams instalados nas equipes| Permite que o aplicativo leia os aplicativos do Teams instalados nas equipes que o usuário conectado pode acessar. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteForTeam_ (visualização privada) | Gerenciar os aplicativos do Teams instalados nas equipes| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams nas equipes que o usuário conectado pode acessar. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim | Não |
| _TeamsAppInstallation.ReadWriteSelfForTeam_ (visualização privada) | Permitir que o aplicativo se gerencie nas equipes| Permite que um aplicativo do Teams se leia, se instale, se atualize e se desinstale para as equipes as quais o usuário conectado possa acessar.| Sim | Não |

#### <a name="application-permissions"></a>Permissões de aplicativos
|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:----------------|:------------------|:-------------|:-----------------------|
| _TeamsAppInstallation.ReadForUser.All_ (visualização privada) | Ler os aplicativos do Teams instalados para todos os usuários| Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteForUser.All_ (visualização privada) | Gerenciar aplicativos do Teams para todos os usuários| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams para qualquer usuário, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteSelfForUser.All_ (visualização privada) | Permitir que o aplicativo se gerencie para todos os usuários| Permite que o aplicativo do Teams se leia, se instale, se atualize e se desinstale para qualquer usuário, sem um usuário conectado.| Sim |
| _TeamsAppInstallation.ReadForTeam.All_ (visualização privada) | Ler os aplicativos do Teams instalados para todas as equipes| Permite que o aplicativo leia os aplicativos do Teams instalados para qualquer equipe, sem um usuário conectado. Não dá a capacidade de ler as configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteForTeam.All_ (visualização privada) | Gerenciar aplicativos de Teams para todas as equipes| Permite que o aplicativo leia, instale, atualize e desinstale aplicativos do Teams em qualquer equipe, sem um usuário conectado. Não permite ler configurações específicas do aplicativo.| Sim |
| _TeamsAppInstallation.ReadWriteSelfForTeam.All_ (visualização privada) | Permitir que o aplicativo do Teams se gerencie para todas as equipes| Permite que o aplicativo do Teams se leia, se instale, se atualize e se desinstale em qualquer equipe, sem um usuário conectado.| Sim |

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

Com a permissão _User.ReadWrite.All_ delegada ou de aplicativo, a atualização de **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não são administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios. Para obter mais detalhes, confira Administrador de suporte técnico (senha) nas [funções disponíveis do Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

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
* _UserActivity.ReadWrite.CreatedByApp_: obter uma lista de atividades de usuários recentes únicos com base nos itens de histórico associados publicados no último dia. (GET /me/activities/recent).
* _UserActivity.ReadWrite.CreatedByApp_: publicar ou atualizar uma atividade do usuário que poderá ser retomada pelo usuário do aplicativo. (PUT /me/activities/%2Farticle%3F12345).
*   _UserActivity.ReadWrite.CreatedByApp_: publicar ou atualizar um item de histórico de uma atividade de usuário especificada para representar o período de engajamento do usuário. (PUT /me/activities/{id}/historyItems/{id}).
*   _UserActivity.ReadWrite.CreatedByApp_: excluir uma atividade de usuário em resposta a uma solicitação iniciada pelo usuário ou para remover dados inválidos. (DELETE /me/activities/{id}).
*   _UserActivity.ReadWrite.CreatedByApp_: excluir um item de histórico em resposta a uma solicitação iniciada pelo usuário ou para remover dados inválidos. (DELETE /me/activities/{id}/historyItems/{id}).

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

Para que um aplicativo leia ou grave todas as configurações de implantação de atualização do Windows com permissões delegadas, o usuário conectado deve ser atribuído à função de Administrador Global ou Administrador do Intune. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).

### <a name="example-usage"></a>Exemplo de uso

#### <a name="delegated"></a>Delegado

* _WindowsUpdates.ReadWrite.All_: crie uma implantação (`POST /beta/admin/windows/updates/deployments`).

#### <a name="application"></a>Aplicativo

* _WindowsUpdates.ReadWrite.All_: crie uma implantação (`POST /beta/admin/windows/updates/deployments`).

## <a name="authentication-methods-policy-permissions-preview"></a>Permissões de política de métodos de autenticação ([visualização](#permissions-availability-status))

#### <a name="delegated-permissions"></a>Permissões delegadas

|Permissão                              |Exibir Cadeia de Caracteres                        |Descrição        |Consentimento Obrigatório do Administrador | Suporte da conta da Microsoft |
|:---------------------------------------|:-------------------------------------|:------------------|:----------------------|:----------------------------|
|_Policy.ReadWrite.AuthenticationMethod_ (visualização)        |Leia e escreva todas as políticas de métodos de autenticação.       |Permite que o aplicativo leia e grave todas as políticas de métodos de autenticação em um locatário do Microsoft Azure Active Directory. Além disso, o usuário conectado deve ter a função de Administrador Global atribuída. |Sim|Não|

#### <a name="application-permissions"></a>Permissões de aplicativos

|Permissão                              |Exibir Cadeia de Caracteres                        |Descrição        |Consentimento Obrigatório do Administrador |
|:---------------------------------------|:-------------------------------------|:------------------|:----------------------|
|_Policy.ReadWrite.AuthenticationMethod_ (visualização privada)   |Leia e escreva todas as políticas de métodos de autenticação.    |Permite que o aplicativo leia e grave todas as políticas de métodos de autenticação em um locatário do Microsoft Azure Active Directory. |Sim|


### <a name="remarks"></a>Comentários

As permissões de política de métodos de autenticação são usadas para gerenciar configurações na política de métodos de autenticação, incluindo habilitar e desabilitar métodos de autenticação, permitir que usuários e grupos usem esses métodos e definir outras configurações relacionadas aos métodos de autenticação que os usuários podem registrar e usar em um locatário.

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
