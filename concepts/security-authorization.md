---
title: Autorização e API de Segurança do Microsoft Graph
description: Os dados de segurança acessíveis por meio da API de Segurança do Microsoft Graph são confidenciais e protegidos por permissões e funções do Azure AD (Azure Active Directory).
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 3064f5f905503f4406f01dba0b34e243c443dafe81c4db8567c86e875abfd4e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54233641"
---
# <a name="authorization-and-the-microsoft-graph-security-api"></a>Autorização e API de Segurança do Microsoft Graph

Os dados de segurança acessíveis por meio da API de Segurança do Microsoft Graph são confidenciais e protegidos por permissões e funções do Azure AD (Azure Active Directory).

A API de Segurança do Microsoft Graph dá suporte a dois tipos de autorização:

- **Autorização no nível de aplicativo** - não há usuário conectado (por exemplo, um cenário SIEM). As permissões concedidas ao aplicativo determinam a autorização. 
    >**Observação:** Esta opção também pode suportar casos em que o RBAC (controle de acesso baseado em função) é gerenciado pelo aplicativo.
- **Autorização delegada pelo usuário** - um usuário que é um membro do locatário do Microsoft Azure AD está conectado. O usuário deve ser um membro de uma função limitada de Administrador do Microsoft Azure AD: ou Leitor de Segurança ou Administrador de Segurança, além de ter dado as permissões necessárias ao aplicativo.

Se você estiver chamando a API de Segurança do Microsoft Graph no Explorador do Graph:

- O administrador do locatário do Microsoft Azure AD deve conceder explicitamente o consentimento das permissões solicitadas ao aplicativo do Explorador do Graph.
- O usuário deve ser um membro da função administrador limitado do leitor de segurança no Microsoft Azure AD (leitor de segurança ou administrador de segurança).

>**Observação**: O Explorador do Graph não suporta autorização no nível de aplicativo.

Se você estiver chamando a API de Segurança do Microsoft Graph de um aplicativo personalizado ou do seu próprio:

- O administrador de locatário do Microsoft Azure AD deve conceder explicitamente o consentimento para o aplicativo. Isso é necessário para autorização no nível de aplicativo e autorização delegada pelo usuário.
- Se você estiver usando autorização delegada do usuário, o usuário deverá ser membro da função Administrador Limitado do Leitor de Segurança ou administrador de segurança no Microsoft Azure AD.

## <a name="manage-authorization-in-security-api-client-applications"></a>Gerenciar autorizações nos aplicativos de clientes de API de segurança

Os dados de segurança fornecidos por meio da API de Segurança do Microsoft Graph são confidenciais e devem ser protegidos por mecanismos de autenticação e autorização apropriados. A tabela a seguir lista as etapas para registrar e criar um aplicativo cliente que pode acessar a API de Segurança do Microsoft Graph.

| **Quem** | **Ação** |
|:---------------------|:------------------|
|Desenvolvedor ou proprietário do aplicativo|Registar o aplicativo como um aplicativo de empresa.|
|Administrador de locatários|Conceda permissões para o aplicativo.|
|Administrador de locatários|Atribuir funções aos usuários.|
|Desenvolvedor do aplicativo|Entre como usuário e use o aplicativo para acessar a API de Segurança do Microsoft Graph.|

O registro do aplicativo define somente quais permissões o mesmo precisa para ser executado. Ele NÃO concede estas permissões ao aplicativo.

O administrador de locatários do Microsoft Azure AD tem que conceder explicitamente a permissão ao aplicativo. Isso precisa ser feito por locatário e tem que ser *executado sempre que* as permissões do aplicativo forem alteradas no portal de registro do aplicativo.

Por exemplo, suponha que você tenha um aplicativo, dois locatários do Microsoft Azure AD, **T1** e **T2**, e duas permissões **P1** e **P2**. O processo de autorização será assim:

- O aplicativo registra para exigir permissão **P1**.
- Quando os usuários no locatário **T1** recebem um token do Microsoft Azure AD para esse aplicativo, o token não contém nenhuma permissão.
- O administrador de locatários do Microsoft Azure AD **T1** concede permissões explicitamente para o aplicativo. Quando os usuários no locatário **T1** recebem um token do Microsoft Azure AD para o aplicativo, ele contém a permissão **P1**.
- Quando os usuários no locatário **T2** recebem um token do Microsoft Azure AD para o aplicativo, o token não contém nenhuma permissão - porque o administrador de locatários **T2** ainda não concedeu permissões ao aplicativo. A permissão deve ser concedida *por locatário* e *por aplicativo*.
- O aplicativo agora tem seu registro alterado para requerer as permissões **P1** e **P2**.
- Quando os usuários no locatário **T1** recebem um token do Microsoft Azure AD para o aplicativo, ele contém apenas a permissão **P1**. As permissões concedidas a um aplicativo são registradas como instantâneos do que foi a elas concedido - as mesmas *não são alteradas automaticamente* depois que o registro do aplicativo (permissão) é alterado.
- O administrador de locatários **T2** concede as permissões **P1** e **P2** do aplicativo. Agora, quando os usuários no locatário **T2** recebem um token do Microsoft Azure AD para o aplicativo, ele contém as permissões **P1** e **P2**.

>**Observação**: Os tokens do Microsoft Azure AD para os aplicativos no locatário **T1** e no locatário **T2** contêm permissões distintas, porque cada administrador de locatário concedeu permissões diferentes ao aplicativo.

- Para que o aplicativo funcione novamente no locatário **T1**, o administrador de locatários **T1** deve conceder explicitamente as permissões **P1** e **P2** ao aplicativo.

## <a name="register-an-application-with-the-microsoft-identity-platform-endpoint"></a>Registrar um aplicativo com o ponto de extremidade da plataforma de identidade da Microsoft 

Para registrar um aplicativo com o ponto de extremidade da plataforma de identidade da Microsoft, você precisará:

- **Nome do aplicativo** - uma cadeia de caracteres usada para o nome do aplicativo.
- **URL de redirecionamento** - o URL no qual a resposta de autenticação do Microsoft Azure AD é enviada. Para começar, você pode usar a homepage do aplicativo Web do cliente de teste.
- **Permissões necessárias** - As permissões que seu aplicativo requer para poder chamar o Microsoft Graph.

Para registrar seu aplicativo:

1. Vá para o [portal de registro do aplicativo Azure](https://go.microsoft.com/fwlink/?linkid=2083908) e conecte-se.
    >**Observação**: não é necessário ser um administrador de locatários. Você será redirecionado para a lista **Meus aplicativos**.
2. Selecione **Novo registro**.
3. Na página de registro do novo aplicativo, digite um valor para **Nome** e selecione os tipos de conta aos quais deseja dar suporte. No campo **URI de redirecionamento**, insira o URL de redirecionamento.
4. Selecione **Registrar** para criar o aplicativo e exibir a respectiva página de visão geral. *
5. Acesse a página **permissões de API** do aplicativo.
6. Selecione **Adicionar uma permissão** e selecione **Microsoft Graph** no submenu. Selecione **Permissões delegadas**. Use a caixa de pesquisa para localizar e selecionar as permissões necessárias. Para obter uma lista de permissões, consulte [Permissões de segurança](permissions-reference.md#security-permissions).

    >**Observação** A API de Segurança do Microsoft Graph requer o escopo *.Read.All para consultas GET, e o escopo *.ReadWrite.All para consultas PATCH/POST/DELETE.

    |Permissão | Entidade | Solicitações com suporte |
    |:----------|:-------|:-------------------|
    |SecurityActions.Read.All| &bull; [securityActions](/graph/api/resources/securityaction?view=graph-rest-beta) (visualização) | GET |
    |SecurityActions.ReadWrite.All| &bull; [securityActions](/graph/api/resources/securityaction?view=graph-rest-beta) (visualização) | GET, POST |
    |SecurityEvents.Read.All | &bull; [alerts](/graph/api/resources/alert?view=graph-rest-1.0)</br> &bull; [secureScores](/graph/api/resources/securescores?view=graph-rest-beta) </br> &bull; [secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta) | OBTER |
    |SecurityEvents.ReadWrite.All | &bull; [alerts](/graph/api/resources/alert?view=graph-rest-1.0)</br> &bull; [secureScores](/graph/api/resources/securescores?view=graph-rest-beta) </br> &bull; [secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta) | GET, POST, PATCH |
    |ThreatIndicators.ReadWrite.OwnedBy | &bull; [tiIndicator](/graph/api/resources/tiindicator?view=graph-rest-beta) (visualização) | GET, POST, PATCH, DELETE|

7. Selecione **Adicionar permissões**.

Salve as informações a seguir:

- ID do aplicativo (cliente)
- URL de redirecionamento
- Lista de permissões necessárias

\*A Proteção Avançada contra Ameaças do Windows Defender (WDATP) exige mais [funções de usuário](/windows/security/threat-protection/microsoft-defender-atp/user-roles) do que as necessárias para a API de Segurança do Microsoft Graph; portanto, somente os usuários nas funções do WDATP e da API de Segurança do Microsoft Graph podem ter acesso aos dados do WDATP.  A autenticação somente para aplicativos não é limitada por isso. Portanto, recomendamos que você use um token de autenticação somente para aplicativos.

Para obter mais informações, consulte [Registrar um aplicativo na Plataforma de Identidade da Microsoft](auth-register-app-v2.md).

## <a name="grant-permissions-to-an-application"></a>Conceder permissões a um aplicativo.

O registro do aplicativo define somente qual permissão o aplicativo requer - ele não concede essas permissões ao aplicativo. Um administrador de locatários do Microsoft Azure AD deve conceder explicitamente essas permissões, fazendo uma chamada para o ponto de extremidade de consentimento do administrador. Para detalhes, consulte [Usando o ponto de extremidade de consentimento do administrador](/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint).

Para conceder permissões a um aplicativo, você precisará:

- **ID do Aplicativo** – ID do aplicativo do portal de registro do aplicativo Azure.
- **URL de redirecionamento** – Cadeia de caracteres que você define no portal de registro do aplicativo para resposta de autenticação.

Para conceder as permissões:

- Em um editor de texto, crie a seguinte cadeia de caracteres de URL:

    `https://login.microsoftonline.com/common/adminconsent?client_id=<Application Id>&state=12345&redirect_uri=<Redirect URL>`

- Em um navegador Web, acesse este URL e faça login como administrador de locatários. A caixa de diálogo mostra a lista de permissões que o aplicativo requer, conforme especificado no portal de registro do aplicativo. Selecione **OK** para conceder ao aplicativo essas permissões.

> **Observação:** Esta etapa concede permissões ao aplicativo - não aos usuários. Isso significa que todos os usuários pertencentes ao locatário do Microsoft Azure AD que usam esse aplicativo receberão essas permissões, inclusive usuários não administradores.

## <a name="assign-azure-ad-roles-to-users"></a>Atribuir funções do Microsoft Azure AD aos usuários

Depois que um aplicativo receber permissões, todas as pessoas com acesso ao aplicativo (ou seja, membros do locatário do Azure AD) receberão as permissões concedidas. Para proteger ainda mais os dados confidenciais de segurança, a API de Segurança do Microsoft Graph também exige que os usuários recebam a função **Leitor de segurança** do Microsoft Azure AD. Para obter detalhes, confira [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles-azure-portal) e [Atribuir funções de administrador e não-administrador aos usuários com o Azure Active Directory](/azure/active-directory/active-directory-users-assign-role-azure-portal).

>**Observação:** Você precisa ser um administrador de locatários para executar esta etapa.

Para atribuir uma função a um usuário:

1. Entre no [portal do Azure](https://portal.azure.com) (https://portal.azure.com).
2. Clique no ícone no canto superior esquerdo para expandir o menu do portal do Azure. Selecione **Azure Active Directory** > **Usuários**.
3. Clique no nome do usuário.
4. Escolha **Funções atribuídas** e, em seguida, **Adicionar atribuição**.
5. Selecione **Leitor de segurança** e clique em **Adicionar**.

## <a name="create-an-authentication-code"></a>Crie um código de autenticação

Para criar um código de autenticação, você precisará de:

- **ID do Aplicativo** - a ID do aplicativo do portal de registro do aplicativo.
- **URL de redirecionamento** - o URL no qual a resposta de autenticação do Microsoft Azure AD é enviada. Para começar, você pode usar https://localhost ou a homepage do aplicativo Web do cliente de teste.
- **Chave do aplicativo** (opcional) - a chave do aplicativo. Isso se aplica quando você está desenvolvendo um aplicativo que usará somente o código de autenticação do aplicativo (ou seja, não oferecerá suporte à autenticação delegada pelo usuário).

A tabela a seguir lista os recursos que você pode usar para criar um código de autenticação.

|**Tipo de aplicativo**|**Biblioteca de autenticação**|
|------------------------|----------------------------|
|[Aplicativos da área de trabalho, iOS](/azure/active-directory/develop/guidedsetups/active-directory-ios)|[MSAL.framework: Visualização da Biblioteca de Autenticação da Microsoft para iOS](https://github.com/AzureAD/microsoft-authentication-library-for-objc)|
|[Aplicativos da área de trabalho - Android](/azure/active-directory/develop/guidedsetups/active-directory-android)|[Biblioteca de Autenticação Microsoft (MSAL)](https://javadoc.io/doc/com.microsoft.identity.client/msal)|
|[Aplicativos da área de trabalho - .Net](/azure/active-directory/develop/guidedsetups/active-directory-windesktop)|[Biblioteca de Autenticação Microsoft (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client)|
|[Aplicativos Web - JavaScript SPA](/azure/active-directory/develop/guidedsetups/active-directory-javascriptspa)|[Biblioteca de autenticação da Microsoft para visualização de JavaScript](https://github.com/AzureAD/microsoft-authentication-library-for-js)|
|[Aplicativos Web - Servidor Web .NET](/azure/active-directory/develop/guidedsetups/active-directory-aspnetwebapp)|OpenIdConnection, Cookies, SystemWeb|
|[Aplicativos Web - Aplicativo da Web NodeJS](/azure/active-directory/develop/active-directory-v2-devquickstarts-node-web)||

Para aplicativos que não usam nenhuma das bibliotecas existentes, consulte [Obter acesso em nome de um usuário](auth-v2-user.md).

1. Obter um código do Microsoft Azure AD. A consulta a ser chamada contém o parâmetro para a ID do aplicativo, o URL de redirecionamento e as **permissões necessárias**.
2. Use o código para obter um token de acesso.

Se você usa a biblioteca OpenId Connect, consulte [Autenticar usando o Microsoft Azure AD e OpenID Connect](/azure/architecture/multitenant-identity/authenticate) e ligar`app.UseOpenIdConnectAuthentication()`.

>**Observação:** Se você estiver solicitando tokens de autenticação delegada pelo usuário, o parâmetro da biblioteca será **Escopos solicitados**. Use o User.Read para este parâmetro ao invés do que o aplicativo registrado solicitar. O parâmetro **Escopos solicitados** NÃO afeta as permissões contidas nos tokens de autenticação retornados. Estes são determinados pelas permissões que o administrador de locatários concedeu ao aplicativo.

Por exemplo, se você estiver usando a biblioteca MSAL do .NET, chame o seguinte:

`var accessToken = (await client.AcquireTokenAsync(scopes)).AccessToken;`

>**Observação:** Este exemplo deve usar a permissão menos privilegiada, como User.Read. No entanto, o token de acesso retornado pode conter permissões que foram concedidas pelo administrador locatário para o locatário do usuário atual, como User.Read.All ou User.ReadWrite.All.

Um token (cadeia de caracteres) é retornado pelo Microsoft Azure AD que contém informações de autenticação e as permissões necessárias para o aplicativo. Atribua esse token ao cabeçalho HTTP como um token de portador, conforme mostrado no exemplo a seguir.

`request.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);`

O Microsoft Graph validará as informações contidas nesse token e concederá ou rejeitará o acesso.

Para visualizar as declarações contidas no token retornado, use a biblioteca do NuGet System.IdentityModel.Tokens.Jwt.

`JwtSecurityTokenHandler tokenHandler = new JwtSecurityTokenHandler();`</br>
`var securityToken = tokenHandler.ReadToken(accessToken) as JwtSecurityToken;`

A resposta do Microsoft Graph contém um cabeçalho chamado client-request-id, que é um GUID. Se o acesso for negado, especifique esse GUID ao procurar suporte na [Microsoft Tech Community](https://techcommunity.microsoft.com/t5/Microsoft-Graph-Security-API/ct-p/SecurityGraphAPI), para que possamos ajudar a investigar a causa dessa falha de autenticação.