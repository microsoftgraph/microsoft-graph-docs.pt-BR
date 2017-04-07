# <a name="microsoft-graph-permission-scopes"></a>Escopos de permissão do Microsoft Graph

O Microsoft Graph expõe os escopos de permissão do OAuth 2.0 que são usados para controlar o acesso que um aplicativo tem aos recursos. Como desenvolvedor, você especifica os escopos de permissão apropriados para o acesso que o seu aplicativo exige. Se você estiver usando a autenticação do Azure AD, normalmente fará isso por meio do Portal de Gerenciamento do Azure. Se você estiver usando o ponto de extremidade do Azure AD v2.0, solicite permissões dinamicamente durante o tempo de execução.

Depois de entrar, os usuários ou administradores recebem a oportunidade de consentir em permitir o acesso do aplicativo aos seus recursos com os escopos de permissão que você configurou. Por esse motivo, você deve escolher os escopos de permissão que fornecem o menor nível de privilégios exigido pelo seu aplicativo. Para mais detalhes sobre como configurar permissões para o seu aplicativo e sobre o processo de consentimento, confira <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-integrating-applications/" target="_newtab">Integrar Aplicativos com o Azure Active Directory</a>.

>**Observação:** Algumas permissões do Microsoft Graph, como as que pertencem a grupos e tarefas, não são aplicáveis a contas pessoais.  

##<a name="app-only-vs-delegated-permissions"></a>Somente de aplicativo vs. permissões delegadas
Os escopos de permissão podem ser somente do aplicativo ou delegado. Os escopos somente do aplicativo (também conhecidos como funções do aplicativo) concedem ao aplicativo o conjunto completo de privilégios oferecidos pelo escopo. Os escopos somente do aplicativo são, geralmente, usados por aplicativos executados como um serviço, sem a presença de um usuário conectado. 


Os escopos de permissão delegados são para aplicativos que agem em nome de um usuário. Esses escopos delegam privilégios do usuário conectado, permitindo que o aplicativo aja como o usuário. Os reais privilégios concedidos ao aplicativo serão a combinação menos privilegiada (a interseção) dos privilégios concedidos pelo escopo e aqueles que pertencem ao usuário conectado. Por exemplo, se o escopo de permissão conceder privilégios delegados para gravar todos os objetos do diretório, mas o usuário conectado tiver privilégios apenas para atualizar seu próprio perfil de usuário, o aplicativo só poderá gravar o perfil do usuário conectado, mas não outros objetos.

> **Observação**: Para grupos, apenas um subconjunto da API relacionado à administração do grupo principal e ao suporte para gerenciamento, ambos de permissões somente de aplicativo e delegadas. Todos os outros membros do suporte da API do grupo apenas permissões delegadas. Consulte [problemas conhecidos](../overview/release_notes.md#groups) para obter exemplos.

## <a name="full-and-basic-profiles-for-users-and-groups"></a>Perfis completos e básicos para usuários e grupos

O perfil completo (ou perfil) de um Usuário ou de um Grupo inclui todas as propriedades declaradas da entidade. Como o perfil pode conter informações confidenciais do diretório ou informações de identificação pessoal (PII), vários escopos restringem o acesso do aplicativo a um conjunto limitado de propriedades, conhecidas como um perfil básico. Para os usuários, o perfil básico inclui apenas as seguintes propriedades: 

- Nome para exibição
- Nome e sobrenome
- Foto
- Endereço de email

Para grupos, o perfil básico contém apenas o nome de exibição. 

<!---    <a name="msg_perm_details"> </a>  -->

## <a name="permission-scope-details"></a>Detalhes do escopo de permissão

Você deve configurar seu aplicativo para ter as permissões necessárias para acessar os recursos do Microsoft Graph. As permissões têm como escopo recursos individuais para os direitos de ler, de gravar ou ambos. 

As tabelas a seguir listam os escopos de permissão do Microsoft Graph e explicam o acesso concedido por cada um. 

- A coluna **Escopo** lista o nome do escopo. Nomes de escopos têm o formato recurso.operação.restrição. Por exemplo, Group.ReadWrite.All. Se a restrição for "All", o escopo concederá ao aplicativo a possibilidade de realizar a operação (ReadWrite) em todos os recursos especificados (Group) no diretório; caso contrário, o escopo só permitirá a operação no perfil do usuário conectado. Os escopos podem conceder privilégios limitados para a operação especificada. Confira a coluna **Descrição** para obter detalhes.
- A coluna **Permissão** mostra como o escopo é exibido no portal do Azure. 
- A coluna **Descrição** descreve o conjunto completo de privilégios concedidos pelo escopo. Para escopos delegados, o acesso real concedido ao aplicativo será a combinação menos privilegiada (interseção) do acesso concedido pelo escopo e aqueles que pertencem ao usuário conectado. 
- Os escopos são agrupados dependendo se as permissões exigem consentimento do administrador.

  > **Observação**: Confira [Problemas conhecidos](../overview/release_notes.md) para saber as limitações do escopo de permissão de `v1.0` e `beta`.
  
###<a name="permissions-requiring-administrators-consent"></a>Permissões que exigem o consentimento do administrador

|   **Escopo**                  |  **Permissão**                          |  **Descrição** |
|:-----------------------------|:-----------------------------------------|:-----------------|
| _Directory.AccessAsUser.All_   |     Access Directory como o usuário conectado  | Permite ao aplicativo ter o mesmo acesso que o usuário conectado a informações no diretório.|
| _Directory.Read.All_           |     Ler dados do diretório                     | Permite ao aplicativo ler dados no diretório da sua organização, como usuários, grupos e aplicativos. |
| _Directory.ReadWrite.All_      |     Ler e gravar dados de diretório           | Permite ao aplicativo ler e gravar dados no diretório da sua organização, como usuários e grupos.  Não permite a exclusão de usuários ou grupos. Não permite ao aplicativo excluir usuários ou grupos, ou redefinir senhas de usuário. |
| _Group.Read.All_ |    Ler todos os grupos | Permite ao aplicativo listar grupos, e ler suas propriedades e todas as associações do grupo em nome do usuário conectado.  Também permite ao aplicativo ler calendário, conversas, arquivos e outros tipos de conteúdo de todos os grupos que o usuário conectado pode acessar. |
| _Group.ReadWrite.All_ |    Ler e gravar todos os grupos| Permite ao aplicativo criar grupos e ler todas as propriedades e associações do grupo em nome do usuário conectado.  Além disso, permite aos proprietários do grupo gerenciar seus grupos, e permite aos membros do grupo atualizar o conteúdo do grupo. |
| _User.Read.All_                |     Ler os perfis completos de todos os usuários           | Igual a User.ReadBasic.All, exceto por permitir que o aplicativo leia o perfil completo de todos os usuários na organização e ao ler as propriedades de navegação como gerente e subordinado direto. O perfil completo inclui todas as propriedades declaradas da entidade **Usuário**. Para ler os grupos dos quais um usuário é membro, o aplicativo também exigirá Group.Read.All ou Group.ReadWrite.All. |
| _User.ReadWrite.All_           |     Ler e gravar os perfis completos de todos os usuários | Permite ao aplicativo ler e gravar o conjunto completo de propriedades do perfil, relatórios e gerenciadores de outros usuários na sua organização, em nome do usuário conectado. |


###<a name="permissions-not-requiring-administrators-consent"></a>Permissões que não exigem o consentimento do administrador

|   **Escopo**    |  **Permissão**   |  **Descrição** |
|:-----------------------------|:-----------------------------------------|:-----------------|
| _Calendars.Read_ |    Ler calendários do usuário  | Permite ao aplicativo ler eventos nos calendários do usuário.|
| _Calendars.Read.Shared_ |    Ler usuários e calendários compartilhados | Permite que o aplicativo leia os eventos em todos os calendários a que o usuário tem acesso, incluindo os delegados e os calendários compartilhados. |
| _Calendars.ReadWrite_ |    Ter acesso total aos calendários do usuário  | Permite ao aplicativo criar, ler, atualizar e excluir eventos em calendários do usuário. |
| _Calendars.ReadWrite.Shared_ |    Ler e registrar usuário e calendários compartilhados | Permite ao aplicativo criar, ler, atualizar e excluir eventos de todos os calendários que o usuário tenha permissão para acessar. Isso inclui o delegado e os calendários compartilhados.|
| _Contacts.Read_ |    Ler contatos do usuário  | Permite ao aplicativo ler os contatos do usuário. |
| _Contacts.Read.Shared_ |    Ler usuário e contatos compartilhados | Permite que o aplicativo leia os contatos que o usuário tem permissão de acessar, incluindo os próprios contatos do usuário e os contatos compartilhados. |
| _Contacts.ReadWrite_ |    Ter acesso total aos contatos do usuário  | Permite ao aplicativo criar, ler, atualizar e excluir contatos do usuário. |
| _Contacts.ReadWrite.Shared_ |    Ler e registrar usuário e contatos compartilhados | Permite que o aplicativo crie, leia, atualize e exclua os contatos para os quais o usuário tem permissão, incluindo os próprios contatos do usuário e os contatos compartilhados.|
| _Files.Read_ |    Ler arquivos do usuário e arquivos compartilhados com o usuário | Permite ao aplicativo ler os arquivos do usuário conectado e os arquivos compartilhados com o usuário.| 
| _Files.Read.All_ | Ler todos os arquivos que o usuário pode acessar | Permite que o aplicativo para leia todos os arquivos que o usuário conectado pode acessar. |
| _Files.Read.Selected_ |    Ler arquivos selecionados pelo usuário  | Permite ao aplicativo ler arquivos selecionados pelo usuário. O aplicativo tem acesso por várias horas depois que o usuário seleciona um arquivo. |
| _Files.ReadWrite_ |   Ter acesso total a arquivos do usuário e arquivos compartilhados com o usuário | Permite ao aplicativo ler, criar, atualizar e excluir os arquivos do usuário conectado e os arquivos compartilhados com o usuário. |
| _Files.ReadWrite.All_ | Ter acesso total a todos os arquivos que o usuário pode acessar | Permite que o aplicativo leia, crie, atualize e exclua todos os arquivos que o usuário conectado pode acessar. |
| _Files.ReadWrite.AppFolder_ | Tem acesso total à pasta do aplicativo | Permite que o aplicativo leia, crie, atualize e exclua arquivos na pasta do aplicativo. |
| _Files.ReadWrite.Selected_ |    Ler e gravar arquivos selecionados pelo usuário | Permite ao aplicativo ler e gravar arquivos selecionados pelo usuário. O aplicativo tem acesso por várias horas depois que o usuário seleciona um arquivo. |
| _Mail.Read_ |    Ler emails do usuário | Permite ao aplicativo ler emails em caixas de correio do usuário. |
| _Mail.Read.Shared_ |    Ler email compartilhado e de usuário | Permite que o aplicativo leia os emails que o usuário pode acessar, incluindo os próprios contatos do usuário e os emails compartilhados. |
| _Mail.ReadWrite_ |    Acesso de leitura e gravação aos emails do usuário | Permite ao aplicativo criar, ler, atualizar e excluir emails em caixas de correio do usuário. Não inclui a permissão para enviar emails.|
| _Mail.ReadWrite.Shared_ |    Ler e registrar usuário e emails compartilhados | Permite que o aplicativo crie, leia, atualize e exclua emails que o usuário tem permissão de acessar, incluindo os emails compartilhados e os do próprio usuário. Não inclui a permissão para enviar emails. |
| _Mail.Send_ |    Enviar email como um usuário | Permite ao aplicativo enviar emails como usuários na organização. |
| _Mail.Send.Shared_ |    Enviar email em nome de outras pessoas | Permite que o aplicativo enviar emails como o usuário conectado no, incluindo o envio de nome de terceiros. |
| _MailboxSettings.ReadWrite_ |  Leia e grave as configurações de caixa de correio do usuário | Permite ao aplicativo criar, ler, atualizar e excluir as configurações da caixa de correio do usuário. Não inclui a permissão para enviar emails.|
| _offline_access_ |    Acessar dados do usuário a qualquer momento (visualização) | Permite ao aplicativo ler e atualizar dados do usuário, mesmo quando eles não estiver usando o aplicativo.|
| _openid_ |    Conectar os usuários (visualização) | Permite aos usuários entrar no aplicativo com contas corporativas ou de estudante e permite ao aplicativo ver informações básicas do perfil do usuário.|
| _User.Read_       |    Entrar e ler o perfil do usuário | Permite aos usuários entrar no aplicativo e permite ao aplicativo ler o perfil de usuários conectados. O perfil completo inclui todas as propriedades declaradas da entidade Usuário. O aplicativo não pode ler as propriedades de navegação, como gerente ou subordinados diretos. Além disso, permite ao aplicativo ler as seguintes informações básicas da empresa do usuário conectado (por meio do objeto **TenantDetail**): ID de locatário, nome de exibição do locatário e domínios verificados.|
| _User.ReadWrite_ |    Acesso de leitura e gravação ao perfil de usuário | Permite ao aplicativo ler o seu perfil. Ele também permite ao aplicativo atualizar suas informações de perfil em seu nome. |
| _User.ReadBasic.All_ |    Ler os perfis básicos de todos usuários | Permite ao aplicativo ler o perfil básico de todos os usuários da organização em nome do usuário conectado. As seguintes propriedades compõem um perfil básico de usuário: nome de exibição, nome e sobrenome, foto e endereço de email. Para ler os grupos dos quais um usuário é membro, o aplicativo também exigirá Group.Read.All ou Group.ReadWrite.All.| 

###<a name="app-only-permissions-requiring-administrators-consent"></a>Permissões somente do aplicativo exigindo o consentimento do administrador

|   **Escopo**    |  **Permissão**   |  **Descrição** |
|:---------------|:------------------|:-----------------|
| _Calendars.Read_ |    Ler calendários em todas as caixas de correio | Permite ao aplicativo ler eventos de todos os calendários sem um usuário conectado. |
| _Calendars.ReadWrite_ |    Ler e gravar calendários em todas as caixas de correio | Permite ao aplicativo criar, ler, atualizar e excluir eventos de todos os calendários sem um usuário conectado.|
| _Contacts.Read_ |    Ler contatos em todas as caixas de correio | Permite ao aplicativo ler todos os contatos em todas as caixas de correio sem um usuário conectado. |
| _Contacts.ReadWrite_ |    Ler e gravar contatos em todas as caixas de correio  |Permite ao aplicativo criar, ler, atualizar e excluir todos os contatos em todas as caixas de correio sem um usuário conectado.|
| _Device.ReadWrite.All_ | Ler e registrar dispositivos | Permite que o aplicativo leia e registre todos as propriedades dos dispositivos sem um usuário conectado. Não permite a criação de dispositivos, exclusão de dispositivos ou atualização de identificadores de segurança de dispositivo alternativo. |
| _Directory.Read.All_ | Ler dados do diretório | Permite ao aplicativo ler dados no diretório da sua organização, como usuários, grupos e aplicativos, sem um usuário conectado. |
| _Directory.ReadWrite.All_ | Ler e gravar dados de diretório | Permite ao aplicativo ler e registrar dados no diretório de sua organização, como usuários e grupos, sem um usuário conectado. Não permite a exclusão de usuários ou grupos. |
| _Files.Read.All_ | Ler todos os arquivos que o usuário pode acessar | Permite ao aplicativo ler todos os arquivos em todos os conjuntos de sites sem um usuário conectado. |
| _Files.ReadWrite.All_ | Ter acesso total a todos os arquivos que o usuário pode acessar | Permite ao aplicativo ler, criar, atualizar e excluir todos os arquivos em todos os conjuntos de sites sem um usuário conectado. |
| _Group.Read.All_ | Ler todos os grupos | Permite ao aplicativo ler os associados de todos os grupos sem um usuário conectado. Observe que nem todas as API de grupo suportam o acesso usando permissões somente de aplicativo. Consulte [problemas conhecidos](../overview/release_notes.md#groups) para obter exemplos. |
| _Group.ReadWrite.All_ | Ler e gravar todos os grupos | Permite que o aplicativo crie grupos, leia e atualize as associações do grupo e exclua grupos. Todas essas operações podem ser executadas pelo aplicativo sem um usuário conectado. Observe que nem todas as API de grupo suportam o acesso usando permissões somente de aplicativo. Consulte [problemas conhecidos](../overview/release_notes.md#groups) para obter exemplos.|
| _Mail.Read_       |    Ler emails em todas as caixas de correio | Permite ao aplicativo ler emails em todas as caixas de correio sem um usuário conectado.|
| _Mail.ReadWrite_ |    Ler e gravar emails em todas as caixas de correio | Permite ao aplicativo criar, ler, atualizar e excluir emails em todas as caixas de correio sem um usuário conectado. Não inclui a permissão para enviar emails. |
| _Mail.Send_ |    Enviar email como qualquer usuário | Permite ao aplicativo enviar emails como qualquer usuário sem um usuário conectado. | 
| _MailboxSettings.ReadWrite_ | Leia e grave todas as configurações de caixa de correio do usuário  | Permite que o aplicativo crie, leia, atualize e exclua as configurações da caixa de correio sem um usuário conectado. Não inclui a permissão para enviar emails. |
| _Member.Read.Hidden_ | Ler todas as associações ocultas | Permite que o aplicativo leia as associações de grupos ocultos e unidades administrativas sem um usuário conectado. |
| _Reports.Read.All_ | Ler todos os relatórios de uso | Permite que um aplicativo leia todos os relatórios de uso de serviço sem um usuário conectado. Serviços que fornecem relatórios de uso incluem o Office 365 e Azure Active Directory. |
| _User.Read.All_ |    Ler os perfis completos de todos os usuários | Permite ao aplicativo ler o conjunto completo de propriedades do perfil, relatórios e gerenciadores de outros usuários na sua organização, sem um usuário conectado.| 
| _User.ReadWrite.All_ |   Ler e gravar os perfis completos de todos os usuários | Permite ao aplicativo ler e gravar o conjunto completo de propriedades do perfil, relatórios e gerenciadores de outros usuários na sua organização, sem um usuário conectado.|


##<a name="permission-scopes-in-preview"></a>Escopos de permissão em visualização

###<a name="permissions-requiring-administrators-consent-preview"></a>Permissões que exigem o consentimento do administrador (visualização)

|   **Escopo**    |  **Permissão**   |  **Descrição** |
|:---------------|:------------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   Leia as informações de evento de risco de identidade (visualização) | Permite que o aplicativo para leia as informações de evento de risco de identidade para todos os usuários em sua organização em nome do usuário conectado. |
| _DeviceManagementServiceConfiguration.Read.All_ | Configuração de leitura Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades do serviço do Microsoft Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. |
| _DeviceManagementServiceConfiguration.ReadWrite.All_ | Ler e registrar o Microsoft Intune (visualização) | Permite que o aplicativo leia e registre propriedades do serviço do Microsoft Intune, incluindo o registro do dispositivo e a configuração de conexão de serviço de terceiros. |
| _DeviceManagementConfiguration.Read.All_ | Ler a configuração de dispositivo e as políticas do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades configuração de dispositivo e das políticas de conformidade do Microsoft gerenciado Intune e sua atribuição aos grupos.  |
| _DeviceManagementConfiguration.ReadWrite.All_ | Ler e escrever as configurações de dispositivo e as políticas do Microsoft Intune (visualização) | Permite que o aplicativo leia e registre as propriedades de configuração de dispositivo e as políticas de conformidade de dispositivo do Microsoft Intune e sua atribuição aos grupos. |
| _DeviceManagementApps.Read.All_ | Ler aplicativos do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades, as atribuições de grupo, o status de aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. |
| _DeviceManagementApps.ReadWrite.All_ | Ler e registrar os aplicativos do Microsoft Intune (visualização) | Permite que aplicativo leia e registre s propriedades, as atribuições de grupo, o status dos aplicativos, as configurações de aplicativo e as políticas de proteção de aplicativo gerenciadas pelo Microsoft Intune. |
| _DeviceManagementRBAC.Read.All_ | Ler as configurações RBAC (Controle de Acesso com Base em Função) do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades relacionadas às configurações RBAC do Microsoft Intune. |
| _DeviceManagementRBAC.ReadWrite.All_ | Ler e registrar as configurações RBAC do Microsoft Intune (visualização) | Permite que o aplicativo leia e registre as propriedades relacionadas às configurações RBAC do Microsoft Intune. |
| _DeviceManagementManagedDevices.Read.All_ | Ler dispositivos do Microsoft Intune (visualização) | Permite que o aplicativo leia as propriedades de dispositivos gerenciados pelo Microsoft Intune. |
| _DeviceManagementManagedDevices.ReadWrite.All_ | Ler e registrar dispositivos do Microsoft Intune (visualização) | Permite que o aplicativo leia e registre as propriedades de dispositivos gerenciados pelo Microsoft Intune. Não permite operações de alto impacto como apagamento remoto e a redefinição de senha no proprietário do dispositivo. |
| _DeviceManagementManagedDevices.PrivilegedOperations.All_ | Executar ações remotas de impacto no usuário nos dispositivos do Microsoft Intune (visualização) | Permite que o aplicativo execute ações remotas de alto impacto como apagar dispositivo ou redefinir a senha em dispositivos gerenciados pelo Microsoft Intune. |

###<a name="permissions-not-requiring-administrators-consent-preview"></a>Permissões que não exigem o consentimento do administrador (visualização)

|   **Escopo**    |  **Permissão**   |  **Descrição** |
|:---------------|:------------------|:-----------------|
| _Notes.Create_ |    Create pages in users' notebooks (visualização) | Permite ao aplicativo ler os títulos dos blocos de anotações e seções, e criar novas páginas, blocos de anotações e seções em nome do usuário conectado.|
| _Notes.Read_ |    Ler blocos de anotações do usuário (visualização) | Permite ao aplicativo exibir os títulos dos blocos de anotações e seções do OneNote, e ler todas as páginas em nome do usuário conectado. Não pode exibir seções protegidas por senha. |
| _Notes.Read.All_ |    Ler todos os blocos de anotações que o usuário pode acessar (visualização) | Permite ao aplicativo ler os conteúdos de todos os blocos de anotações e seções que o usuário conectado pode acessar.   Não pode ler seções protegidas por senha. |
| _Notes.ReadWrite_ |    Ler e gravar blocos de anotações do usuário (visualização) | Permite ao aplicativo ler os títulos dos blocos de anotações e seções, ler todas as páginas, gravar todas as páginas e criar novas páginas em nome do usuário conectado.  Não pode acessar seções protegidas por senha. |
| _Notes.ReadWrite.All_ |    Ler e gravar todos os blocos de anotações que o usuário pode acessar (visualização) | Permite ao aplicativo ler e gravar os conteúdos de todos os blocos de anotações e seções que o usuário conectado pode acessar.  Não pode acessar seções protegidas por senha.|
| _Notes.ReadWrite.CreatedByApp_ |    Acesso limitado ao bloco de anotações (visualização) | Permite ao aplicativo ler os títulos de blocos de anotações e seções, criar novas páginas em nome do usuário conectado. Também permite ao aplicativo ler e atualizar as páginas criadas pelo aplicativo. |
| _People.Read_ |    Ler listas de pessoas relevantes dos usuários (visualização) | Permite ao aplicativo ler uma lista classificada de pessoas relevantes do usuário conectado. A lista inclui contatos locais, contatos das redes sociais, diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).|
| _Sites.Read.All_ |    Ler itens em todos os conjuntos de sites | Permite ao aplicativo ler documentos e listar itens em todos os conjuntos de sites em nome do usuário conectado. |
| _Sites.ReadWrite.All_ |    Ler e gravar listas itens em todos os conjuntos de sites | Permite que o aplicativo edite ou exclua documentos e liste itens em todos os conjuntos de sites em nome do usuário conectado. |
| _Tasks.Read_ | Ler tarefas do usuário | Permite que o aplicativo leia as tarefas do usuário. |
| _Tasks.Read.Shared_ | Ler as tarefas do usuário e as tarefas compartilhadas | Permite que o aplicativo leia as tarefas que o usuário tem permissão de acessar, incluindo as próprias tarefas e as tarefas compartilhadas. |
| _Tasks.ReadWrite_ |    Criar, ler, atualizar e excluir tarefas e planos do usuário (visualização) | Permite ao aplicativo criar, ler, atualizar e excluir tarefas e planos (e tarefas neles), que são atribuídos ou compartilhado com o usuário conectado.|
| _Tasks.ReadWrite.Shared_ | Ler e registrar as tarefas do usuário e as tarefas compartilhadas | Permite que o aplicativo crie, leia, atualize e exclua as tarefas permitidas para um usuário, incluindo suas próprias tarefas e as compartilhadas. |



##<a name="permission-scope-scenarios"></a>Cenários de escopo de permissão
A seguir, alguns cenários de aplicativo usando os recursos `User` e `Group` e seus escopos necessários correspondentes. A tabela a seguir mostra os escopos de permissão necessários para que um aplicativo seja capaz de executar operações específicas. Observe que, em alguns casos, a capacidade do aplicativo de executar algumas operações dependerá de se o escopo de permissão é somente do aplicativo ou delegado, e, no caso de escopos de permissão delegada, dos privilégios do usuário conectado. 

###<a name="access-scenarios-using-the-user-resource-and-the-required-scopes"></a>Acessar cenários usando o recurso Usuário e os escopos obrigatórios

| **Tarefas do aplicativo envolvendo o Usuário**     |  **Escopos obrigatórios** | **Permissões** |
|:-------------------------------|:---------------------|:---------------|
| O aplicativo deseja ler as informações básicas de outros usuários (somente o nome para exibição e a imagem), por exemplo, para mostrar uma experiência de seleção de pessoas     | _User.ReadBasic.All_  |  Ler os perfis básicos de todos usuários |
| O aplicativo deseja ler o perfil completo do usuário de um usuário conectado (ver subordinados diretos, gerente etc.)     | _User.Read_ | Habilitar entrada e ler o perfil de usuário|
| O aplicativo deseja ler o perfil completo de todos os usuários     | _User.Read.All_ |  Ler os perfis completos de todos os usuários   |
| O aplicativo deseja ler informações de arquivos, email e calendário do usuário conectado     | _User.Read_, _Files.Read_, _Mail.Read_, _Calendars.Read_ | Habilitar entrada e ler o perfil de usuário, ler arquivos dos usuários, ler email do usuário, ler calendários do usuário |
| O aplicativo deseja ler os arquivos dos usuários (meus) conectados e os arquivos que outros usuários compartilharam com o usuário conectado (eu). | _User.Read_, _Files.Read_, _Sites.Read.All_ | Habilitar entrada e ler o perfil de usuário, ler arquivos dos usuários, ler itens em todos os conjuntos de sites |
| O aplicativo deseja ler e gravar o perfil completo do usuário conectado     | _User.ReadWrite_ | Acesso de leitura e gravação ao perfil de usuário |
| O aplicativo deseja ler e gravar o perfil completo de todos os usuários     | _User.ReadWrite.All_ | Ler e gravar os perfis completos de todos os usuários |
| O aplicativo deseja ler e gravar informações de arquivos, de email e de calendário do usuário conectado     | _User.ReadWrite_, _Files.ReadWrite_, _Mail.ReadWrite_, _Calendars.ReadWrite_  |  Acesso de leitura e gravação ao perfil de usuário, acesso de leitura e gravação ao perfil de usuário, acesso de leitura e gravação ao email do usuário, acesso total a calendários do usuário |
   

###<a name="access-scenarios-using-the-group-resource-and-the-required-scopes"></a>Acessar cenários usando o recurso Grupo e os escopos obrigatórios
    
| **Tarefas do aplicativo envolvendo o Grupo**     |  **Escopos obrigatórios** |  **Permissões** |
|:-------------------------------|:---------------------|:---------------|
| O aplicativo deseja ler as informações básicas do grupo (somente o nome para exibição e a imagem), por exemplo, para mostrar uma experiência de seleção de um grupo     | _Group.Read.All_  | Ler todos os grupos|
| O aplicativo deseja ler todo o conteúdo em todos os grupos do Office 365, incluindo arquivos, conversas.  Também precisa mostrar associações de grupo, ser capaz de atualizar associações de grupo (caso seja o proprietário).  |  _Group.Read.All_ | Ler itens em todos os conjuntos de sites, ler todos os grupos|
| O aplicativo deseja ler e gravar todo o conteúdo em todos os grupos do Office 365, incluindo arquivos, conversas.  Também precisa mostrar associações de grupo, ser capaz de atualizar associações de grupo (caso seja o proprietário).  |     _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  Ler e gravar todos os grupos, editar ou excluir itens em todos os conjuntos de sites |
| O aplicativo deseja descobrir (localizar) um grupo do Office 365. Permite ao usuário procurar um grupo específico e escolher um deles na lista enumerada para ingressar no grupo.     | _Group.ReadWrite.All_ | Ler e gravar todos os grupos|
| O aplicativo deseja criar um grupo por meio do AAD Graph |     _Group.ReadWrite.All_ | Ler e gravar todos os grupos|
 


