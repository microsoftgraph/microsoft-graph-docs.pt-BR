# <a name="intune-devices-and-apps-api-overview"></a>Visão geral da API de dispositivos e aplicativos do Intune

O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização. Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas. 

Se você for um ISV, também poderá usar a API do Intune para gerenciar locatários de clientes.

## <a name="why-integrate-with-intune"></a>Por que se integrar com o Intune?

Você pode usar a API do Intune no Microsoft Graph para acessar informações de dispositivos e aplicativos do Intune, gerenciar dispositivos, gerenciar aplicativos e automatizar o Intune.

### <a name="manage-devices"></a>Gerenciar dispositivos

Você pode usar a API do Intune para:

- Definir e impor políticas de [conformidade de dispositivos](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md), como a complexidade e a duração de senhas, a criptografia, os níveis de proteção de ameaças e assim por diante.  (As políticas permitidas variam de acordo com o sistema operacional e a versão).
- [Proteger os dados da empresa](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md), independentemente de a plataforma do dispositivo ser Windows, Android, Mac ou iOS.
- Criar e implantar políticas de [configuração de dispositivo](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md), incluindo o controle de versão/plataforma do sistema operacional, a associação a domínios e o gerenciamento de configurações.
- Criar e implantar políticas de [controle de acesso](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md) de dispositivo, incluído, downloads restritos, acesso a acessórios de rede e transferência de arquivos.
- Realizar [ações remotas](../api-reference/v1.0/resources/intune_devices_manageddevice.md), como localizar o dispositivo, alterar a senha e apagar o dispositivo.

### <a name="manage-apps"></a>Gerenciar aplicativos 

Você pode usar a API do Intune para executar as seguintes tarefas de gerenciamento de aplicativos:

- Implantar [aplicativos em dispositivos](../api-reference/v1.0/resources/intune_apps_mobileapp.md) ou impedir que aplicativos sejam implantados.
- Gerenciar o acesso a [livros eletrônicos](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md) e serviços relacionados.
- Definir e implantar configurações de aplicativos, configurações de proteção de aplicativos e políticas de uso de aplicativos.

### <a name="automate-intune"></a>Automatizar o Intune

Automatize o Intune usando a API do Intune para:

- Definir e atribuir controles de acesso [por função](../api-reference/v1.0/resources/intune_rbac_conceptual.md).
- Auditar e reportar conformidade, uso e acesso.
- Gerenciar [despesas de telecomunicações](../api-reference/v1.0/resources/intune_tem_conceptual.md).


## <a name="next-steps"></a>Próximas etapas

- [Usar o Azure AD para acessar a API do Intune](https://docs.microsoft.com/intune/intune-graph-apis).
- Veja como realizar tarefas comuns usando os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples).
- Saiba como [usar a API REST do Intune](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/intune_graph_overview).
- Confira o [log de alterações](changelog.md) para obter informações sobre as novidades na API do Intune.
- Explore [exemplos](https://developer.microsoft.com/en-us/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.
