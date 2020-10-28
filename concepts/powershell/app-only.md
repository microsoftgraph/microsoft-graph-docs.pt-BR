---
title: Usar a autenticação somente de aplicativo com o SDK do Microsoft Graph PowerShell
description: Saiba como usar a autenticação somente de aplicativo para habilitar cenários não interativos com o SDK do Microsoft Graph PowerShell.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 6cad5979e5bd7523174a792465d015dfe7d3d217
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782925"
---
# <a name="use-app-only-authentication-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="220a0-103">Usar a autenticação somente de aplicativo com o SDK do Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="220a0-103">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="220a0-104">O SDK do PowerShell oferece suporte a dois tipos de autenticação: [acesso delegado](..\auth-v2-user.md)e [acesso somente de aplicativo](..\auth-v2-service.md).</span><span class="sxs-lookup"><span data-stu-id="220a0-104">The PowerShell SDK supports two types of authentication: [delegated access](..\auth-v2-user.md), and [app-only access](..\auth-v2-service.md).</span></span> <span data-ttu-id="220a0-105">Este guia se concentrará na configuração necessária para habilitar o acesso somente de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220a0-105">This guide will focus on the configuration needed to enable app-only access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="220a0-106">O acesso somente do aplicativo concede permissões diretamente a um aplicativo e exige que um administrador concorde com os escopos de permissão necessários.</span><span class="sxs-lookup"><span data-stu-id="220a0-106">App-only access grants permissions directly to an application, and requires an administrator to consent to the required permission scopes.</span></span> <span data-ttu-id="220a0-107">Para obter mais detalhes sobre acesso somente de aplicativo, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="220a0-107">For more details on app-only access, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

<span data-ttu-id="220a0-108">Vamos examinar a configuração de acesso somente aplicativo para um script simples para listar usuários e grupos em seu locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="220a0-108">Let's walk through configuring app-only access for a simple script to list users and groups in your Microsoft 365 tenant.</span></span>

## <a name="configuration"></a><span data-ttu-id="220a0-109">Configuração</span><span class="sxs-lookup"><span data-stu-id="220a0-109">Configuration</span></span>

<span data-ttu-id="220a0-110">Para poder usar o acesso somente de aplicativo com o SDK, você precisa do seguinte.</span><span class="sxs-lookup"><span data-stu-id="220a0-110">Before you can use app-only access with the SDK, you need the following.</span></span>

- <span data-ttu-id="220a0-111">Um certificado a ser usado como uma credencial para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220a0-111">A certificate to use as a credential for the application.</span></span> <span data-ttu-id="220a0-112">Pode ser um certificado autoassinado ou um certificado de uma autoridade.</span><span class="sxs-lookup"><span data-stu-id="220a0-112">This can be a self-signed certificate or a certificate from an authority.</span></span>
- <span data-ttu-id="220a0-113">Você deve [registrar um aplicativo](/azure/active-directory/develop/app-objects-and-service-principals) no Azure AD, configurá-lo com os escopos de permissão que seu cenário requer e compartilhar a chave pública do seu certificado.</span><span class="sxs-lookup"><span data-stu-id="220a0-113">You must [register an application](/azure/active-directory/develop/app-objects-and-service-principals) in Azure AD, configure it with the permission scopes your scenario requires, and share the public key for your certificate.</span></span>

### <a name="certificate"></a><span data-ttu-id="220a0-114">Certificado</span><span class="sxs-lookup"><span data-stu-id="220a0-114">Certificate</span></span>

<span data-ttu-id="220a0-115">Você precisará de um certificado X. 509 instalado no armazenamento confiável do usuário no computador em que o script será executado.</span><span class="sxs-lookup"><span data-stu-id="220a0-115">You will need an X.509 certificate installed in your user's trusted store on the machine where you will run the script.</span></span> <span data-ttu-id="220a0-116">Você também precisará da chave pública do certificado exportada no formato. cer,. PEM ou. CRT.</span><span class="sxs-lookup"><span data-stu-id="220a0-116">You'll also need the certificate's public key exported in .cer, .pem, or .crt format.</span></span> <span data-ttu-id="220a0-117">Você precisará do valor do requerente do certificado.</span><span class="sxs-lookup"><span data-stu-id="220a0-117">You'll need the value of the certificate subject.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="220a0-118">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="220a0-118">Register the application</span></span>

<span data-ttu-id="220a0-119">Você pode registrar o aplicativo no [portal do Azure Active Directory](https://aad.portal.azure.com)ou usando o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="220a0-119">You can register the application either in the [Azure Active Directory portal](https://aad.portal.azure.com), or using PowerShell.</span></span>

# <a name="portal"></a>[<span data-ttu-id="220a0-120">Portal</span><span class="sxs-lookup"><span data-stu-id="220a0-120">Portal</span></span>](#tab/azure-portal)

1. <span data-ttu-id="220a0-121">Abra um navegador e navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando um administrador da organização de locatários do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="220a0-121">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using an Microsoft 365 tenant organization admin.</span></span>

1. <span data-ttu-id="220a0-122">Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar** .</span><span class="sxs-lookup"><span data-stu-id="220a0-122">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage** .</span></span>

    ![<span data-ttu-id="220a0-123">Uma captura de tela dos registros de aplicativo</span><span class="sxs-lookup"><span data-stu-id="220a0-123">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="220a0-124">Selecione **Novo registro** .</span><span class="sxs-lookup"><span data-stu-id="220a0-124">Select **New registration** .</span></span> <span data-ttu-id="220a0-125">Na página **Registrar um aplicativo** , defina os valores da seguinte forma.</span><span class="sxs-lookup"><span data-stu-id="220a0-125">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="220a0-126">Defina **Nome** para `Graph PowerShell Script`.</span><span class="sxs-lookup"><span data-stu-id="220a0-126">Set **Name** to `Graph PowerShell Script`.</span></span>
    - <span data-ttu-id="220a0-127">Defina os **tipos de conta com suporte** para **contas nesse diretório organizacional apenas** .</span><span class="sxs-lookup"><span data-stu-id="220a0-127">Set **Supported account types** to **Accounts in this organizational directory only** .</span></span>
    - <span data-ttu-id="220a0-128">Deixe **URI de redirecionamento** em branco.</span><span class="sxs-lookup"><span data-stu-id="220a0-128">Leave **Redirect URI** blank.</span></span>

    ![Uma captura de tela da página registrar um aplicativo](./images/register-app.png)

1. <span data-ttu-id="220a0-130">Selecione **Registrar** .</span><span class="sxs-lookup"><span data-stu-id="220a0-130">Select **Register** .</span></span> <span data-ttu-id="220a0-131">Na página **script do PowerShell do Graph** , copie os valores da ID do **aplicativo (cliente)** e da ID do **diretório (locatário)** e salve-os.</span><span class="sxs-lookup"><span data-stu-id="220a0-131">On the **Graph PowerShell Script** page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them.</span></span>

    ![Uma captura de tela da ID do aplicativo do novo registro de aplicativo](./images/aad-application-id.png)

1. <span data-ttu-id="220a0-133">Selecione **permissões de API** em **gerenciar** .</span><span class="sxs-lookup"><span data-stu-id="220a0-133">Select **API Permissions** under **Manage** .</span></span> <span data-ttu-id="220a0-134">Escolha **Adicionar uma permissão** .</span><span class="sxs-lookup"><span data-stu-id="220a0-134">Choose **Add a permission** .</span></span>

1. <span data-ttu-id="220a0-135">Selecione **Microsoft Graph** e, em seguida, **permissões de aplicativo** .</span><span class="sxs-lookup"><span data-stu-id="220a0-135">Select **Microsoft Graph** , then **Application Permissions** .</span></span> <span data-ttu-id="220a0-136">Add **User. Read. All** e **Group. Read. All** e, em seguida, selecione **adicionar permissões** .</span><span class="sxs-lookup"><span data-stu-id="220a0-136">Add **User.Read.All** and **Group.Read.All** , then select **Add permissions** .</span></span>

1. <span data-ttu-id="220a0-137">Nas **permissões configuradas** , remova a permissão **usuário delegado. Read** no **Microsoft Graph** selecionando o **...** à direita da permissão e selecionando **remover permissão** .</span><span class="sxs-lookup"><span data-stu-id="220a0-137">In the **Configured permissions** , remove the delegated **User.Read** permission under **Microsoft Graph** by selecting the **...** to the right of the permission and selecting **Remove permission** .</span></span> <span data-ttu-id="220a0-138">Selecione **Sim, remover** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="220a0-138">Select **Yes, remove** to confirm.</span></span>

1. <span data-ttu-id="220a0-139">Selecione o botão **conceder permissão de administrador para...** e, em seguida, selecione **Sim** para conceder consentimento de administrador para as permissões de aplicativo configuradas.</span><span class="sxs-lookup"><span data-stu-id="220a0-139">Select the **Grant admin consent for...** button, then select **Yes** to grant admin consent for the configured application permissions.</span></span> <span data-ttu-id="220a0-140">A coluna **status** na tabela de **permissões configurada** é alterada para **concedido para..** ..</span><span class="sxs-lookup"><span data-stu-id="220a0-140">The **Status** column in the **Configured permissions** table changes to **Granted for ...** .</span></span>

    ![Uma captura de tela das permissões configuradas para o webhook com consentimento de administrador concedido](./images/configured-permissions.png)

1. <span data-ttu-id="220a0-142">Selecione **Certificados e segredos** sob **Gerenciar** .</span><span class="sxs-lookup"><span data-stu-id="220a0-142">Select **Certificates & secrets** under **Manage** .</span></span> <span data-ttu-id="220a0-143">Selecione o botão **carregar certificado** .</span><span class="sxs-lookup"><span data-stu-id="220a0-143">Select the **Upload certificate** button.</span></span> <span data-ttu-id="220a0-144">Navegue até o arquivo de chave pública do certificado e selecione **Adicionar** .</span><span class="sxs-lookup"><span data-stu-id="220a0-144">Browse to your certificate's public key file and select **Add** .</span></span>

# <a name="powershell"></a>[<span data-ttu-id="220a0-145">PowerShell</span><span class="sxs-lookup"><span data-stu-id="220a0-145">PowerShell</span></span>](#tab/powershell)

> [!NOTE]
> <span data-ttu-id="220a0-146">Você deve ter o SDK do Microsoft Graph PowerShell [instalado](installation.md) antes de seguir estas etapas.</span><span class="sxs-lookup"><span data-stu-id="220a0-146">You must have the Microsoft Graph PowerShell SDK [installed](installation.md) before following these steps.</span></span>

<span data-ttu-id="220a0-147">Você pode estar se perguntando: "posso usar o SDK do PowerShell para registrar um aplicativo, para que eu possa usar o SDK do PowerShell?"</span><span class="sxs-lookup"><span data-stu-id="220a0-147">You may be wondering: "I can use the PowerShell SDK to register an app, so that I can use the PowerShell SDK?"</span></span> <span data-ttu-id="220a0-148">Sim!</span><span class="sxs-lookup"><span data-stu-id="220a0-148">Yes!</span></span> <span data-ttu-id="220a0-149">Nesse caso, você está usando o SDK do PowerShell com acesso delegado, fazendo logon como administrador e criando o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220a0-149">In this case, you're using the PowerShell SDK with delegated access, logging in as an administrator, and creating the app registration.</span></span> <span data-ttu-id="220a0-150">Em seguida, usando esse registro de aplicativo, você é capaz de usar o SDK do PowerShell com acesso somente de aplicativo, permitindo scripts autônomos.</span><span class="sxs-lookup"><span data-stu-id="220a0-150">Then, using that app registration, you're able to use the PowerShell SDK with app-only access, allowing for unattended scripts.</span></span>

1. <span data-ttu-id="220a0-151">Use um editor de texto para criar um novo arquivo chamado **RegisterAppOnly.ps1** .</span><span class="sxs-lookup"><span data-stu-id="220a0-151">Use a text editor to create a new file named **RegisterAppOnly.ps1** .</span></span> <span data-ttu-id="220a0-152">Cole o código a seguir no arquivo.</span><span class="sxs-lookup"><span data-stu-id="220a0-152">Paste the following code into the file.</span></span>

    :::code language="powershell" source="RegisterAppOnly.ps1":::

1. <span data-ttu-id="220a0-153">Salve o arquivo.</span><span class="sxs-lookup"><span data-stu-id="220a0-153">Save the file.</span></span> <span data-ttu-id="220a0-154">Abra o PowerShell no diretório que contém **RegisterAppOnly.ps1** e execute o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="220a0-154">Open PowerShell in the directory that contains **RegisterAppOnly.ps1** and run the following command.</span></span>

    ```powershell
    .\RegisterAppOnly.ps1 -AppName "Graph PowerShell Script" -CertPath "PATH_TO_PUBLIC_KEY_FILE"
    ```

1. <span data-ttu-id="220a0-155">Abra o navegador conforme solicitado.</span><span class="sxs-lookup"><span data-stu-id="220a0-155">Open your browser as prompted.</span></span> <span data-ttu-id="220a0-156">Entre com uma conta de administrador e aceite as permissões.</span><span class="sxs-lookup"><span data-stu-id="220a0-156">Sign in with an administrator account and accept the permissions.</span></span>

1. <span data-ttu-id="220a0-157">Revise a saída do prompt `Please go to the following URL in your browser to provide admin consent` .</span><span class="sxs-lookup"><span data-stu-id="220a0-157">Review the output for the prompt `Please go to the following URL in your browser to provide admin consent`.</span></span> <span data-ttu-id="220a0-158">Copie a URL fornecida e cole-a no navegador.</span><span class="sxs-lookup"><span data-stu-id="220a0-158">Copy the URL provided and paste it in your browser.</span></span> <span data-ttu-id="220a0-159">Entre com uma conta de administrador para conceder o consentimento do administrador ao aplicativo recentemente registrado.</span><span class="sxs-lookup"><span data-stu-id="220a0-159">Sign in with an administrator account to grant admin consent to your newly registered application.</span></span>

    > [!NOTE]
    > <span data-ttu-id="220a0-160">Após conceder o consentimento do administrador, o navegador exibirá um erro: `AADSTS500113: No reply address is registered for the application` .</span><span class="sxs-lookup"><span data-stu-id="220a0-160">After granting admin consent, the browser will display an error: `AADSTS500113: No reply address is registered for the application`.</span></span> <span data-ttu-id="220a0-161">Isso ocorre porque o registro do aplicativo não inclui uma URL de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="220a0-161">This is because the app registration does not include a redirect URL.</span></span> <span data-ttu-id="220a0-162">Esse erro pode ser ignorado.</span><span class="sxs-lookup"><span data-stu-id="220a0-162">This error can be ignored.</span></span>

1. <span data-ttu-id="220a0-163">Revise o restante da saída do PowerShell para o `Connect-MgGraph` comando previamente preenchido com os valores para o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220a0-163">Review the rest of the PowerShell output for `Connect-MgGraph` command pre-filled with the values for your app registration.</span></span>

---

## <a name="authenticate"></a><span data-ttu-id="220a0-164">Autenticar</span><span class="sxs-lookup"><span data-stu-id="220a0-164">Authenticate</span></span>

<span data-ttu-id="220a0-165">Você deve ter três informações depois de concluir as etapas de configuração acima.</span><span class="sxs-lookup"><span data-stu-id="220a0-165">You should have three pieces of information after completing the configuration steps above.</span></span>

- <span data-ttu-id="220a0-166">Requerente do certificado do certificado carregado no registro de aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="220a0-166">Certificate subject of the certificate uploaded to your Azure AD app registration.</span></span>
- <span data-ttu-id="220a0-167">ID de aplicativo para o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220a0-167">Application ID for your app registration.</span></span>
- <span data-ttu-id="220a0-168">Sua ID de locatário.</span><span class="sxs-lookup"><span data-stu-id="220a0-168">Your tenant ID.</span></span>

<span data-ttu-id="220a0-169">Vamos usá-los para testar a autenticação.</span><span class="sxs-lookup"><span data-stu-id="220a0-169">Let's use those to test authentication.</span></span> <span data-ttu-id="220a0-170">Abra o PowerShell e execute o comando a seguir, substituindo os espaços reservados por suas informações.</span><span class="sxs-lookup"><span data-stu-id="220a0-170">Open PowerShell and run the following command, replacing the placeholders with your information.</span></span>

```powershell
Connect-MgGraph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT
```

<span data-ttu-id="220a0-171">Se isso tiver êxito, você verá `Welcome To Microsoft Graph!` .</span><span class="sxs-lookup"><span data-stu-id="220a0-171">If this succeeds, you will see `Welcome To Microsoft Graph!`.</span></span> <span data-ttu-id="220a0-172">Execute `Get-MgContext` para verificar se você se autenticou somente com o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="220a0-172">Run `Get-MgContext` to verify that you've authenticated with app-only.</span></span> <span data-ttu-id="220a0-173">A saída deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="220a0-173">The output should look like the following.</span></span>

```powershell
ClientId              : YOUR_APP_ID
TenantId              : YOUR_TENANT_ID
CertificateThumbprint :
Scopes                : {Group.Read.All, User.Read.All}
AuthType              : AppOnly
CertificateName       : YOUR_CERT_SUBJECT
Account               :
AppName               : Graph PowerShell Script
ContextScope          : Process
```

## <a name="create-the-script"></a><span data-ttu-id="220a0-174">Criar o script</span><span class="sxs-lookup"><span data-stu-id="220a0-174">Create the script</span></span>

<span data-ttu-id="220a0-175">Crie um novo arquivo chamado **GraphAppOnly.ps1** e adicione o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="220a0-175">Create a new file named **GraphAppOnly.ps1** and add the following code.</span></span>

```powershell
# Authenticate
Connect-MgGraph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT

Write-Host "USERS:"
Write-Host "======================================================"
# List first 50 users
Get-MgUser -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

Write-Host "GROUPS:"
Write-Host "======================================================"
# List first 50 groups
Get-MgGroup -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

# Disconnect
Disconnect-MgGraph
```

<span data-ttu-id="220a0-176">Substitua os espaços reservados no `Connect-MgGraph` comando por suas informações.</span><span class="sxs-lookup"><span data-stu-id="220a0-176">Replace the placeholders in the `Connect-MgGraph` command with your information.</span></span> <span data-ttu-id="220a0-177">Salve o arquivo e, em seguida, abra o PowerShell no diretório em que você criou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="220a0-177">Save the file, then open PowerShell in the directory where you created the file.</span></span> <span data-ttu-id="220a0-178">Execute o script com o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="220a0-178">Run the script with the following command.</span></span>

```powershell
.\GraphAppOnly.ps1
```

<span data-ttu-id="220a0-179">O script gera uma lista de usuários e grupos semelhante à saída abaixo (truncada para obter brevidade).</span><span class="sxs-lookup"><span data-stu-id="220a0-179">The script outputs a list of users and groups similar to the output below (truncated for brevity).</span></span>

```powershell
Welcome To Microsoft Graph!
USERS:
======================================================

DisplayName              Id
-----------              --
Conf Room Adams          88d1ba68-8ff5-4de2-90ed-768c00abcfae
Adele Vance              3103c7b9-cfe6-4cd3-a696-f88909b9a609
MOD Administrator        da3a885e-2d97-41de-9347-5271ef321b58
...

GROUPS:
======================================================

DisplayName                         Id
-----------                         --
App Development                     06dce3e5-d310-4add-ab2c-be728fb9076e
All Employees                       1a1cd42d-9801-4e9d-9b77-5215886174ef
Mark 8 Project Team                 2bf1b0d0-81f6-4e80-b971-d1db69f8d651
...
```
