---
title: Obtenha acesso sem um usuário
description: 'Alguns aplicativos chamam o Microsoft Graph com sua própria identidade e não em nome de um usuário. Em muitos casos, esses são os serviços em plano de fundo ou daemons que podem ser executados em um servidor sem a presença de um usuário conectado. Um exemplo de como um aplicativo pode ser um serviço de arquivamento de email que é ativado e executado durante a noite. Em alguns casos, aplicativos que tenham um usuário conectado no momento talvez precisem chamar o Microsoft Graph com sua própria identidade também. Por exemplo, um aplicativo talvez precise usar a funcionalidade que exige privilégios mais elevados em uma organização do que aqueles realizados pelo usuário conectado.  '
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca003bc10551c03dd781db05aad7170b799304b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977497"
---
# <a name="get-access-without-a-user"></a><span data-ttu-id="8a421-107">Obter acesso sem um usuário</span><span class="sxs-lookup"><span data-stu-id="8a421-107">Get access without a user</span></span>

<span data-ttu-id="8a421-p102">Alguns aplicativos chamam o Microsoft Graph com sua própria identidade e não em nome de um usuário. Em muitos casos, esses são os serviços em plano de fundo ou daemons que podem ser executados em um servidor sem a presença de um usuário conectado. Um exemplo de como um aplicativo pode ser um serviço de arquivamento de email que é ativado e executado durante a noite. Em alguns casos, aplicativos que tenham um usuário conectado no momento talvez precisem chamar o Microsoft Graph com sua própria identidade também. Por exemplo, um aplicativo talvez precise usar a funcionalidade que exige privilégios mais elevados em uma organização do que aqueles realizados pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8a421-p102">Some apps call Microsoft Graph with their own identity and not on behalf of a user. In many cases, these are background services or daemons that run on a server without the presence of a signed-in user. An example of such an app might be an email archival service that wakes up and runs overnight. In some cases, apps that have a signed-in user present may also need to call Microsoft Graph under their own identity. For example, an app may need to use functionality that requires more elevated privileges in an organization than those carried by the signed-in user.</span></span>  

<span data-ttu-id="8a421-p103">Os aplicativos que chamam o Microsoft Graph com sua própria identidade usam o fluxo de concessão de credenciais do cliente OAuth 2.0 para obter tokens de acesso do Azure AD. Neste tópico, vamos orientá-lo pelas etapas básicas para configurar um serviço e usar o fluxo de concessão de credenciais do cliente OAuth para obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="8a421-p103">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 client credentials grant flow to get access tokens from Azure AD. In this topic, we will walk through the basic steps to configure a service and use the OAuth client credentials grant flow to get an access token.</span></span> 

## <a name="authentication-and-authorization-steps"></a><span data-ttu-id="8a421-115">Etapas de autenticação e autorização</span><span class="sxs-lookup"><span data-stu-id="8a421-115">Authentication and authorization steps</span></span>

<span data-ttu-id="8a421-116">As etapas básicas necessárias para configurar um serviço e obter um token para o ponto de extremidade do Azure AD v2.0 que seu serviço pode usar para fazer chamadas para o Microsoft Graph com sua própria identidade são:</span><span class="sxs-lookup"><span data-stu-id="8a421-116">The basic steps required to configure a service and get a token from the Azure AD v2.0 endpoint that your service can use to call Microsoft Graph under its own identity are:</span></span>

1. <span data-ttu-id="8a421-117">Registre seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a421-117">Register your app.</span></span>
2. <span data-ttu-id="8a421-118">Configure permissões para o Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a421-118">Configure permissions for Microsoft Graph on your app.</span></span>
3. <span data-ttu-id="8a421-119">Obtenha o consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="8a421-119">Get administrator consent.</span></span>
4. <span data-ttu-id="8a421-120">Obtenha um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="8a421-120">Get an access token.</span></span>
5. <span data-ttu-id="8a421-121">Use o token de acesso para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8a421-121">Use the access token to call Microsoft Graph.</span></span>

## <a name="1-register-your-app"></a><span data-ttu-id="8a421-122">1. Registre seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a421-122">1. Register your app</span></span>

<span data-ttu-id="8a421-p104">Para autenticar com o ponto de extremidade do Azure v2.0, primeiro você deve registrar seu aplicativo no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/). Você pode usar uma conta da Microsoft ou uma conta corporativa ou de estudante para registrar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a421-p104">To authenticate with the Azure v2.0 endpoint, you must first register your app at the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/). You can use either a Microsoft account or a work or school account to register your app.</span></span> 

<span data-ttu-id="8a421-p105">A captura de tela a seguir mostra um registro do aplicativo Web que foi configurado para um serviço em segundo plano. ![Registro do aplicativo de serviço](./images/v2-service-registration.png)</span><span class="sxs-lookup"><span data-stu-id="8a421-p105">The following screenshot shows a web app registration that has been configured for a background service. ![Service app registration](./images/v2-service-registration.png)</span></span>

<span data-ttu-id="8a421-127">Para um serviço que chamará o Microsoft Graph com sua própria identidade, você precisa registrar seu aplicativo na plataforma Web e copiar os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="8a421-127">For a service that will call Microsoft Graph under its own identity, you need to register your app for the Web platform and copy the following values:</span></span>

- <span data-ttu-id="8a421-128">A ID do Aplicativo atribuída pelo portal de registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a421-128">The Application ID assigned by the app registration portal.</span></span>
- <span data-ttu-id="8a421-129">Um Segredo do Aplicativo, que pode ser uma senha ou um par de chaves públicas/particulares (certificado).</span><span class="sxs-lookup"><span data-stu-id="8a421-129">An Application Secret, either a password or a public/private key pair (certificate).</span></span>
- <span data-ttu-id="8a421-130">Uma URL de redirecionamento para seu serviço receber respostas do token do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a421-130">A Redirect URL for your service to receive token responses from Azure AD.</span></span>
- <span data-ttu-id="8a421-131">Uma URL de redirecionamento para seu serviço receber respostas de consentimento do administrador se seu aplicativo implementar a funcionalidade para solicitar o consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="8a421-131">A Redirect URL for your service to receive admin consent responses if your app implements functionality to request administrator consent.</span></span>  

<span data-ttu-id="8a421-132">Para obter etapas sobre como configurar um aplicativo usando o Portal de Registro de Aplicativos da Microsoft, confira [Registre seu aplicativo](./auth-register-app-v2.md).</span><span class="sxs-lookup"><span data-stu-id="8a421-132">For steps on how to configure an app using the Microsoft App Registration Portal, see [Register your app](./auth-register-app-v2.md).</span></span>

<span data-ttu-id="8a421-133">Com o fluxo de concessão de credenciais do cliente OAuth 2.0, o aplicativo se autentica diretamente no ponto de extremidade `/token` do Azure AD v2.0 usando a ID do Aplicativo atribuída pelo Azure AD e o Segredo do Aplicativo que você cria usando o portal.</span><span class="sxs-lookup"><span data-stu-id="8a421-133">With the OAuth 2.0 client credentials grant flow, your app authenticates directly at the Azure AD v2.0 `/token` endpoint using the Application ID assigned by Azure AD and the Application Secret that you create using the portal.</span></span> 

## <a name="2-configure-permissions-for-microsoft-graph"></a><span data-ttu-id="8a421-134">2. Configure permissões para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a421-134">2. Configure permissions for Microsoft Graph</span></span>

<span data-ttu-id="8a421-p106">Para aplicativos que chamam o Microsoft Graph com sua própria identidade, o Microsoft Graph expõe permissões do aplicativo. (O Microsoft Graph também expõe as permissões delegadas para aplicativos que chamam o Microsoft Graph em nome de um usuário.) Configure previamente as Permissões de aplicativo necessárias quando registrar o aplicativo. As Permissões de aplicativo sempre exigem o consentimento do administrador. Um administrador pode autorizar essas permissões usando o [Portal do Azure](https://portal.azure.com) quando o aplicativo for instalado em sua organização ou pode fornecer uma experiência de inscrição em seu aplicativo por meio da qual os administradores podem concordar com as permissões configuradas. Depois que o consentimento do administrador for registrado pelo Azure AD, seu aplicativo poderá solicitar tokens sem ter que solicitar consentimento novamente. Para obter mais informações sobre as permissões disponibilizadas pelo Microsoft Graph, confira a [Referência de permissões](./permissions-reference.md)</span><span class="sxs-lookup"><span data-stu-id="8a421-p106">For apps that call Microsoft Graph under their own identity, Microsoft Graph exposes application permissions. (Microsoft Graph also exposes delegated permissions for apps that call Microsoft Graph on behalf of a user.) You pre-configure the application permissions your app needs when you register your app. Application permissions always require administrator consent. An administrator can either consent to these permissions using the [Azure portal](https://portal.azure.com) when your app is installed in their organization, or you can provide a sign-up experience in your app through which administrators can consent to the permissions you configured. Once administrator consent is recorded by Azure AD, your app can request tokens without having to request consent again. For more detailed information about the permissions available with Microsoft Graph, see the [Permissions reference](./permissions-reference.md)</span></span>

<span data-ttu-id="8a421-141">Para configurar as Permissões de aplicativo para seu aplicativo no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/), em **Microsoft Graph**, escolha **Adicionar** ao lado de **Permissões de aplicativo** e, em seguida, escolha as permissões exigidas pelo aplicativo na caixa de diálogo **Selecionar Permissões**.</span><span class="sxs-lookup"><span data-stu-id="8a421-141">To configure application permissions for your app in the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/): under **Microsoft Graph**, choose **Add** next to **Application Permissions** and then select the permissions your app requires in the **Select Permissions** dialog.</span></span>

<span data-ttu-id="8a421-142">A captura de tela a seguir mostra a caixa de diálogo **Selecionar Permissões** para Permissões de aplicativo do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8a421-142">The following screenshot shows the **Select Permissions** dialog for Microsoft Graph application permissions.</span></span> 

![Marque a caixa de diálogo Permissões para as Permissões de aplicativo do Microsoft Graph.](./images/v2-application-permissions.png)

> <span data-ttu-id="8a421-p107">**Observação**: Recomendamos configurar o conjunto com menos privilégios de permissões necessárias para seu aplicativo. Isso proporciona uma experiência muito mais confortável para os administradores do que ter que consentir com uma longa lista de permissões.</span><span class="sxs-lookup"><span data-stu-id="8a421-p107">**Note**: We recommend configuring the least privileged set of permissions required by your app. This provides a much more comfortable experience for administrators than having to consent to a long list of permissions.</span></span>

## <a name="3-get-administrator-consent"></a><span data-ttu-id="8a421-146">3. Obtenha o consentimento do administrador</span><span class="sxs-lookup"><span data-stu-id="8a421-146">3. Get administrator consent</span></span>

<span data-ttu-id="8a421-147">Você pode confiar em um administrador para conceder as permissões que seu aplicativo precisa no [Portal do Azure](https://portal.azure.com). Entretanto, muitas vezes, a melhor opção seria fornecer uma experiência de inscrição para administradores usando o ponto de extremidade `/adminconsent` do Azure AD v2.0.</span><span class="sxs-lookup"><span data-stu-id="8a421-147">You can rely on an administrator to grant the permissions your app needs at the [Azure portal](https://portal.azure.com); however, often, a better option is to provide a sign-up experience for administrators by using the Azure AD v2.0 `/adminconsent` endpoint.</span></span> 

> <span data-ttu-id="8a421-148">**Importante**: Sempre que fizer uma alteração nas permissões configuradas, convém repetir o processo de Consentimento do Administrador.</span><span class="sxs-lookup"><span data-stu-id="8a421-148">**Important**: Any time you make a change to the configured permissions, you must also repeat the Admin Consent process.</span></span> <span data-ttu-id="8a421-149">As alterações feitas no portal de registro de aplicativos não serão refletidas até que o consentimento tiver sido reaplicado pelo administrador do locatário.</span><span class="sxs-lookup"><span data-stu-id="8a421-149">Changes made in the app registration portal will not be reflected until consent has been reapplied by the tenant's administrator.</span></span>

### <a name="request"></a><span data-ttu-id="8a421-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a421-150">Request</span></span>

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=https://localhost/myapp/permissions
```

| <span data-ttu-id="8a421-151">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a421-151">Parameter</span></span>     | <span data-ttu-id="8a421-152">Condição</span><span class="sxs-lookup"><span data-stu-id="8a421-152">Condition</span></span>   | <span data-ttu-id="8a421-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a421-153">Description</span></span> 
|:--------------|:------------|:------------
| <span data-ttu-id="8a421-154">locatário</span><span class="sxs-lookup"><span data-stu-id="8a421-154">tenant</span></span>        | <span data-ttu-id="8a421-155">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-155">Required</span></span>    | <span data-ttu-id="8a421-p109">O locatário do diretório do qual você deseja solicitar permissão. Pode ser no formato de nome amigável ou GUID. Se você não souber a qual locatário o usuário pertence e quiser permitir que ele entre em qualquer locatário, use `common`.</span><span class="sxs-lookup"><span data-stu-id="8a421-p109">The directory tenant that you want to request permission from. This can be in GUID or friendly name format. If you don't know which tenant the user belongs to and you want to let them sign in with any tenant, use `common`.</span></span> 
| <span data-ttu-id="8a421-159">client_id</span><span class="sxs-lookup"><span data-stu-id="8a421-159">client_id</span></span>     | <span data-ttu-id="8a421-160">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-160">Required</span></span>    | <span data-ttu-id="8a421-161">ID de Aplicativo que o [Portal de Registro de Aplicativos](https://apps.dev.microsoft.com/) atribuiu a seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a421-161">The Application ID that the [Application Registration Portal](https://apps.dev.microsoft.com/) assigned to your app.</span></span> 
| <span data-ttu-id="8a421-162">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="8a421-162">redirect_uri</span></span>  | <span data-ttu-id="8a421-163">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-163">Required</span></span>    | <span data-ttu-id="8a421-p110">O URI de redirecionamento para onde você deseja que a resposta seja enviada para que o aplicativo trate da situação. Ele deve corresponder exatamente a um dos URIs de redirecionamento registrados no portal, exceto que ele deve ser codificado por URL e pode ter segmentos de caminho adicionais.</span><span class="sxs-lookup"><span data-stu-id="8a421-p110">The redirect URI where you want the response to be sent for your app to handle. It must exactly match one of the redirect URIs that you registered in the portal, except that it must be URL encoded, and it can have additional path segments.</span></span> 
| <span data-ttu-id="8a421-166">estado</span><span class="sxs-lookup"><span data-stu-id="8a421-166">state</span></span>         | <span data-ttu-id="8a421-167">Recomendado</span><span class="sxs-lookup"><span data-stu-id="8a421-167">Recommended</span></span> | <span data-ttu-id="8a421-p111">Um valor incluído na solicitação e que também será retornado na resposta do token. Pode ser uma cadeia de caracteres de qualquer conteúdo que você desejar. O estado é usado para codificar as informações sobre o estado do usuário no aplicativo antes da solicitação de autenticação ter ocorrido, como a página ou o modo de exibição em que ele estava.</span><span class="sxs-lookup"><span data-stu-id="8a421-p111">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span> 

### <a name="administrator-consent-experience"></a><span data-ttu-id="8a421-171">Experiência de consentimento do administrador</span><span class="sxs-lookup"><span data-stu-id="8a421-171">Administrator consent experience</span></span>

<span data-ttu-id="8a421-p112">Através de solicitações ao ponto de extremidade `/adminconsent`, o Azure AD exige que apenas um administrador de locatário possa fazer logon para concluir a solicitação. O administrador será solicitado a aprovar todas as Permissões de aplicativo que você solicitar para seu aplicativo no Portal de Registro de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8a421-p112">With requests to the `/adminconsent` endpoint, Azure AD enforces that only a tenant administrator can sign in to complete the request. The administrator will be asked to approve all the application permissions that you have requested for your app in the app registration portal.</span></span> 

<span data-ttu-id="8a421-174">Veja a seguir um exemplo da caixa de diálogo de consentimento que o Azure AD apresenta ao administrador:</span><span class="sxs-lookup"><span data-stu-id="8a421-174">The following is an example of the consent dialog that Azure AD presents to the administrator:</span></span>

![Caixa de diálogo do consentimento do administrador.](./images/admin-consent.png)

### <a name="response"></a><span data-ttu-id="8a421-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a421-176">Response</span></span>

<span data-ttu-id="8a421-177">Se o administrador aprovar as permissões de seu aplicativo, a resposta bem-sucedida ficará assim:</span><span class="sxs-lookup"><span data-stu-id="8a421-177">If the administrator approves the permissions for your application, the successful response looks like this:</span></span>

```
// Line breaks are for legibility only.

GET https://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| <span data-ttu-id="8a421-178">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a421-178">Parameter</span></span>     | <span data-ttu-id="8a421-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a421-179">Description</span></span> 
|:--------------|:------------
| <span data-ttu-id="8a421-180">locatário</span><span class="sxs-lookup"><span data-stu-id="8a421-180">tenant</span></span>        | <span data-ttu-id="8a421-181">O locatário do diretório que concedeu as permissões de aplicativo solicitadas, no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="8a421-181">The directory tenant that granted your application the permissions that it requested, in GUID format.</span></span> 
| <span data-ttu-id="8a421-182">estado</span><span class="sxs-lookup"><span data-stu-id="8a421-182">state</span></span>         | <span data-ttu-id="8a421-p113">Um valor incluído na solicitação e que também será retornado na resposta do token. Pode ser uma cadeia de caracteres de qualquer conteúdo que você desejar. O estado é usado para codificar as informações sobre o estado do usuário no aplicativo antes da solicitação de autenticação ter ocorrido, como a página ou o modo de exibição em que ele estava.</span><span class="sxs-lookup"><span data-stu-id="8a421-p113">A value that is included in the request that also is returned in the token response. It can be a string of any content that you want. The state is used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.</span></span> 
| <span data-ttu-id="8a421-186">admin_consent</span><span class="sxs-lookup"><span data-stu-id="8a421-186">admin_consent</span></span> | <span data-ttu-id="8a421-187">Definir como **true**.</span><span class="sxs-lookup"><span data-stu-id="8a421-187">Set to **true**.</span></span> 


> <span data-ttu-id="8a421-p114">**Experimente**: Você pode experimentar ao colar a solicitação abaixo em um navegador. Se fizer logon como um Administrador global em um locatário do Azure AD, você verá a caixa de diálogo de consentimento do administrador para o aplicativo. (Este aplicativo será diferente do aplicativo exibido na tela da caixa de diálogo do consentimento previamente mostrada.)</span><span class="sxs-lookup"><span data-stu-id="8a421-p114">**Try**: You can try this for yourself by pasting the following request in a browser. If you sign in as a Global administrator for an Azure AD tenant, you will be presented with the administrator consent dialog box for the app. (This will be a different app than that in the consent dialog box screenshot shown earlier.)</span></span>
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a><span data-ttu-id="8a421-191">4. Obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="8a421-191">4. Get an access token</span></span>

<span data-ttu-id="8a421-192">No fluxo de concessão de credenciais do cliente OAuth 2.0, use os valores da ID do Aplicativo e o Segredo do aplicativo salvos quando você registrou o aplicativo para solicitar um token de acesso diretamente no ponto de extremidade `/token` do Azure AD v2.0.</span><span class="sxs-lookup"><span data-stu-id="8a421-192">In the OAuth 2.0 client credentials grant flow, you use the Application ID and Application Secret values that you saved when you registered your app to request an access token directly from the Azure AD v2.0 `/token` endpoint.</span></span>

<span data-ttu-id="8a421-p115">Você especifica as permissões pré-configuradas passando `https://graph.microsoft.com/.default` como o valor para o parâmetro `scope` na solicitação de token. Confira a descrição do parâmetro `scope` na solicitação de token abaixo para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="8a421-p115">You specify the pre-configured permissions by passing `https://graph.microsoft.com/.default` as the value for the `scope` parameter in the token request. See the `scope` parameter description in the token request below for details.</span></span>

### <a name="token-request"></a><span data-ttu-id="8a421-195">Solicitação de token</span><span class="sxs-lookup"><span data-stu-id="8a421-195">Token request</span></span>

<span data-ttu-id="8a421-196">Envie uma solicitação POST ao ponto de extremidade `/token` do v2.0 para adquirir um token de acesso:</span><span class="sxs-lookup"><span data-stu-id="8a421-196">You send a POST request to the `/token` v2.0 endpoint to acquire an access token:</span></span>

```
// Line breaks are for legibility only.

POST https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=535fb089-9ff3-47b6-9bfb-4f1264799865
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default
&client_secret=qWgdYAmab0YSkuL1qKv5bPX
&grant_type=client_credentials
```

| <span data-ttu-id="8a421-197">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a421-197">Parameter</span></span>     | <span data-ttu-id="8a421-198">Condição</span><span class="sxs-lookup"><span data-stu-id="8a421-198">Condition</span></span> | <span data-ttu-id="8a421-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a421-199">Description</span></span> 
|:--------------|:----------|:------------
| <span data-ttu-id="8a421-200">locatário</span><span class="sxs-lookup"><span data-stu-id="8a421-200">tenant</span></span>        | <span data-ttu-id="8a421-201">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-201">Required</span></span>  | <span data-ttu-id="8a421-p116">O locatário do diretório do qual você deseja solicitar permissão. Pode ser no formato de nome amigável ou GUID.</span><span class="sxs-lookup"><span data-stu-id="8a421-p116">The directory tenant that you want to request permission from. This can be in GUID or friendly name format.</span></span> 
| <span data-ttu-id="8a421-204">client_id</span><span class="sxs-lookup"><span data-stu-id="8a421-204">client_id</span></span>     | <span data-ttu-id="8a421-205">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-205">Required</span></span>  | <span data-ttu-id="8a421-206">A ID de Aplicativo que o [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com) atribuiu quando você registrou seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a421-206">The Application ID that the [Microsoft App Registration Portal](https://apps.dev.microsoft.com) assigned when you registered your app.</span></span> 
| <span data-ttu-id="8a421-207">escopo</span><span class="sxs-lookup"><span data-stu-id="8a421-207">scope</span></span>         | <span data-ttu-id="8a421-208">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-208">Required</span></span>  | <span data-ttu-id="8a421-p117">O valor passado para o parâmetro `scope` nesta solicitação deve ser o identificador do recurso (URI da ID do Aplicativo) do recurso desejado, afixado com o sufixo `.default`. Para o Microsoft Graph, o valor é `https://graph.microsoft.com/.default`. Esse valor informa ao ponto de extremidade do Microsoft Azure ADv2.0 que, de todas as Permissões de aplicativo que você configurou para seu aplicativo, ele deve emitir um token para os aplicativos associados ao recurso que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="8a421-p117">The value passed for the `scope` parameter in this request should be the resource identifier (Application ID URI) of the resource you want, affixed with the `.default` suffix. For Microsoft Graph, the value is `https://graph.microsoft.com/.default`. This value informs the v2.0 endpoint that of all the application permissions you have configured for your app, it should issue a token for the ones associated with the resource you want to use.</span></span> 
| <span data-ttu-id="8a421-212">client_secret</span><span class="sxs-lookup"><span data-stu-id="8a421-212">client_secret</span></span> | <span data-ttu-id="8a421-213">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-213">Required</span></span>  | <span data-ttu-id="8a421-214">O Segredo do Aplicativo gerado para seu aplicativo no portal de registro de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8a421-214">The Application Secret that you generated for your app in the app registration portal.</span></span> 
| <span data-ttu-id="8a421-215">grant_type</span><span class="sxs-lookup"><span data-stu-id="8a421-215">grant_type</span></span>    | <span data-ttu-id="8a421-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a421-216">Required</span></span>  | <span data-ttu-id="8a421-217">Deve ser `client_credentials`.</span><span class="sxs-lookup"><span data-stu-id="8a421-217">Must be `client_credentials`.</span></span> 

#### <a name="token-response"></a><span data-ttu-id="8a421-218">Resposta do token</span><span class="sxs-lookup"><span data-stu-id="8a421-218">Token response</span></span>

<span data-ttu-id="8a421-219">Uma resposta bem-sucedida tem esta aparência:</span><span class="sxs-lookup"><span data-stu-id="8a421-219">A successful response looks like this:</span></span>

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| <span data-ttu-id="8a421-220">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a421-220">Parameter</span></span>     | <span data-ttu-id="8a421-221">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a421-221">Description</span></span> 
|:--------------|:------------
| <span data-ttu-id="8a421-222">access_token</span><span class="sxs-lookup"><span data-stu-id="8a421-222">access_token</span></span>  | <span data-ttu-id="8a421-p118">O token de acesso solicitado. Seu aplicativo pode usar esse token em chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8a421-p118">The requested access token. Your app can use this token in calls to Microsoft Graph.</span></span> 
| <span data-ttu-id="8a421-225">token_type</span><span class="sxs-lookup"><span data-stu-id="8a421-225">token_type</span></span>    | <span data-ttu-id="8a421-p119">Indica o valor de tipo de token. O único tipo ao qual o Azure AD dá suporte é `bearer`.</span><span class="sxs-lookup"><span data-stu-id="8a421-p119">Indicates the token type value. The only type that Azure AD supports is `bearer`.</span></span> 
| <span data-ttu-id="8a421-228">expires_in</span><span class="sxs-lookup"><span data-stu-id="8a421-228">expires_in</span></span>    | <span data-ttu-id="8a421-229">Por quanto tempo o token de acesso é válido (em segundos).</span><span class="sxs-lookup"><span data-stu-id="8a421-229">How long the access token is valid (in seconds).</span></span> 

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a><span data-ttu-id="8a421-230">5. Use o token de acesso para chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a421-230">5. Use the access token to call Microsoft Graph</span></span>

<span data-ttu-id="8a421-p120">Após obter o token de acesso, você pode usá-lo para chamar o Microsoft Graph, incluindo-o no cabeçalho `Authorization` de uma solicitação. A solicitação a seguir obtém o perfil de um usuário específico. Seu aplicativo deve ter a permissão _User.Read.All_ para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8a421-p120">After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of a specific user. Your app must have the _User.Read.All_ permission to call this API.</span></span>

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f 
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
<span data-ttu-id="8a421-234">Uma resposta bem-sucedida terá a seguinte aparência (alguns cabeçalhos de resposta foram removidos):</span><span class="sxs-lookup"><span data-stu-id="8a421-234">A successful response will look similar to this (some response headers have been removed):</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 309.0273
Date: Wed, 26 Apr 2017 19:53:49 GMT
Content-Length: 407
```

```json
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="supported-app-scenarios-and-resources"></a><span data-ttu-id="8a421-235">Recursos e cenários de aplicativo com suporte</span><span class="sxs-lookup"><span data-stu-id="8a421-235">Supported app scenarios and resources</span></span>

<span data-ttu-id="8a421-236">Os aplicativos que chamam o Microsoft Graph com sua própria identidade se enquadram em uma dessas categorias:</span><span class="sxs-lookup"><span data-stu-id="8a421-236">Apps that call Microsoft Graph under their own identity fall into one of two categories:</span></span>

- <span data-ttu-id="8a421-237">Serviços em segundo plano (daemons) que podem ser executados em um servidor sem um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8a421-237">Background services (daemons) that run on a server without a signed-in user.</span></span>
- <span data-ttu-id="8a421-238">Aplicativos que têm um usuário conectado, mas que também chamam o Microsoft Graph com sua própria identidade. Por exemplo, para usar a funcionalidade que exige privilégios mais elevados do usuário.</span><span class="sxs-lookup"><span data-stu-id="8a421-238">Apps that have a signed-in user but also call Microsoft Graph with their own identity; for example, to use functionality that requires more elevated privileges than those of the user.</span></span>

<span data-ttu-id="8a421-p121">Os aplicativos que chamam o Microsoft Graph com sua própria identidade usam a concessão de credenciais do cliente OAuth 2.0 para autenticar com o Azure AD e obter um token. Para o ponto de extremidade do v2.0, você pode explorar esse cenário ainda mais com os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="8a421-p121">Apps that call Microsoft Graph with their own identity use the OAuth 2.0 client credentials grant to authenticate with Azure AD and get a token. For the v2.0 endpoint, you can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="8a421-241">Para ver um tratamento mais completo do Fluxo de Concessão de Credenciais do Cliente que também inclui respostas de erro, confira o artigo [Azure Active Directory v2.0 e o fluxo de Credenciais do Cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds).</span><span class="sxs-lookup"><span data-stu-id="8a421-241">For a more complete treatment of the client credentials grant flow that also includes error responses, see [Azure Active Directory v2.0 and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols-oauth-client-creds).</span></span> 
- <span data-ttu-id="8a421-242">Para obter um exemplo que chama o Microsoft Graph a partir de um serviço, confira o [exemplo do daemon v2.0](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="8a421-242">For a sample that calls Microsoft Graph from a service, see the [v2.0 daemon sample](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) on GitHub.</span></span>
- <span data-ttu-id="8a421-243">Para obter mais informações sobre bibliotecas de autenticação recomendadas da Microsoft e de terceiros do Azure AD v2.0, confira as [bibliotecas de autenticação do Azure Active Directory v2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).</span><span class="sxs-lookup"><span data-stu-id="8a421-243">For more information about recommended Microsoft and third-party authentication libraries for Azure AD v2.0, see [Azure Active Directory v2.0 authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).</span></span>

## <a name="azure-ad-endpoint-considerations"></a><span data-ttu-id="8a421-244">Considerações sobre o ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="8a421-244">Azure AD endpoint considerations</span></span>

<span data-ttu-id="8a421-245">Se você estiver usando o ponto de extremidade do Azure AD, existem algumas diferenças na maneira de configurar seu aplicativo e a maneira de conectá-lo ao Azure AD:</span><span class="sxs-lookup"><span data-stu-id="8a421-245">If you are using the Azure AD endpoint, there are some differences in the way that you configure your app and the way that it signs in to Azure AD:</span></span>

- <span data-ttu-id="8a421-p122">Você usa o [Portal do Azure](https://portal.azure.com) para configurar seu aplicativo. Para obter mais informações sobre como configurar aplicativos com o Portal do Azure, confira [Integração de aplicativos com o Azure Active Directory: Como adicionar um aplicativo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)</span><span class="sxs-lookup"><span data-stu-id="8a421-p122">You use the [Azure portal](https://portal.azure.com) to configure your app. For more information about configuring apps with the Azure portal, see [Integrating applications with Azure Active Directory: Adding an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)</span></span>
- <span data-ttu-id="8a421-248">Se o aplicativo for um aplicativo multilocatário, você deve configurá-lo explicitamente para funcionar como vários locatários no [Portal do Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="8a421-248">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant at the [Azure portal](https://portal.azure.com).</span></span>
- <span data-ttu-id="8a421-p123">Não há um ponto de extremidade de consentimento do administrador (`/adminconsent`), em vez disso, o aplicativo pode solicitar o consentimento do administrador durante o tempo de execução adicionando o parâmetro `prompt=admin_consent` a uma solicitação de autorização. Para obter mais informações, confira **Como acionar a estrutura do consentimento do Azure AD no tempo de execução** no artigo [Integração de aplicativos com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).</span><span class="sxs-lookup"><span data-stu-id="8a421-p123">There is no admin consent endpoint (`/adminconsent`), instead, your app can request administrator consent during runtime by adding the `prompt=admin_consent` parameter to an authorization request. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).</span></span>
- <span data-ttu-id="8a421-p124">Os parâmetros nas solicitações de token e de autorização são diferentes. Por exemplo, não existe um parâmetro `scope` nas solicitações do ponto de extremidade do Azure AD. Em vez disso, o parâmetro `resource` é usado para especificar o URI do recurso (`resource=https://graph.microsoft.com`) que a autorização (para consentimento do administrador) ou um token está solicitando.</span><span class="sxs-lookup"><span data-stu-id="8a421-p124">The parameters in authorization and token requests are different. For example, there is no `scope` parameter in Azure AD endpoint requests; instead, the `resource` parameter is used to specify the URI of the resource (`resource=https://graph.microsoft.com`) that authorization (for administrator consent) or a token is being requested for.</span></span>

<span data-ttu-id="8a421-253">Para o ponto de extremidade do Azure AD, você pode explorar esse cenário ainda mais com os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="8a421-253">For the Azure AD endpoint, you can explore this scenario further with the following resources:</span></span>

- <span data-ttu-id="8a421-254">Para obter links rápidos para uma visão geral, exemplos e um tratamento detalhado do fluxo de Concessão de Credenciais do Cliente, confira **Serviço a serviço**, na **seção de Introdução** da página [Azure Active Directory para desenvolvedores](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide).</span><span class="sxs-lookup"><span data-stu-id="8a421-254">For quick links to an overview, samples, and a detailed treatment of the client credentials grant flow, see **Service-to-Service** in the **Getting Started section** in [Azure Active Directory for Developers](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide).</span></span>
- <span data-ttu-id="8a421-p125">Para o ponto de extremidade do AD do Azure, você pode usar a Biblioteca de Autenticação do Azure Active Directory (ADAL) para obter tokens do Azure AD. A ADAL está disponível para várias plataformas, incluindo .NET, iOS, Android, JavaScript, Java e Node.js. Para obter mais informações sobre a ADAL e outras bibliotecas de autenticação da Microsoft para o ponto de extremidade do Azure AD, confira as [Bibliotecas de Autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="8a421-p125">For the Azure AD endpoint, you can use the Azure Active Directory Authentication Library (ADAL) to get tokens from Azure AD. ADAL is available for several platforms including .NET, iOS, Android, JavaScript, Java, and Node.js. For more information about ADAL and other Microsoft authentication libraries for the Azure AD endpoint, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> 

 
