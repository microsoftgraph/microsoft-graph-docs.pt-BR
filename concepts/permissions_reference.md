<a id="microsoft-graph-permissions-reference" class="xliff"></a>

# Referência de permissões do Microsoft Graph 
O Microsoft Graph expõe as permissões granulares que controlam o acesso que os aplicativos têm aos recursos, como email, grupos e usuários. Como desenvolvedor, você decide quais permissões para o Microsoft Graph seu aplicativo deverá solicitar. Quando um usuário entra no aplicativo, ele, ou, em alguns casos, um administrador, tem a opção de consentir essas permissões. Se o usuário consentir, seu aplicativo receberá acesso aos recursos e APIs que solicitados. Para aplicativos que não aceitam usuários conectados, as permissões podem ser previamente consentidas pelo administrador quando o aplicativo é instalado ou durante a inscrição. 

<a id="delegated-permissions-application-permissions-and-effective-permissions" class="xliff"></a>

## Permissões delegadas, Permissões de aplicativo e permissões efetivas
O Microsoft Graph tem dois tipos de permissões: **Permissões Delegadas** e **Permissões de aplicativo**. 

- As **Permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente. Para esses aplicativos, o usuário ou um administrador concorda com as permissões que o aplicativo solicita e o aplicativo tem permissão delegada para agir como o usuário conectado ao fazer chamadas para o Microsoft Graph. Algumas Permissões Delegadas podem ser autorizadas por usuários não administrativos, mas algumas permissões com privilégios mais altos exigem o consentimento do administrador.  

- As **Permissões de aplicativo** são usadas pelos aplicativos que são executados sem um usuário conectado. Por exemplo, aplicativos executados como daemons ou serviços em segundo plano.  As Permissões de aplicativo só podem ser autorizadas por um administrador. 

As _permissões efetivas_ são as permissões que seu aplicativo terá ao fazer solicitações ao Microsoft Graph. É importante compreender a diferença entre as Permissões Delegadas e as Permissões de aplicativo que o aplicativo tem autorização para usar e as respectivas Permissões Efetivas ao fazer chamadas para o Microsoft Graph

- No caso de Permissões Delegadas, as _Permissões Efetivas_ do aplicativo estarão na interseção menos privilegiada das Permissões Delegadas que o aplicativo recebeu (por meio de consentimento) e dos privilégios do usuário atualmente conectado. O aplicativo jamais pode ter mais privilégios do que o usuário conectado. Nas organizações, os privilégios do usuário conectado podem ser determinados por uma política ou pela associação a uma ou mais funções de administrador. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles).<br/><br/>Por exemplo, digamos que o aplicativo recebeu a Permissão Delegada _User.ReadWrite.All_. Essa permissão autoriza o aplicativo a ler e atualizar o perfil de todos os usuários em uma organização. Se o usuário conectado for um administrador global, seu aplicativo conseguirá atualizar o perfil de todos os usuários na organização. No entanto, se o usuário conectado não tiver uma função de administrador, seu aplicativo conseguirá atualizar apenas o perfil do usuário conectado. Ele não conseguirá atualizar os perfis de outros usuários na organização porque o usuário que tem permissão para agir em nome de outra pessoa não tem esses privilégios.
  
- No caso de Permissões de aplicativo, as _Permissões Efetivas_ do aplicativo estarão no nível completo de privilégios implícitos da permissão. Por exemplo, um aplicativo que tem a Permissão de aplicativo _User.ReadWrite.All_ pode atualizar o perfil de todos os usuários na organização. 

<a id="microsoft-graph-permission-names" class="xliff"></a>

### Nomes de permissões do Microsoft Graph
Os nomes de permissões do Microsoft Graph seguem um padrão simples: _resource.operation.constraint_. Por exemplo, _User.Read_ concede permissão para ler o perfil do usuário conectado, _User.ReadWrite_ concede permissão para ler e modificar o perfil do usuário conectado e _Mail.Send_ concede permissão para enviar emails em nome do usuário conectado. 

O elemento _constraint_ do nome determina a extensão potencial do acesso que o aplicativo terá dentro do diretório. No momento, o Microsoft Graph é compatível com as seguintes restrições: 

* **Todos** concede permissão para o aplicativo realizar as operações em todos os recursos do tipo especificado em um diretório. Por exemplo, _User.Read.All_ potencialmente concede privilégios ao aplicativo para ler os perfis de todos os usuários em um diretório. 
* **Compartilhado** concede permissão para o aplicativo realizar as operações em recursos que outros usuários compartilharam com o usuário conectado. Essa restrição é usada principalmente com recursos como emails, calendários e contatos do Outlook. Por exemplo, _Mail.Read.Shared_ concede privilégios para ler email na caixa de correio do usuário conectado e emails em caixas de correio que outros usuários na organização compartilharam com o usuário conectado.
* **AppFolder** concede permissão para o aplicativo ler e gravar arquivos em uma pasta dedicada no OneDrive. Essa restrição é exposta somente em [Permissões de arquivos](#files-permissions) e só é válida para contas da Microsoft.
* Se **sem restrição** estiver especificado, o aplicativo estará limitado a executar as operações nos recursos pertencentes ao usuário conectado. Por exemplo, _User.Read_ concede privilégios para ler o perfil apenas do usuário conectado e _Mail.Read_ concede permissão para ler apenas os emails na caixa de correio do usuário conectado.

> **Observação**: Em cenários delegados, as permissões efetivas concedidas ao aplicativo podem ser limitadas pelos privilégios do usuário conectado na organização.
> 

<a id="microsoft-accounts-and-work-or-school-accounts" class="xliff"></a>

### Contas da Microsoft e contas corporativas e de estudante

Nem todas as permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante. Você pode escolher **Comentários** para cada grupo de permissão para determinar se uma permissão específica é válida para contas da Microsoft, contas corporativas ou de estudante ou ambas. 

<a id="user-and-group-search-limitations-for-guest-users-in-organizations" class="xliff"></a>

### Limitações de pesquisa de usuário e grupo para usuários convidados em organizações

Os recursos de pesquisa de usuário e grupo permitem que o aplicativo pesquise usuários ou grupos em um diretório da organização executando consultas no conjunto de recursos `/users` ou `/groups` (por exemplo, `https://graph.microsoft.com/v1.0/users`). Os administradores e os usuários têm esse recurso. No entanto, os usuários convidados não. Se o usuário conectado for um usuário convidado, dependendo das permissões que recebeu um aplicativo, ele pode ler o perfil de um usuário específico ou grupo (por exemplo, `https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`). No entanto, o usuário não pode executar consultas no conjunto de recursos `/users` ou `/groups` que, potencialmente, retornam mais de um recurso. Com as permissões apropriadas, o aplicativo pode ler os perfis de usuários ou grupos que ele obtém seguindo os links nas propriedades de navegação. Por exemplo, `/users/{id}/directReports` ou `/groups/{id}/members`.

---

<a id="calendars-permissions" class="xliff"></a>

## Permissões de calendários

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    Ler calendários do usuário  | Permite ao aplicativo ler eventos nos calendários do usuário.| Não |
| _Calendars.Read.Shared_ |    Ler usuários e calendários compartilhados | Permite que o aplicativo leia os eventos em todos os calendários a que o usuário tem acesso, incluindo os delegados e os calendários compartilhados. | Não |
| _Calendars.ReadWrite_ |    Ter acesso total aos calendários do usuário  | Permite ao aplicativo criar, ler, atualizar e excluir eventos em calendários do usuário. | Não |
| _Calendars.ReadWrite.Shared_ |    Ler e registrar usuário e calendários compartilhados | Permite ao aplicativo criar, ler, atualizar e excluir eventos de todos os calendários que o usuário tenha permissão para acessar. Isso inclui o delegado e os calendários compartilhados.| Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    Ler calendários em todas as caixas de correio  | Permite ao aplicativo ler eventos de todos os calendários sem um usuário conectado.| Sim |
| _Calendars.ReadWrite_ |    Ler e gravar calendários em todas as caixas de correio | Permite ao aplicativo criar, ler, atualizar e excluir eventos de todos os calendários sem um usuário conectado.| Sim |

<a id="remarks" class="xliff"></a>

### Comentários

_Calendars.Read.Shared_ e _Calendars.ReadWrite.Shared_ só são válidos para contas corporativas ou de estudante. Todas as demais permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso

<a id="delegated" class="xliff"></a>

#### Delegado

* _Calendars.Read_: Obter eventos do calendário do usuário entre 23 de abril de 2017 e 29 de abril de 2017 (`GET /me/calendarView?startDateTime=2017-04-23T00:00:00&endDateTime=2017-04-29T00:00:00`).
* _Calendars.Read.Shared_: Encontrar horários de reuniões onde todos os participantes estejam disponíveis (`POST /users/{id|userPrincipalName}/findMeetingTimes`).
* _Calendars.ReadWrite_: Adicionar um evento ao calendário do usuário (`POST /me/events`).

<a id="application" class="xliff"></a>

#### Aplicativo

* _Calendars.Read_: Localizar eventos do calendário de uma sala de conferências organizado por pedro@contoso.com (`GET /users/{id | userPrincipalName}/events?$filter=organizer/emailAddress/address eq 'bob@contoso.com'`).
* _Calendars.Read_: Listar todos os eventos do mês de maio do calendário de um usuário (`GET /users/{id | userPrincipalName}/calendarView?startDateTime=2017-05-01T00:00:00&endDateTime=2017-06-01T00:00:00`)
* _Calendars.ReadWrite_: Adicionar um evento de folga aprovada (`POST /users/{id | userPrincipalName}/events`) ao calendário de um usuário.
* _Calendars.Send_: Enviar uma mensagem (`POST /users/{id | userPrincipalName}/sendCalendars`).


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="contacts-permissions" class="xliff"></a>

## Permissões de contatos

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    Ler contatos do usuário  | Permite ao aplicativo ler os contatos do usuário. | Não |
| _Contacts.Read.Shared_ |    Ler usuário e contatos compartilhados | Permite que o aplicativo leia os contatos que o usuário tem permissão de acessar, incluindo os próprios contatos do usuário e os contatos compartilhados. | Não |
| _Contacts.ReadWrite_ |    Ter acesso total aos contatos do usuário  | Permite ao aplicativo criar, ler, atualizar e excluir contatos do usuário. | Não |
| _Contacts.ReadWrite.Shared_ |    Ler e registrar usuário e contatos compartilhados | Permite que o aplicativo crie, leia, atualize e exclua os contatos para os quais o usuário tem permissão, incluindo os próprios contatos do usuário e os contatos compartilhados.| Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    Ler contatos em todas as caixas de correio | Permite ao aplicativo ler todos os contatos em todas as caixas de correio sem um usuário conectado. | Sim |
| _Contacts.ReadWrite_ |    Ler e gravar contatos em todas as caixas de correio  |Permite ao aplicativo criar, ler, atualizar e excluir todos os contatos em todas as caixas de correio sem um usuário conectado.| Sim |

<a id="remarks" class="xliff"></a>

### Comentários
Apenas as Permissões Delegadas _Contacts.Read_ e _Contacts.ReadWrite_ são válidas para contas da Microsoft. 

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _Contacts.Read_: Ler um contato a partir de uma das pastas de contatos de nível superior do usuário conectado (`GET /me/contactfolders/{Id}/contacts/{id}`).
* _Contacts.ReadWrite_: Atualizar a foto de contato de um dos contatos do usuário conectado (`PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`). 
* _Contacts.ReadWrite_: Adicionar contatos à pasta raiz do usuário conectado (`POST /me/contacts`).

<a id="application" class="xliff"></a>

#### Aplicativo

* _Contacts.Read_: Ler contatos a parir de uma das pastas de contatos de nível superior de qualquer usuário da organização (`GET /users/{id | userPrincipalName}/contactfolders/{Id}/contacts/{id}`). 
* _Contacts.ReadWrite_: Atualizar a foto de qualquer contato de qualquer usuário em uma organização (`PUT /user/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`). 
* _Contacts.ReadWrite_: Adicionar contatos à pasta raiz de qualquer usuário da organização (`POST /users/{id | userPrincipalName}/contacts`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="device-permissions" class="xliff"></a>

## Permissões de dispositivos

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.Read_ | Ler os dispositivos do usuário | Permite ao aplicativo ler a lista de dispositivos do usuário em nome do usuário conectado. | Não |
| _Device.Command_ | Comunicar-se com os dispositivos do usuário | Permite ao aplicativo se comunicar ou inicializar outro aplicativo no dispositivo do usuário em nome do usuário conectado. | Não |


<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.ReadWrite.All_ | Ler e registrar dispositivos | Permite que o aplicativo leia e registre todos as propriedades dos dispositivos sem um usuário conectado. Não permite a criação de dispositivos, exclusão de dispositivos ou atualização de identificadores de segurança de dispositivo alternativo. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários

As Permissões Delegadas _Device.Read_ e _Device.Command_ são válidas apenas para contas pessoais da Microsoft.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="application" class="xliff"></a>

#### Aplicativo

* _Device.ReadWrite.All_: Ler todos os dispositivos registrados na organização (`GET /devices`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="microsoft-intune-device-management-permissions" class="xliff"></a>

## Permissões de Gerenciamento de Dispositivos do Microsoft Intune

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

Nenhum

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _DeviceManagementServiceConfiguration.Read.All_ | Configuração de leitura Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades do serviço do Microsoft Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. | Sim |
| _DeviceManagementServiceConfiguration.ReadWrite.All_ | Ler e registrar o Microsoft Intune (visualização) | Permite que o aplicativo leia e registre propriedades do serviço do Microsoft Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. | Sim |
| _DeviceManagementConfiguration.Read.All_ | Ler a configuração de dispositivo e as políticas do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades configuração de dispositivo e das políticas de conformidade do Microsoft gerenciado Intune e sua atribuição aos grupos.  | Sim |
| _DeviceManagementConfiguration.ReadWrite.All_ | Ler e escrever as configurações de dispositivo e as políticas do Microsoft Intune (visualização) | Permite que o aplicativo leia e registre as propriedades de configuração de dispositivo e as políticas de conformidade de dispositivo do Microsoft Intune e sua atribuição aos grupos. | Sim |
| _DeviceManagementApps.Read.All_ | Ler aplicativos do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades, as atribuições de grupo, o status de aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. | Sim |
| _DeviceManagementApps.ReadWrite.All_ | Ler e registrar os aplicativos do Microsoft Intune (visualização) | Permite que aplicativo leia e registre s propriedades, as atribuições de grupo, o status dos aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. | Sim |
| _DeviceManagementRBAC.Read.All_ | Ler as configurações RBAC (Controle de Acesso com Base em Função) do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades relacionadas às configurações RBAC do Microsoft Intune. | Sim |
| _DeviceManagementRBAC.ReadWrite.All_ | Ler e registrar as configurações RBAC do Microsoft Intune (visualização) | Permite que o aplicativo leia e registre as propriedades relacionadas às configurações RBAC do Microsoft Intune. | Sim |
| _DeviceManagementManagedDevices.Read.All_ | Ler dispositivos do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades de dispositivos gerenciados pelo Microsoft Intune. | Sim |
| _DeviceManagementManagedDevices.ReadWrite.All_ | Ler e registrar dispositivos do Microsoft Intune (visualização) | Permite que o aplicativo leia e registre as propriedades de dispositivos gerenciados pelo Microsoft Intune. Não permite operações de alto impacto como apagamento remoto e a redefinição de senha no proprietário do dispositivo. | Sim |
| _DeviceManagementManagedDevices.PrivilegedOperations.All_ | Executar ações remotas de impacto no usuário nos dispositivos do Microsoft Intune (visualização) | Permite que o aplicativo execute ações remotas de alto impacto como apagar dispositivo ou redefinir a senha em dispositivos gerenciados pelo Microsoft Intune. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários
> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Essas permissões só são válidas para contas corporativas ou de estudante.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="application" class="xliff"></a>

#### Aplicativo

* _DeviceManagementServiceConfiguration.Read.All_: Verificar o estado atual da assinatura do Intune (`GET /deviceManagement/subscriptionState`)
* _DeviceManagementServiceConfiguration.ReadWrite.All_: Criar novos Termos e Condições (`POST /deviceManagement/termsAndConditions`)
* _DeviceManagementConfiguration.Read.All_: Localizar o status da configuração de um dispositivo (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`)
* _DeviceManagementConfiguration.ReadWrite.All_: Atribuir uma política de conformidade do dispositivo para um grupo (`POST deviceCompliancePolicies/{id}/assign`)
* _DeviceManagementApps.Read.All_: Localizar todos os aplicativos da Windows Store publicados no Intune (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`)
* _DeviceManagementApps.ReadWrite.All_: Publicar um novo aplicativo (`POST /deviceAppManagement/mobileApps`)
* _DeviceManagementRBAC.Read.All_: Localizar uma atribuição de função pelo nome (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`)
* _DeviceManagementRBAC.ReadWrite.All_: Criar uma nova função personalizada (`POST /deviceManagement/roleDefinitions`)
* _DeviceManagementManagedDevices.Read.All_: Localizar um dispositivo gerenciado pelo nome (`GET /managedDevices/?$filter=deviceName eq 'My Device'`)
* _DeviceManagementManagedDevices.ReadWrite.All_: Remover um dispositivo gerenciado (`DELETE /managedDevices/{id}`)
* _DeviceManagementManagedDevices.PrivilegedOperations.All_: Redefinir a senha em um dispositivo gerenciado do usuário (`POST /managedDevices/{id}/resetPasscode`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="directory-permissions" class="xliff"></a>

## Permissões do diretório

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_           |     Ler dados do diretório                     | Permite ao aplicativo ler dados no diretório da sua organização, como usuários, grupos e aplicativos. | Sim |
| _Directory.ReadWrite.All_      |     Ler e gravar dados de diretório           | Permite ao aplicativo ler e gravar dados no diretório da sua organização, como usuários e grupos.  Não permite ao aplicativo excluir usuários ou grupos, ou redefinir senhas de usuário. | Sim |
| _Directory.AccessAsUser.All_   |     Access Directory como o usuário conectado  | Permite ao aplicativo ter o mesmo acesso que o usuário conectado a informações no diretório.| Sim |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_ | Ler dados do diretório | Permite ao aplicativo ler dados no diretório da sua organização, como usuários, grupos e aplicativos, sem um usuário conectado. | Sim |
| _Directory.ReadWrite.All_ | Ler e gravar dados de diretório | Permite ao aplicativo ler e registrar dados no diretório de sua organização, como usuários e grupos, sem um usuário conectado. Não permite a exclusão de usuários ou grupos. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários
As permissões de diretório não são compatíveis com contas da Microsoft. 

 As permissões de diretório fornecem o nível mais alto de privilégio para acessar recursos de diretório, como [Usuário](../api-reference/v1.0/resources/user.md), [Grupo](../api-reference/v1.0/resources/group.md) e [Dispositivo](../api-reference/v1.0/resources/device.md) em uma organização. Elas também controlam exclusivamente o acesso a outros recursos de diretório como: [contatos organizacionais](../api-reference/beta/resources/orgcontact.md), [APIs de extensão de esquema](../api-reference/beta/resources/schemaextension.md), [APIs de PIM (Privileged Identity Management)](../api-reference/beta/resources/privilegedidentitymanagement_root.md) e muitos dos recursos e APIs listados no nó **Azure Active Directory** na documentação de referência da API beta e v1.0. Isso inclui unidades administrativas, funções de diretório, configurações de diretório, política e muito mais. 

A permissão _Directory.ReadWrite.All_ concede os seguintes privilégios:

- Leitura completa de todos os recursos de diretório (propriedades declaradas e propriedades de navegação)
- Criar e atualizar usuários
- Desabilitar e habilitar usuários (mas não o administrador da empresa)
- Definir a id de segurança alternativa do usuário (mas não administradores)
- Criar e atualizar grupos
- Gerenciar associações do grupo
- Atualizar o proprietário do grupo
- Gerenciar as atribuições de licença
- Definir as extensões de esquema em aplicativos
- **Observação**: Não há direitos para redefinir senhas de usuários
- **Observação**: Não há direitos para excluir recursos (incluindo usuários ou grupos)
- **Observação**: Exclui especificamente a criação ou a atualização de recursos que não estão listados acima. Isso inclui: application, oAauth2Permissiongrant, appRoleAssignment, device, servicePrincipal, organization, domains e assim por diante.
 

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado
* _Directory.Read.All_: Listar todas as unidades administrativas em uma organização (`GET /beta/administrativeUnits`)
* _Directory.ReadWrite.All_: Adicionar membros a uma função de diretório (`POST /directoryRoles/{id}/members/$ref`)

<a id="application" class="xliff"></a>

#### Aplicativo
* _Directory.Read.All_: Listar todas as associações de um usuário, incluindo funções de diretório e unidades administrativas (`GET /beta/users/{id}/memberOf`)
* _Directory.Read.All_: Listar todos os membros do grupo, incluindo as entidades de serviço (`GET /beta/groups/{id}/members`)
* _Directory.ReadWrite.All_: Adicionar um proprietário a um grupo (`POST /groups/{id}/owners/$ref`)


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="files-permissions" class="xliff"></a>

## Permissões de arquivos

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Files.Read_ |    Ler arquivos do usuário | Permite que o aplicativo leia todos os arquivos do usuário conectado.| Não |
| _Files.Read.All_ | Ler todos os arquivos que o usuário pode acessar | Permite que o aplicativo para leia todos os arquivos que o usuário conectado pode acessar. | Não |
| _Files.ReadWrite_ |   Ter acesso total aos arquivos do usuário | Permite que o aplicativo leia, crie, atualize e exclua os arquivos do usuário conectado. | Não |
| _Files.ReadWrite.All_ | Ter acesso total a todos os arquivos que o usuário pode acessar | Permite que o aplicativo leia, crie, atualize e exclua todos os arquivos que o usuário conectado pode acessar. | Não |
| _Files.ReadWrite.AppFolder_ | Ter acesso total à pasta do aplicativo (prévia) | (Prévia) Permite que o aplicativo leia, crie, atualize exclua arquivos na pasta do aplicativo. | Não |
| _Files.Read.Selected_ |    Ler arquivos selecionados pelo usuário (visualização) | **Suporte limitado no Microsoft Graph – confira Comentários** <br/> (Visualização) Permite ao aplicativo ler arquivos selecionados pelo usuário. O aplicativo tem acesso por várias horas depois que o usuário tiver selecionado um arquivo. | Não |
| _Files.ReadWrite.Selected_ |    Ler e gravar arquivos selecionados pelo usuário (visualização) | **Suporte limitado no Microsoft Graph – confira Comentários** <br/> (Visualização) Permite ao aplicativo ler e gravar arquivos selecionados pelo usuário. O aplicativo tem acesso por várias horas depois que o usuário tiver selecionado um arquivo. | Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Files.Read.All_ | Ler arquivos em todos os conjuntos de sites (prévia) | (Prévia) Permite que o aplicativo leia todos os arquivos em todos os conjuntos de sites sem que um usuário esteja conectado. | Sim |
| _Files.ReadWrite.All_ | Ler e gravar arquivos em todos os conjuntos de sites (prévia) | **Suporte limitado no Microsoft Graph** <br/> (Prévia) Permite que o aplicativo leia, crie, atualize e exclua todos os arquivos em todos os conjuntos de sites sem que um usuário esteja conectado. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários

As permissões delegadas Files.Read, Files.ReadWrite, Files.Read.All e Files.ReadWrite.All são válidas nas contas pessoais, corporativas ou de estudante da Microsoft. Observe que nas contas pessoais,Files.Read e Files.ReadWrite também concedem acesso a arquivos compartilhados com o usuário conectado. 

As permissões delegadas Files.Read.Selected e Files.ReadWrite.Selected são válidas apenas em contas corporativas ou de estudante e são expostas apenas para trabalhar com [manipuladores (v1.0) de arquivos do Office 365](https://msdn.microsoft.com/office/office365/howto/using-cross-suite-apps). Elas não devem ser usadas para chamar diretamente as APIs do Microsoft Graph. 

A permissão delegada Files.ReadWrite.AppFolder só é válida para contas pessoais e é usada para acessar a [pasta especial da Raiz de Aplicativo](https://dev.onedrive.com/items/special_folders.htm) com a API do Microsoft Graph [Obter pasta especial](../api-reference/v1.0/api/drive_special.md) do OneDrive.

A permissão de aplicativo Files.ReadWrite.All ainda não oferece suporte à API do Microsoft Graph [Criar sessão de carregamento retornável](../api-reference/v1.0/api/item_createuploadsession.md) do OneDrive. Suporte completo em breve. 

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _Files.Read_: Ler arquivos armazenados no OneDrive do usuário conectado (`GET /me/drive/root/children`)
* _Files.Read.All_: Ler arquivos compartilhados com o usuário conectado (`GET /me/drive/root/sharedWithMe`)
* _Files.ReadWrite_: Gravar um arquivo no OneDrive do usuário conectado (`PUT /me/drive/root/children/filename.txt/content`)
* _Files.ReadWrite.All_: Gravar um arquivo compartilhado com o usuário (`PUT /users/rgregg@contoso.com/drive/root/children/file.txt/content`)
* _Files.ReadWrite.AppFolder_: Gravar arquivos na pasta do aplicativo do OneDrive (`PUT /me/drive/special/approot/children/file.txt/content`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="group-permissions" class="xliff"></a>

## Permissões de grupo

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ |    Ler todos os grupos | Permite ao aplicativo listar grupos, e ler suas propriedades e todas as associações do grupo em nome do usuário conectado.  Também permite ao aplicativo ler calendário, conversas, arquivos e outros tipos de conteúdo de todos os grupos que o usuário conectado pode acessar. | Sim |
| _Group.ReadWrite.All_ |    Ler e gravar todos os grupos| Permite ao aplicativo criar grupos e ler todas as propriedades e associações do grupo em nome do usuário conectado.  Além disso, permite aos proprietários do grupo gerenciar seus grupos, e permite aos membros do grupo atualizar o conteúdo do grupo. | Sim |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ | Ler todos os grupos | Permite ao aplicativo ler os associados de todos os grupos sem um usuário conectado. Observe que nem todas as API de grupo suportam o acesso usando permissões somente de aplicativo. Consulte [problemas conhecidos](../concepts/known_issues.md) para obter exemplos. | Sim |
| _Group.ReadWrite.All_ | Ler e gravar todos os grupos | Permite que o aplicativo crie grupos, leia e atualize as associações do grupo e exclua grupos. Todas essas operações podem ser executadas pelo aplicativo sem um usuário conectado. Observe que nem todas as API de grupo suportam o acesso usando permissões somente de aplicativo. Consulte [problemas conhecidos](../concepts/known_issues.md) para obter exemplos.| Sim |


<a id="remarks" class="xliff"></a>

### Comentários

A funcionalidade de grupo não é compatível com contas da Microsoft. 

Para grupos do Office 365, as Permissões de grupo concedem ao aplicativo acesso ao conteúdo do grupo. Por exemplo, conversas, arquivos, anotações e assim por diante. As Permissões de grupo também são usadas para controlar o acesso a APIs e recursos do [Microsoft Planner](../api-reference/beta/resources/planner_overview.md).

No caso de Permissões de aplicativo, há algumas limitações para APIs com suporte. Para obter mais informações, confira os [problemas conhecidos](../concepts/known_issues.md).

Em alguns casos, um aplicativo pode precisar de [Permissões de diretório](#directory-permissions) para ler algumas propriedades do grupo como `member` e `memberOf`. Por exemplo, se um grupo tiver um ou mais [servicePrincipals](../api-reference/beta/resources/serviceprincipal.md) como membros, o aplicativo precisará de permissões eficazes para ler as entidades de serviço através do recebimento de uma das _Permissões de diretório\*_, caso contrário, o Microsoft Graph retornará um erro. No caso de Permissões Delegadas, o usuário conectado deve ter privilégios suficientes na organização para ler as entidades de serviço. A mesma orientação se aplica à propriedade `memberOf` que pode retornar [administrativeUnits](../api-reference/beta/resources/administrativeunit.md).

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _Group.Read.All_: Ler todos os grupos do Office 365 dos quais o usuário conectado é membro (`GET /me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`).
* _Group.Read.All_: Ler todo o conteúdo do grupo do Office 365, como conversas (`GET /groups/{id}/conversations`).
* _Group.ReadWrite.All_: Atualizar propriedades do grupo, como fotografias (`PUT /groups/{id}/photo/$value`).
* _Group.ReadWrite.All_: Atualizar membros do grupo (`POST /groups/{id}/members/$ref`). OBSERVAÇÃO: Isso também requer o _User.ReadBasic.All_ para ler o usuário para adicionar como membro.

<a id="application" class="xliff"></a>

#### Aplicativo

* _Group.Read.All_: Localizar todos os grupos com nomes que começam com “Vendas” (`GET /groups?$filter=startswith(displayName,'Sales')`).
* _Group.ReadWrite.All_: O serviço daemon cria novos eventos no calendário de um grupo do Office 365 (`POST /groups/{id}/events`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="identity-risk-event-permissions" class="xliff"></a>

## Permissões de Eventos de Risco de Identidade

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade  | Permite que o aplicativo para leia as informações de evento de risco de identidade para todos os usuários em sua organização em nome do usuário conectado. | Sim |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade | Permite que o aplicativo leia as informações do evento de risco de identidade para todos os usuários em sua organização sem um usuário conectado. | Sim |


<a id="remarks" class="xliff"></a>

### Comentários

_IdentityRiskEvent.Read.All_ é válido apenas para contas corporativas ou de estudante. No caso de um aplicativo com permissões delegadas para ler as informações de risco de identidade, o usuário conectado deve ser um membro de uma das seguintes funções de administrador: Administrador Global, Administrador de Segurança ou funções do Leitor de Segurança. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles).

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated-and-application" class="xliff"></a>

#### Permissões delegadas e de aplicativo
Os seguintes usos são válidos para Permissões Delegadas e Permissões de aplicativo:

* Ler todos os eventos de risco gerados para todos os usuários do locatário (`GET /beta/identityRiskEvents`)
* Ler todos os eventos de risco de malware gerados pelo botnet Dorknet (`GET /beta/malwareRiskEvents?$filter=malwareName eq 'Dorkbot'`)
* Ler os mais recentes 50 eventos de risco (`GET /beta/identityRiskEvents?$orderBy=riskEventDateTime desc&top=50`)
 
Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="mail-permissions" class="xliff"></a>

## Permissões de email

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_ |    Ler emails do usuário | Permite ao aplicativo ler emails em caixas de correio do usuário. | Não |
| _Mail.ReadWrite_ |    Acesso de leitura e gravação aos emails do usuário | Permite ao aplicativo criar, ler, atualizar e excluir emails em caixas de correio do usuário. Não inclui a permissão para enviar emails.| Não |
| _Mail.Read.Shared_ |    Ler email compartilhado e de usuário | Permite que o aplicativo leia os emails que o usuário pode acessar, incluindo os próprios contatos do usuário e os emails compartilhados. | Não |
| _Mail.ReadWrite.Shared_ |    Ler e registrar usuário e emails compartilhados | Permite que o aplicativo crie, leia, atualize e exclua emails que o usuário tem permissão de acessar, incluindo os emails compartilhados e os do próprio usuário. Não inclui a permissão para enviar emails. | Não |
| _Mail.Send_ |    Enviar email como um usuário | Permite ao aplicativo enviar emails como usuários na organização. | Não |
| _Mail.Send.Shared_ |    Enviar email em nome de outras pessoas | Permite que o aplicativo enviar emails como o usuário conectado no, incluindo o envio de nome de terceiros. | Não |
| _MailboxSettings.Read_ |  Ler as configurações da caixa de correio do usuário | Permite ao aplicativo ler as configurações da caixa de correio do usuário. Não inclui a permissão para enviar emails. | Não |
| _MailboxSettings.ReadWrite_ |  Leia e grave as configurações de caixa de correio do usuário | Permite ao aplicativo criar, ler, atualizar e excluir as configurações da caixa de correio do usuário. Não inclui a permissão para enviar emails. | Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_       |    Ler emails em todas as caixas de correio | Permite ao aplicativo ler emails em todas as caixas de correio sem um usuário conectado.| Sim |
| _Mail.ReadWrite_ |    Ler e gravar emails em todas as caixas de correio | Permite ao aplicativo criar, ler, atualizar e excluir emails em todas as caixas de correio sem um usuário conectado. Não inclui a permissão para enviar emails. | Sim |
| _Mail.Send_ |    Enviar email como qualquer usuário | Permite ao aplicativo enviar emails como qualquer usuário sem um usuário conectado. | Sim | 
| _MailboxSettings.Read_ |  Ler as configurações de caixa de correio do usuário | Permite que o aplicativo leia configurações da caixa de correio do usuário sem um usuário conectado. Não inclui a permissão para enviar emails. | Não |
| _MailboxSettings.ReadWrite_ | Leia e grave todas as configurações de caixa de correio do usuário  | Permite que o aplicativo crie, leia, atualize e exclua as configurações da caixa de correio sem um usuário conectado. Não inclui a permissão para enviar emails. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários

_Mail.Read.Shared_, _Mail.ReadWrite.Shared_, e _Mail.Send.Shared_ só são válidos para contas corporativas ou de estudante. Todas as demais permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante.

Com a permissão _Mail.Send_ ou _Mail.Send.Shared_, um aplicativo pode enviar emails e salvar uma cópia na pasta Itens Enviados do usuário, mesmo se o aplicativo não usar uma permissão _Mail.ReadWrite_ ou _Mail.ReadWrite.Shared_ correspondente.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso

<a id="delegated" class="xliff"></a>

#### Delegado

* _Mail.Read_: Listar mensagens na caixa de entrada do usuário classificadas por `receivedDateTime` (`GET /me/mailfolders/inbox/messages?$orderby=receivedDateTime DESC`).
* _Mail.Read.Shared_: Localizar todas as mensagens com anexos na caixa de entrada de um usuário que compartilhou sua caixa de entrada com o usuário conectado (`GET /users{id | userPrincipalName}/mailfolders/inbox/messages?$filter=hasAttachments eq true`).
* _Mail.ReadWrite_: Marcar uma mensagem lida (`PATCH /me/messages/{id}`).
* _Mail.Send_: Enviar uma mensagem (`POST /me/sendmail`).
* _MailboxSettings.ReadWrite_: Atualizar a resposta automática do usuário (`PATCH /me/mailboxSettings`).

<a id="application" class="xliff"></a>

#### Aplicativo

* _Mail.Read_: Localizar mensagens de pedro@contoso.com (`GET /users/{id | userPrincipalName}/messages?$filter=from/emailAddress/address eq 'bob@contoso.com'`).
* _Mail.ReadWrite_: Criar uma nova pasta na Caixa de Entrada chamada `Expense Reports` (`POST /users/{id | userPrincipalName}/mailfolders`).
* _Mail.Send_: Enviar uma mensagem (`POST /users/{id | userPrincipalName}/sendmail`).
* _MailboxSettings.Read_: Obter o fuso horário padrão para a caixa de correio do usuário (`GET /users/{id | userPrincipalName}/mailboxSettings/timeZone`)


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="member-permissions" class="xliff"></a>

## Permissões de membro

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

Nenhum

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Member.Read.Hidden_ | Ler todas as associações ocultas | Permite que o aplicativo leia as associações de grupos ocultos e unidades administrativas sem um usuário conectado. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários
A associação pode estar oculta em alguns grupos do Office 365. Isso significa que somente os membros do grupo podem exibir seus membros. Esse recurso pode ser usado para ajudar a cumprir regulamentos que exijam a ocultação da associação do grupo de pessoas externas (por exemplo, um grupo do Office 365 que representa os alunos registrados em uma classe).

<a id="example-usage" class="xliff"></a>

### Exemplo de uso

<a id="application" class="xliff"></a>

#### Aplicativo

* _Member.Read.Hidden_: Ler os membros de uma unidade administrativa com associação oculta (`GET /administrativeUnits/{id}/members`).
* _Member.Read.Hidden_: Ler os membros de um grupo com associação oculta (`GET /groups/{id}/members`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="notes-permissions" class="xliff"></a>

## Permissões de anotações
<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read_ |    Ler blocos de anotações do OneNote do usuário | Permite ao aplicativo ler os títulos dos blocos de anotações e seções do OneNote e criar novas páginas, blocos de anotações e seções em nome do usuário conectado. | Não |
| _Notes.Create_ |    Criar blocos de anotações do OneNote do usuário | Permite ao aplicativo ler os títulos dos blocos de anotações e seções do OneNote e criar novas páginas, blocos de anotações e seções em nome do usuário conectado.| Não |
| _Notes.ReadWrite_ |    Ler e gravar blocos de anotações do OneNote do usuário | Permite ao aplicativo ler, compartilhar e modificar blocos de anotações do OneNote em nome do usuário conectado. | Não |
| _Notes.Read.All_ |    Ler todos os blocos de anotações do OneNote que o usuário pode acessar | Permite que o aplicativo leia os blocos de anotações do OneNote aos quais o usuário conectado tem acesso dentro da organização. | Não |
| _Notes.ReadWrite.All_ |    Ler e gravar todos os blocos de anotações do OneNote que o usuário pode acessar | Permite que o aplicativo leia, compartilhe e modifique blocos de anotações do OneNote aos quais o usuário conectado tem acesso dentro da organização.| Não |
| _Notes.ReadWrite.CreatedByApp_ |    Acesso limitado ao bloco de anotações (preterido) | **Preterido** <br/>Não usar. Essa permissão não concede privilégios. | Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read.All_ |    Ler todos os blocos de anotações do OneNote | Permite que o aplicativo leia todos os blocos de anotações do OneNote em sua organização sem um usuário conectado. | Sim |
| _Notes.ReadWrite.All_ |    Ler e gravar todos os blocos de anotações do OneNote | Permite que o aplicativo leia, compartilhe e modifique todos os blocos de anotações do OneNote em sua organização sem um usuário conectado.| Sim |


<a id="remarks" class="xliff"></a>

### Comentários
_Notes.Read.All_ e _Notes.ReadWrite.All_ só são válidos para contas corporativas ou de estudante. Todas as demais permissões são válidas tanto para contas da Microsoft como para contas corporativas e de estudante.

Com a permissão _Notes.Create_, um aplicativo pode exibir a hierarquia do bloco de anotações do OneNote do usuário conectado e criar conteúdo do OneNote (blocos de anotações, grupos de seção, seções, páginas, etc.).

_Notes.ReadWrite_ e _Notes.ReadWrite.All_ também permitem que o aplicativo modifique as permissões no conteúdo do OneNote que pode ser acessado pelo usuário conectado. 

Para contas corporativas ou de estudante, _Notes.Read.All_ e _Notes.ReadWrite.All_ permitem que o aplicativo acesse o conteúdo do OneNote de outros usuários ao qual o usuário conectado tenha permissão dentro da organização.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _Notes.Create_: Criar novos blocos de anotações para o usuário conectado (`POST /me/onenote/notebooks`).
* _Notes.Read_: Criar blocos de anotações para o usuário conectado (`GET /me/onenote/notebooks`).
* _Notes.Read.All_: Obter todos os blocos de anotações aos quais o usuário conectado tenha acesso dentro da organização (`GET /me/onenote/notebooks?includesharednotebooks=true`).
* _Notes.ReadWrite_: Atualizar a página do usuário conectado (`PATCH /me/onenote/pages/{id}/$value`).
* _Notes.ReadWrite.All_: Criar uma página no bloco de anotações de outro usuário ao qual o usuário conectado tenha acesso ao dentro da organização (`POST /users/{id}/onenote/pages`).

<a id="application" class="xliff"></a>

#### Aplicativo

* _Notes.Read.All_: Ler todos os blocos de anotações de usuários em um grupo (`GET /groups/{id}/onenote/notebooks`).
* _Notes.ReadWrite.All_: Atualizar a página em um bloco de anotações para qualquer usuário da organização (`PATCH /users/{id}/onenote/pages/{id}/$value`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="openid-permissions" class="xliff"></a>

## Permissões do OpenID

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _email_ |    Exibir o endereço de email do usuário | Permite ao aplicativo ler o endereço de email principal do usuário. | Não |
| _offline_access_ |    Acessar dados do usuário a qualquer momento | Permite ao aplicativo ler e atualizar dados do usuário, mesmo quando eles não estiver usando o aplicativo.| Não |
| _openid_ |    Conectar os usuários | Permite aos usuários entrar no aplicativo com contas corporativas ou de estudante e permite ao aplicativo ver informações básicas do perfil do usuário.| Não |
| _profile_ |    Exibir os perfis básicos dos usuários | Permite que o aplicativo veja o perfil básico do usuário (nome, foto, nome de usuário).| Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

Nenhum

<a id="remarks" class="xliff"></a>

### Comentários
Você pode usar essas permissões para especificar os artefatos que deseja que sejam retornados nas solicitações de token e de autorização do Azure AD. O suporte a elas é oferecido de formas diferentes nos pontos de extremidade v 1.0 e v 2.0. do Azure AD.

Com o ponto de extremidade (v 1.0) do Azure AD, somente a permissão _openid_ é usada. Você especifica no parâmetro *scope*, na solicitação de autorização, para retornar um token de ID quando usar o protocolo OpenID Connect para conectar um usuário ao seu aplicativo. Para saber mais, confira o artigo [Autorizar o acesso aos aplicativos web usando o OpenID Connect e o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-protocols-openid-connect-code). Para retornar com êxito um token de ID, você também deve garantir que a permissão _User.Read_ esteja configurada quando você registrar seu aplicativo. 

Com o ponto de extremidade v 2.0 do Azure AD, você especifica a permissão _offline\_access_ no parâmetro _scope_ para solicitar explicitamente um token de atualização quando estiver usando os protocolos OAuth 2.0 ou OpenID Connect. Com o OpenID Connect, você especifica a permissão _openid_ para solicitar um token de ID. Também é possível especificar a permissão _email_, a permissão _profile_, ou ambas, para retornar declarações adicionais no token de ID. Você não precisa especificar a _User.Read_ para retornar um token de ID com o ponto de extremidade v 2.0. Para saber mais, confira os [escopos do OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes).

> **Importante** A Biblioteca de Autenticação da Microsoft (MSAL) atualmente especifica as permissões _offline\_access_, _openid_, _profile_ e _email_ por padrão nas solicitações de autorização e de token. Isso significa que, para o caso padrão, se você especificar explicitamente essas permissões, o Azure AD pode retornar um erro.
>  

---

<a id="people-permissions" class="xliff"></a>

## Permissões de pessoas

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read_ |    Ler listas de pessoas relevantes dos usuários (visualização) | Permite ao aplicativo ler uma lista classificada de pessoas relevantes do usuário conectado. A lista inclui contatos locais, contatos das redes sociais, diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).| Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

Nenhum

<a id="remarks" class="xliff"></a>

### Comentários


<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="reports-permissions" class="xliff"></a>

## Permissões de relatórios

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

Nenhum

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Reports.Read.All_ | Ler todos os relatórios de uso | Permite que um aplicativo leia todos os relatórios de uso de serviço sem um usuário conectado. Serviços que fornecem relatórios de uso incluem o Office 365 e Azure Active Directory. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários
As permissões de relatórios só são válidas para contas corporativas ou de estudante. 

<a id="example-usage" class="xliff"></a>

### Exemplo de uso

<a id="application" class="xliff"></a>

#### Aplicativo

* _Reports.Read.All_: Ler o relatório de detalhes de uso de aplicativos de email com período de 7 dias (`GET /reports/EmailAppUsage(view='Detail',period='D7')/content`)
* _Reports.Read.All_: Ler o relatório de detalhes de atividade de email com data de '2017-01-01' (`GET /reports/EmailActivity(view='Detail',data='2017-01-01')/content`)
* _Reports.Read.All_: Ler o relatório de detalhes de ativações do Office 365 (`GET /reports/Office365Activations(view='Detail')/content`)

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="sites-permissions" class="xliff"></a>

## Permissões de sites

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Sites.Read.All_ |    Ler itens em todos os conjuntos de sites | Permite ao aplicativo ler documentos e listar itens em todos os conjuntos de sites em nome do usuário conectado. | Não |
| _Sites.ReadWrite.All_ |    Ler e gravar listas itens em todos os conjuntos de sites | Permite que o aplicativo edite ou exclua documentos e liste itens em todos os conjuntos de sites em nome do usuário conectado. | Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

Nenhum

<a id="remarks" class="xliff"></a>

### Comentários
Essas permissões de sites só são válidas para contas corporativas ou de estudante.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _Sites.Read.All_: Ler as listas no site raiz do SharePoint (`GET /beta/sharePoint/site/lists`)
* _Sites.ReadWrite.All_: Criar novos itens de lista em uma lista do SharePoint (`POST /beta/sharePoint/site/lists/123/items`)


Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="tasks-permissions" class="xliff"></a>

## Permissões de tarefas

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Tasks.Read_ | Ler tarefas do usuário | Permite que o aplicativo leia as tarefas do usuário. | Não |
| _Tasks.Read.Shared_ | Ler as tarefas do usuário e as tarefas compartilhadas | Permite que o aplicativo leia as tarefas que o usuário tem permissão de acessar, incluindo as próprias tarefas e as tarefas compartilhadas. | Não |
| _Tasks.ReadWrite_ |    Criar, ler, atualizar e excluir tarefas e contêineres do usuário | Permite ao aplicativo criar, ler, atualizar e excluir tarefas e contêineres (e tarefas neles) que são atribuídos ou compartilhados com o usuário conectado.| Não |
| _Tasks.ReadWrite.Shared_ | Ler e registrar as tarefas do usuário e as tarefas compartilhadas | Permite que o aplicativo crie, leia, atualize e exclua as tarefas permitidas para um usuário, incluindo suas próprias tarefas e as compartilhadas. | Não |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

Nenhum

<a id="remarks" class="xliff"></a>

### Comentários
As permissões de _tarefas_ são usadas para controlar o acesso de tarefas do Outlook. O acesso a tarefas do Microsoft Planner é controlado pelas permissões do [_Grupo_](#group-permissions).

As permissões _Compartilhadas_ atualmente só são compatíveis com contas corporativas ou de estudante. Mesmo com permissões _Compartilhadas_, as leituras e gravações podem falhar se o usuário que possui o conteúdo compartilhado não tiver concedido as permissões de usuário de acesso para modificar o conteúdo dentro da pasta.

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _Tasks.Read_: Obter todas as tarefas na caixa de correio do usuário (`GET /me/outlook/tasks`).
* _Tasks.Read.Shared_: Acessar tarefas em uma pasta compartilhada com você por outro usuário em sua organização (`Get /users{id|userPrincipalName}/outlook/taskfolders/{id}/tasks`).
* _Tasks.ReadWrite_: Adicionar um evento à pasta de tarefas padrão do usuário (`POST /me/outook/tasks`).
* _Tasks.Read_: Obter todas as tarefas não concluídas na caixa de correio do usuário (`GET /users/{id | userPrincipalName}/outlook/tasks?$filter=status ne 'completed'`).
* _Tasks.ReadWrite_: Atualizar uma tarefa na caixa de correio do usuário (`PATCH /users/{id | userPrincipalName}/outlook/tasks/id`).
* _Tasks.ReadWrite.Shared_: Concluir uma tarefa em nome de outro usuário (`POST /users/{id | userPrincipalName}/outlook/tasks/id/complete`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="user-permissions" class="xliff"></a>

## Permissões do usuário

<a id="delegated-permissions" class="xliff"></a>

#### Permissões delegadas

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read_       |    Entrar e ler o perfil do usuário | Permite aos usuários entrar no aplicativo e permite ao aplicativo ler o perfil de usuários conectados. Também permite que o aplicativo leia as informações básicas da empresa sobre os usuários conectados.| Não |
| _User.ReadWrite_ |    Acesso de leitura e gravação ao perfil de usuário | Permite ao aplicativo ler o seu perfil. Ele também permite ao aplicativo atualizar suas informações de perfil em seu nome. | Não |
| _User.ReadBasic.All_ |    Ler os perfis básicos de todos usuários | Permite ao aplicativo ler um conjunto básico de propriedades de perfil de outros usuários em sua organização em nome do usuário conectado. Inclui o nome para exibição, nome e sobrenome, endereço de email e foto. | Não |
| _User.Read.All_  |     Ler os perfis completos de todos os usuários           | Permite ao aplicativo ler o conjunto completo de propriedades do perfil, relatórios e gerentes de outros usuários em sua organização, em nome do usuário conectado. | Sim |
| _User.ReadWrite.All_ |     Ler e gravar os perfis completos de todos os usuários | Permite ao aplicativo ler e gravar o conjunto completo de propriedades do perfil, relatórios e gerentes de outros usuários na sua organização, em nome do usuário conectado. Também permite que o aplicativo crie e exclua usuários, além de redefinir senhas de usuário em nome do usuário conectado. | Sim |
| _User.Invite.All_  |     Convidar usuários convidados para a organização | Permite que o aplicativo convide usuários para sua organização em nome do usuário conectado. | Sim |

<a id="application-permissions" class="xliff"></a>

#### Permissões de aplicativos

|   Permissão    |  Exibir Cadeia de Caracteres   |  Descrição | Consentimento Obrigatório do Administrador |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read.All_ |    Ler os perfis completos de todos os usuários | Permite ao aplicativo ler o conjunto completo de propriedades do perfil, relatórios e gerenciadores de outros usuários na sua organização, sem um usuário conectado.| Sim |
| _User.ReadWrite.All_ |   Ler e gravar os perfis completos de todos os usuários | Permite ao aplicativo ler e gravar o conjunto completo de propriedades do perfil, relatórios e gerentes de outros usuários na sua organização, sem um usuário conectado.  Também permite que o aplicativo crie e exclua usuários não administrativos. Não permite a redefinição de senhas de usuário. | Sim |
| _User.Invite.All_  |     Convidar usuários convidados para a organização | Permite que o aplicativo convide usuários para sua organização sem um usuário conectado. | Sim |

<a id="remarks" class="xliff"></a>

### Comentários

As únicas permissões válidas para contas da Microsoft são _User.Read_ e _User.ReadWrite_. Todas as permissões são válidas para contas corporativas ou de estudante.

Com a permissão _User.Read_, um aplicativo também pode ler as informações básicas da empresa do usuário conectado de uma conta corporativa ou de estudante através do recurso [Organização](../api-reference/v1.0/resources/organization.md). As propriedades a seguir estão disponíveis: id, displayName e verifiedDomains.

Para contas corporativas ou de estudante, o perfil completo inclui todas as propriedades declaradas do recurso [Usuário](../api-reference/v1.0/resources/user.md). No caso das leituras, somente um número limitado de propriedades é retornado por padrão. Para ler propriedades que não estão no conjunto padrão, use `$select`. As propriedades padrão são:

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
- Foto
- preferredName
- responsibilities
- schools
- skills

Com a Permissão de aplicativo _User.ReadWrite.All_, o aplicativo pode atualizar todas as propriedades declaradas das contas corporativas ou de estudante, com exceção da senha.

Para ler ou gravar os subordinados diretos (`directReports`) ou o gerente (`manager`) de uma conta corporativa ou de estudante, o aplicativo deve ter as permissões _User.Read.All_ (somente leitura) ou _User.ReadWrite.All_.

A permissão _User.ReadBasic.All_ restringe o acesso do aplicativo a um conjunto limitado de propriedades conhecido como o perfil básico. Isso ocorre porque o perfil completo pode conter informações de diretório confidenciais. O perfil básico inclui apenas as seguintes propriedades: 

- displayName
- givenName
- Email
- Foto
- surname
- userPrincipalName

Para ler as associações de grupos de um usuário (`memberOf`), o aplicativo deve ter o [_Group.Read.All_](#group-permissions) ou o [_Group.ReadWrite.All_](#group-permissions). No entanto, se o usuário também tiver uma associação a um [directoryRole](../api-reference/v1.0/resources/directoryrole.md) ou [administrativeUnit](../api-reference/beta/resources/administrativeunit.md), o aplicativo também precisará de permissões efetivas para ler esses recursos ou o Microsoft Graph retornará um erro. Isso significa que o aplicativo deve ter também [Permissões do diretório](#directory-permissions); para as Permissões Delegadas, o usuário conectado deve ter privilégios suficientes na organização para acessar unidades administrativas e funções de diretório. 

<a id="example-usage" class="xliff"></a>

### Exemplo de uso
<a id="delegated" class="xliff"></a>

#### Delegado

* _User.Read_: Ler o perfil completo para o usuário conectado (`GET /me`).
* _User.ReadWrite_: Atualizar a foto do usuário conectado (`PUT /me/photo/$value`).
* _User.ReadBasic.All_: Localizar todos os usuários cujos nomes começam com "Davi" (`GET /users?$filter=startswith(displayName,'David')`).
* _User.Read.All_: Ler o gerente do usuário (`GET /user/{id | userPrincipalName}/manager`).


<a id="application" class="xliff"></a>

#### Aplicativo

* _User.Read.All_: Ler todos os usuários e relações usando a consulta delta (`GET /beta/users/delta?$select=displayName,givenName,surname`).
* _User.ReadWrite.All_: Atualizar a foto de qualquer usuário na organização (`PUT /user/{id | userPrincipalName}/photo/$value`).

Para cenários mais complexos que envolvem várias permissões, confira [Cenários de permissões](#permission-scenarios).

---

<a id="permission-scenarios" class="xliff"></a>

## Cenários de permissão

Esta seção mostra alguns cenários comuns direcionados aos recursos [usuário](../api-reference/v1.0/resources/user.md) e [grupo](../api-reference/v1.0/resources/group.md) em uma organização. As tabelas mostram as permissões que um aplicativo precisa para conseguir executar operações específicas necessárias para o cenário. Observe que, em alguns casos, a capacidade do aplicativo de executar operações específicas dependerá se uma permissão é uma Permissão de aplicativo ou Permissão Delegada. No caso de Permissões Delegadas, as Permissões Efetivas do aplicativo também dependerão dos privilégios do usuário conectado na organização. Para obter mais informações, confira [Permissões delegadas, Permissões de aplicativo e permissões efetivas](#delegated-permissions-application-permissions-and-effective-permissions).

<a id="access-scenarios-on-the-user-resource" class="xliff"></a>

### Cenários de acesso do recurso Usuário

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
   

<a id="access-scenarios-on-the-group-resource" class="xliff"></a>

### Cenários de acesso do recurso Grupo
    
| **Tarefas do aplicativo envolvendo o Grupo**  |  **Permissões necessárias** |  **Cadeias de caracteres de permissão** |
|:-------------------------------|:---------------------|:---------------|
| O aplicativo deseja ler as informações básicas do grupo (somente o nome para exibição e a imagem), por exemplo, para mostrar uma experiência de seleção de um grupo  | _Group.Read.All_  | Ler todos os grupos|
| O aplicativo deseja ler todo o conteúdo em todos os grupos do Office 365, incluindo arquivos, conversas.  Também precisa mostrar associações de grupo, ser capaz de atualizar associações de grupo (caso seja o proprietário).  |  _Group.Read.All_ | Ler itens em todos os conjuntos de sites, ler todos os grupos|
| O aplicativo deseja ler e gravar todo o conteúdo em todos os grupos do Office 365, incluindo arquivos, conversas.  Também precisa mostrar associações de grupo, ser capaz de atualizar associações de grupo (caso seja o proprietário).  |   _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  Ler e gravar todos os grupos, editar ou excluir itens em todos os conjuntos de sites |
| O aplicativo deseja descobrir (localizar) um grupo do Office 365. Permite ao usuário procurar um grupo específico e escolher um deles na lista enumerada para ingressar no grupo.     | _Group.ReadWrite.All_ | Ler e gravar todos os grupos|
| O aplicativo deseja criar um grupo por meio do AAD Graph |   _Group.ReadWrite.All_ | Ler e gravar todos os grupos|
