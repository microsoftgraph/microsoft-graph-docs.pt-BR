# <a name="working-with-intune-in-microsoft-graph"></a>Trabalhando com o Intune no Microsoft Graph  

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/pt-BR/cloud-platform/microsoft-intune-pricing) pelo cliente.

A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.  

Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](https://docs.microsoft.com/pt-BR/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune. 

## <a name="using-the-intune-graph-api"></a>Uso da API do Graph para Intune

O Intune fornece dados para a API da Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com valiosas informações sobre entidades e navegação de relacionamentos.  Use a API do Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados com serviços variados para profissionais de TI ou usuários finais.     

Veja um exemplo de como determinar se um aplicativo está instalado no dispositivo de um usuário: 

1. Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário: 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. Em seguida, exiba a lista de aplicativos do seu locatário: 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a>Usar escopos de permissão

A API do Microsoft Graph controla o acesso a recursos por meio de escopos de permissão. Como desenvolvedor, você deve especificar os escopos de permissão necessários para acessar os recursos do Intune. Normalmente, você deve especificar os escopos de permissão necessários no portal do Azure Active Directory. Para saber mais, veja [Escopos de permissão do Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/docs/authorization/permission_scopes) e [Escopos de permissão do Intune](https://developer.microsoft.com/pt-BR/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).

