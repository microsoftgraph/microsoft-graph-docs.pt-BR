---
title: Chamar o Microsoft Graph por um Provedor de Soluções na Nuvem
description: Este tópico descreve como habilitar o acesso do aplicativo aos dados do cliente gerenciados por parceiros através do Microsoft Graph usando o fluxo de concessão do código de autorização ou o fluxo de credenciais do cliente de serviços.
author: jackson-woods
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 4817c905f5283a1b248d38d9a1910e9a52db18c6
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296230"
---
# <a name="call-microsoft-graph-from-a-cloud-solution-provider-application"></a>Chamar o Microsoft Graph por um Provedor de Soluções na Nuvem

> **Observação:** Este tópico se aplica **somente** a desenvolvedores de aplicativos do Provedor de Soluções na Nuvem (CSP) da Microsoft. O programa [Provedor de Soluções na Nuvem (CSP) da Microsoft](https://partner.microsoft.com/cloud-solution-provider) permite que os parceiros da Microsoft revendam e gerenciem os serviços online da Microsoft para os clientes.

Este tópico descreve como habilitar o acesso do aplicativo aos dados do cliente gerenciados por parceiros através do Microsoft Graph usando o [fluxo de concessão do código de autorização](/azure/active-directory/develop/active-directory-protocols-oauth-code) ou o [fluxo de credenciais do cliente de serviços](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service).

**Importante:** Chamar o Microsoft Graph a partir de um aplicativo CSP só é compatível com recursos de diretório (como **usuário**, **grupo**, **dispositivo**, **organização**) e recursos do [Intune](/graph/api/resources/intune-graph-overview).

## <a name="what-is-a-partner-managed-application"></a>O que é um aplicativo gerenciado por parceiros

O programa CSP permite que os parceiros da Microsoft revendam e gerenciem os Serviços Online da Microsoft (como o Microsoft 365, Microsoft Azure e CRM Online) para os clientes. O gerenciamento do atendimento ao cliente é feito por meio de Privilégios de Administrador Delegados e isso permite que os usuários de parceiros designados (conhecidos como agentes) acessem e configurem os ambientes de seus clientes.

Além disso, como desenvolvedor do parceiro, você pode criar um **aplicativo gerenciado por parceiros** para gerenciar os serviços da Microsoft de seus clientes. Os aplicativos gerenciados por parceiros são frequentemente chamados de *aplicativos pré-consentidos* porque todos os seus clientes são automaticamente pré-autorizados a utilizar os aplicativos gerenciados por parceiros. Isso significa que, quando um usuário de um dos locatários do cliente usa um de seus aplicativos gerenciados por parceiros, o usuário pode usá-lo sem ser solicitado a dar consentimento. Os aplicativos gerenciados por parceiros também herdam os Privilégios de Administrador Delegados para que os agentes do parceiro também possam obter acesso privilegiado aos clientes através do aplicativo gerenciado por parceiros.

## <a name="how-to-set-up-a-partner-managed-application"></a>Como configurar um aplicativo gerenciado por parceiros

Um aplicativo é exibido como *gerenciado por parceiros* quando recebe permissões elevadas para acessar dados de seus clientes.

> **Observação:** Aplicativos gerenciados por parceiros podem *somente* ser configurados em locatários de Parceiro para gerenciar recursos de locatário do cliente, aplicativos gerenciados por parceiros **devem** ser configurados como **locatários de vários aplicativos**.

### <a name="register-and-configure-a-multi-tenant-app"></a>Registrar e configurar um aplicativo de vários locatários

As etapas iniciais exigidas aqui seguem quase as mesmas etapas usadas para registrar e configurar um aplicativo multilocatário:

1. [Registre seu aplicativo](/azure/active-directory/active-directory-app-registration) no Locatário do parceiro usando o [Portal do Azure](https://portal.azure.com). Para funcionar como um aplicativo gerenciado por parceiros, o aplicativo deve ser configurado como um [aplicativo multilocatário](/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant). Além disso, se o aplicativo for implantado e vendido em diversas regiões geográficas, você precisará registrar seu aplicativo em cada uma dessas regiões conforme descrito <a href="#region">aqui</a>.
2. Configure seu aplicativo multilocatário, novamente através do Portal do Azure, com as *permissões exigidas* necessárias usando uma abordagem menos privilegiada.

### <a name="pre-consent-your-app-for-all-your-customers"></a>Consentimento prévio de seu aplicativo para todos os seus clientes

Por fim, conceda ao seu aplicativo gerenciado por parceiro essas permissões configuradas para todos os seus clientes. Você pode fazer isso adicionando o **servicePrincipal** que representa o aplicativo ao grupo *Adminagents* em seu locatário de parceiro, usando [Azure AD powershell V2](https://www.powershellgallery.com/packages/AzureAD) ou [Microsoft Graph PowerShell](/powershell/microsoftgraph/installation). Siga estas etapas para localizar o grupo *Adminagents*, o **servicePrincipal** e adicioná-lo ao grupo.

# <a name="azure-ad-powershell"></a>[Azure AD PowerShell](#tab/azuread)

1. Abra uma sessão do PowerShell e conecte-se ao locatário do parceiro digitando suas credenciais de administrador na janela de entrada.

    ```PowerShell
    Connect-AzureAd
    ```

2. Localize o grupo que representa os *Adminagents*.

    ```PowerShell
    $group = Get-AzureADGroup -Filter "displayName eq 'Adminagents'"
    ```

3. Encontrar a entidade de serviço que tenha a mesma *appId* do aplicativo.

    ```PowerShell
    $sp = Get-AzureADServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. Por fim, adicione a entidade de serviço ao grupo *Adminagents*.

    ```PowerShell
    Add-AzureADGroupMember -ObjectId $group.ObjectId -RefObjectId $sp.ObjectId
    ```

# <a name="microsoft-graph-powershell"></a>[Microsoft Graph PowerShell](#tab/graphpowershell)

1. Abra uma sessão do PowerShell e conecte-se ao locatário do parceiro digitando suas credenciais de administrador na janela de entrada.

    ```PowerShell
    Connect-MgGraph
    ```

2. Localize o grupo que representa os *Adminagents*.

    ```PowerShell
    $group = Get-MgGroup -Filter "displayName eq 'Adminagents'"
    ```

3. Encontrar a entidade de serviço que tenha a mesma *appId* do aplicativo.

    ```PowerShell
    $sp = Get-MgServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. Por fim, adicione a entidade de serviço ao grupo *Adminagents*.

    ```PowerShell
    New-MgGroupMember -GroupId $group.Id -DirectoryObjectId $sp.Id
    ```
----

## <a name="token-acquisition-flows"></a>Fluxos de aquisição do token

Os fluxos de aquisição de tokens de aplicativos gerenciados por parceiros, ou seja, o [fluxo de concessão do código de autorização](/azure/active-directory/develop/active-directory-protocols-oauth-code) e o [fluxo de credenciais de cliente de serviço a serviço](/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service), são os mesmos dos aplicativos multilocatário normais.

Além do acesso previamente consentido a todos os locatários do cliente, os aplicativos gerenciados por parceiros têm um recurso adicional. Esse recurso permite que os agentes usem seu aplicativo para acessar os dados de locatário de seus clientes (usando os privilégios de administrador delegados). Conceitualmente funciona da seguinte maneira:

1. Seu agente entra em seu aplicativo com suas credenciais de usuário emitidas no locatário do parceiro.
2. O aplicativo solicita um token de acesso para o locatário do cliente gerenciado por parceiros pretendido.
3. O aplicativo usa o token de acesso para chamar o Microsoft Graph.

Este é um [fluxo de concessão de código de autorização](/azure/active-directory/develop/active-directory-protocols-oauth-code) padrão, exceto que seus agentes precisam se conectar usando suas contas do parceiro. Para ver como isso ficaria, imagine que o locatário de seu parceiro fosse *parceiro.com* (que é o locatário principal de seus agentes) e um de seus clientes fosse *cliente.com*:

1. [Adquira um código de autorização:](/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code) Seu aplicativo faz uma solicitação para o ponto de extremidade ```/authorize``` e precisa usar um **locatário de cliente** em nosso exemplo ```customer.com```, para o locatário de destino. Seus agentes ainda se conectariam com a conta ```username@partner.com```.

    ```http
    GET https://login.microsoftonline.com/customer.com/oauth2/authorize
    ```

2. [Adquira um token de acesso usando o código de autorização:](/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token) seu aplicativo deve usar um **locatário do cliente** como o locatário de destino — no nosso exemplo, ```customer.com``` — ao fazer a solicitação para o ponto de extremidade ```token```:

    ```http
    POST https://login.microsoftonline.com/customer.com/oauth2/token
    ```

3. Agora que você tem um token de acesso, chame o Microsoft Graph colocando o token de acesso no cabeçalho de autorização HTTP:

    ```http
    GET https://graph.microsoft.com/beta/users
    Authorization: Bearer <token>
    ```

## <a name="register-your-app-in-the-regions-you-support"></a>Registre seu aplicativo nas regiões para as quais você oferece suporte
<a name="region"></a>

Atualmente, o contrato de cliente do CSP encontra-se limitado a uma única região. Os aplicativos gerenciados por parceiros têm a mesma limitação. Isso significa que você deve ter um locatário separado para cada região na qual venderá. Por exemplo, se seu aplicativo gerenciado por parceiros estiver registrado em um locatário nos EUA, mas seu cliente estiver na UE, o aplicativo gerenciado por parceiros não funcionará.  Cada um dos locatários de parceiros regionais deve manter seu próprio conjunto de aplicativos gerenciados por parceiros para gerenciar clientes dentro da mesma região. Isso pode exigir uma lógica adicional no aplicativo (antes de entrar) para obter o nome de usuário de entrada de seus clientes para decidir qual a identidade de aplicativos gerenciados por parceiros específica da região usar para atender o usuário.

## <a name="calling-microsoft-graph-immediately-after-customer-creation"></a>Chamar o Microsoft Graph imediatamente após a criação do cliente

Quando você cria um novo cliente usando a [API do Partner Center](https://partnercenter.microsoft.com/partner/developer), é criado um novo locatário do cliente. Além disso, uma relação de parceiro também é criada, que torna você o parceiro de registro deste novo locatário do cliente. Essa relação de parceiro pode levar até 3 minutos para ser propagada para o novo locatário do cliente. Se seu aplicativo chamar o Microsoft Graph logo após a criação, é provável que seu aplicativo receba um erro de acesso negado. Um atraso semelhante poderá ocorrer quando um cliente existente aceitar o convite. Isso ocorre porque o consentimento prévio depende da relação de parceiro estar presente no locatário do cliente.

Para evitar esse problema, recomendamos que seu aplicativo parceiro aguarde **três minutos** após a criação do cliente antes de chamar o Azure AD para adquirir um token (para chamar o Microsoft Graph). Isso deve abranger a maioria dos casos. No entanto, se depois de esperar três minutos você ainda receber um erro de autorização, aguarde mais 60 segundos e tente novamente.

> **Observação:** Na repetição, você deve adquirir um novo token de acesso do Azure AD antes de chamar o Microsoft Graph.  Não adiantará chamar o Microsoft Graph com o token de acesso que você já tem porque o token de acesso serve para uma hora e não conterá as declarações de permissão pré-autorizadas.
