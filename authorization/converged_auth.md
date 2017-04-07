# <a name="authenticate-microsoft-graph-apps-with-the-azure-ad-v20-endpoint"></a>Autenticar aplicativos do Microsoft Graph com o ponto de extremidade do Azure AD v2.0

> **Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>.  

> Para fornecer suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie os aplicativos usando o [Portal de Gerenciamento do Microsoft Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0](auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).


Ao usar o ponto de extremidade do Azure AD v2.0, você pode criar aplicativos que aceitem identidades corporativas e de estudante (Azure Active Directory), bem como pessoais (conta da Microsoft).

Antigamente, se você quisesse desenvolver um aplicativo que desse suporte tanto a contas da Microsoft quanto ao Azure Active Directory, tinha que integrar dois sistemas diferentes. Usando o ponto de extremidade do Azure AD v2.0, você pode agora dar suporte a dois tipos de contas com uma única integração: um processo simples para alcançar um público que abrange milhões de usuários com contas pessoais e corporativas ou de estudante.  

Depois que você integra os aplicativos com o ponto de extremidade do Azure AD v2.0, eles podem acessar instantaneamente os pontos de extremidade do Microsoft Graph disponíveis para contas pessoais e corporativas ou de estudante, como: 

| Dados              | Ponto de extremidade                                       |
|:------------------|:-----------------------------------------------|
| Perfil de usuário      | `https://graph.microsoft.com/v1.0/me`          |
| Email do Outlook      | `https://graph.microsoft.com/v1.0/me/messages` |
| Contatos do Outlook  | `https://graph.microsoft.com/v1.0/me/contacts` |
| Calendários do Outlook | `https://graph.microsoft.com/v1.0/me/events`   |
| OneDrive          | `https://graph.microsoft.com/v1.0/me/drive`    |

 >**Observação:** Alguns pontos de extremidade do Microsoft Graph, como grupos e tarefas, não são aplicáveis a contas pessoais.  

## <a name="microsoft-graph-authentication-scopes"></a>Escopos de autenticação do Microsoft Graph

O ponto de extremidade do Azure AD v2.0 dá suporte a todos os escopos de permissão listados nos [Escopos de permissão do Microsoft Graph](permission_scopes.md). 

Para saber mais sobre como usar escopos com o ponto de extremidade do Azure AD v2.0 e como ele difere do uso de recursos no Azure AD, confira <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#scopes-not-resources" target="_newtab">Escopos, não recursos</a>.

## <a name="see-it-in-action"></a>Veja isso em ação

O [Exemplos de conexão no repositório do Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) fornece exemplos simples de como autenticar usuários e conectar-se ao Microsoft Graph em uma ampla gama de plataformas.

Além disso, a seção [Introdução](http://developer.microsoft.com/en-us/graph/docs/platform/get-started) contém artigos que descrevem como criar esses exemplos de aplicativo, incluindo as bibliotecas de autenticação usadas em cada plataforma.

## <a name="see-also"></a>Ver também

- [Registrar um aplicativo com o ponto de extremidade do Azure AD v2.0](auth_register_app_v2.md)
- [Autenticação de aplicativo com o Microsoft Graph](auth_overview.md)
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare" target="_newtab">Novidades sobre o modelo do Azure AD v2.0</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/" target="_newtab">Devo usar o ponto de extremidade do Azure AD v2.0?</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/?product=active-directory&term=azure+ad+v2.0" target="_newtab">Documentação do ponto de extremidade do Azure AD v2.0 no Azure.com</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-app-registration/#build-a-quick-start-app" target="_newtab">Inícios rápidos do código do Azure AD v2.0 no Azure.com</a>

