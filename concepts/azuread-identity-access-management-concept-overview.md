# <a name="azure-ad-identity-and-access-management-api-overview"></a>Visão geral da API de gerenciamento de identidade e acesso do Azure AD

O Active Directory do Azure (Azure AD) ajuda a centralizar o gerenciamento de identidade e acesso para permitir acesso seguro e produtivo entre aplicativos, dispositivos, serviços e infraestrutura. As organizações podem usar o Azure AD para gerenciar identidades e controlar o acesso em ambientes locais, híbridos e em nuvem.  

Você pode usar as APIs REST do Azure AD no Microsoft Graph para criar fluxos de trabalho exclusivos entre os [recursos](../api-reference/v1.0/resources/azure_ad_overview.md) do Azure AD e serviços de terceiros.

## <a name="why-use-the-azure-ad-apis"></a>Por que usar as APIs do Azure AD?

Mais de 15 milhões de organizações usam o Azure AD ao se inscreverem em serviços em nuvem da Microsoft, como o Office 365, Microsoft Azure, Enterprise Mobility Suite ou Microsoft 365.  

Os desenvolvedores corporativos usam o Microsoft Graph para integrar o gerenciamento de identidades do Azure AD e outros serviços para automatizar fluxos de trabalho administrativos, como a integração (e rescisão) de funcionários, a manutenção de perfis, a implantação de licenças e muito mais.

Para muitos desenvolvedores corporativos, o Microsoft Graph e o Azure AD ajudam a "elevar e deslocar" os aplicativos existentes para a nuvem, acelerando a transformação digital de uma organização. Você pode aproveitar os recursos do Azure AD para adicionar mecanismos de controle de acesso a aplicativos, incluindo a verificação de associação de grupo, a função de diretório ou a associação de unidades administrativas de um usuário.

Você pode usar o Microsoft Graph e o Azure AD como uma maneira rápida e fácil de alcançar mais de 15 milhões de organizações, incluindo 90% das empresas da Fortune 500 que já usam os serviços do Azure AD. Os aplicativos integrados apresentam experiências de logon sem interrupções e podem usar dados organizacionais existentes para criar experiências personalizadas.  

Você pode usar as APIs do Azure AD no Microsoft Graph para consultar o perfil do usuário, encontrar outros usuários, gerenciar relações organizacionais, rastrear atribuições ou criar soluções originais que incorporem dados organizacionais existentes. Essas APIs fornecem uma base sólida para integrar aplicativos de negócios personalizados aos serviços digitais existentes de uma organização.

### <a name="access-users-and-groups"></a>Acessar usuários e grupos

Você pode usar as APIs do Azure AD no Microsoft Graph para:

- Pesquisar e gerenciar informações de [perfil de usuário](../api-reference/v1.0/resources/user.md), como nome, foto, endereço de email, cargo, localização do escritório e muito mais de usuários na sua organização.
- Criar [grupos](../api-reference/v1.0/resources/groups-overview.md) para projetos e equipes na sua organização. Adicionar e remover membros do grupo para controlar o acesso aos recursos. (Os grupos dinâmicos podem alterar automaticamente a associação com base nos valores da propriedade do usuário).
- Para controlar o acesso, você pode verificar a [associação transitiva](../api-reference/v1.0/api/user_checkmembergroups.md) em uma lista de grupos ou obter todos os recursos de um tipo especificado (como um usuário ou grupo) de uma lista de [IDs de recursos genéricos](../api-reference/v1.0/api/directoryobject_getbyids.md).

### <a name="manage-directory-roles"></a>Gerenciar funções de diretório

Você pode atribuir usuários a [funções de diretório](../api-reference/v1.0/resources/directoryrole.md) administrativas predefinidas do Azure AD, que concede permissão para executar tarefas específicas.

### <a name="manage-devices"></a>Gerenciar dispositivos

[Gerencie os dispositivos](https://docs.microsoft.com/pt-BR/azure/active-directory/device-management-introduction.md) registrados na organização. Os dispositivos são registrados a usuários e incluem itens como laptops, computadores desktop e celulares. Os dispositivos são em geral criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Microsoft Intune. Eles são utilizados por políticas de acesso condicional para a autenticação multifator.

### <a name="partner-tenant-management"></a>Gerenciamento de locatário do parceiro

Os parceiros da Microsoft que revendem e gerenciam o Microsoft Online Services (como o Office 365, o Microsoft Azure e o CRM Online) podem exibir os [locatários da organização](../api-reference/v1.0/resources/contract.md) que eles gerenciam atualmente.

Você também pode [gerenciar domínios](../api-reference/v1.0/resources/domain.md) associados a um locatário. As operações de domínio permitem que os parceiros da Microsoft automatizem o registro de domínio para serviços como o Office 365.

### <a name="tenant-management"></a>Gerenciamento de locatários

As APIs do Azure AD para o gerenciamento de locatários permitem:

- Obter informações sobre uma [organização](../api-reference/v1.0/resources/organization.md), como seu endereço comercial, contatos de notificação e técnicos, assinaturas de serviço ativas e os domínios associados a ela.
- Obter informações sobre [SKUs do serviço](../api-reference/v1.0/resources/subscribedsku.md) nos quais a empresa está inscrita.
- [Convidar usuários externos](../api-reference/v1.0/resources/invitation.md) (convidados) para uma organização.

### <a name="monitor-identity-protection-risks-preview"></a>Monitorar os riscos de proteção de identidade (prévia)

Recuperar eventos de risco gerados pela [Proteção de Identidade](../api-reference/beta/resources/identityprotection_root.md) do Azure AD, como o tipo do evento de risco, a gravidade, a data, o horário, o local, os usuários afetados e muito mais. A Proteção de Identidade é oferecida no Azure AD Premium P2.

### <a name="activate-users-into-privileged-roles-preview"></a>Ativar usuários em funções privilegiadas (prévia)

Você pode garantir o acesso a recursos ativando privilégios administrativos sob demanda. O [Gerenciamento de Identidade Privilegiada](../api-reference/beta/resources/privilegedidentitymanagement_root.md) é oferecido no Azure AD Premium P2.


## <a name="next-steps"></a>Próximas etapas

- Saiba como [Usar as APIs REST do Azure AD](../api-reference/v1.0/resources/azure_ad_overview.md).
- Use o Azure AD para se [autenticar](auth_overview.md) no Microsoft Graph. 
- Integre o [logon do Azure AD](https://azure.microsoft.com/pt-BR/develop/identity/signin/) ao seu aplicativo ou website.
- Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.
- Explore [exemplos](https://developer.microsoft.com/pt-BR/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.
