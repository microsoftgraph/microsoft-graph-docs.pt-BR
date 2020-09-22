---
title: Usar a autenticação somente de aplicativo com o SDK do Microsoft Graph PowerShell
description: Saiba como usar a autenticação somente de aplicativo para habilitar cenários não interativos com o SDK do Microsoft Graph PowerShell.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 5e43072844193a7d971027e7e5368e4782c32e54
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193665"
---
# <a name="use-app-only-authentication-with-the-microsoft-graph-powershell-sdk"></a>Usar a autenticação somente de aplicativo com o SDK do Microsoft Graph PowerShell

O SDK do PowerShell oferece suporte a dois tipos de autenticação: [acesso delegado](..\auth-v2-user.md)e [acesso somente de aplicativo](..\auth-v2-service.md). Este guia se concentrará na configuração necessária para habilitar o acesso somente de aplicativo.

> [!IMPORTANT]
> O acesso somente do aplicativo concede permissões diretamente a um aplicativo e exige que um administrador concorde com os escopos de permissão necessários. Para obter mais detalhes sobre acesso somente de aplicativo, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

Vamos examinar a configuração de acesso somente aplicativo para um script simples para listar usuários e grupos em seu locatário do Microsoft 365.

## <a name="configuration"></a>Configuração

Para poder usar o acesso somente de aplicativo com o SDK, você precisa do seguinte.

- Um certificado a ser usado como uma credencial para o aplicativo. Pode ser um certificado autoassinado ou um certificado de uma autoridade.
- Você deve [registrar um aplicativo](/azure/active-directory/develop/app-objects-and-service-principals) no Azure AD, configurá-lo com os escopos de permissão que seu cenário requer e compartilhar a chave pública do seu certificado.

### <a name="certificate"></a>Certificado

Você precisará de um certificado X. 509 instalado no armazenamento confiável do usuário no computador em que o script será executado. Você também precisará da chave pública do certificado exportada no formato. cer,. PEM ou. CRT. Você precisará do valor do requerente do certificado.

### <a name="register-the-application"></a>Registrar o aplicativo

Você pode registrar o aplicativo no [portal do Azure Active Directory](https://aad.portal.azure.com)ou usando o PowerShell.

# <a name="portal"></a>[Portal](#tab/azure-portal)

1. Abra um navegador e navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando um administrador da organização de locatários do Microsoft 365.

1. Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar**.

    ![Uma captura de tela dos registros de aplicativo ](./images/aad-portal-app-registrations.png)

1. Selecione **Novo registro**. Na página **Registrar um aplicativo**, defina os valores da seguinte forma.

    - Defina **Nome** para `Graph PowerShell Script`.
    - Defina os **tipos de conta com suporte** para **contas nesse diretório organizacional apenas**.
    - Deixe **URI de redirecionamento** em branco.

    ![Uma captura de tela da página registrar um aplicativo](./images/register-app.png)

1. Selecione **Registrar**. Na página **script do PowerShell do Graph** , copie os valores da ID do **aplicativo (cliente)** e da ID do **diretório (locatário)** e salve-os.

    ![Uma captura de tela da ID do aplicativo do novo registro de aplicativo](./images/aad-application-id.png)

1. Selecione **permissões de API** em **gerenciar**. Escolha **Adicionar uma permissão**.

1. Selecione **Microsoft Graph**e, em seguida, **permissões de aplicativo**. Add **User. Read. All** e **Group. Read. All**e, em seguida, selecione **adicionar permissões**.

1. Nas **permissões configuradas**, remova a permissão **usuário delegado. Read** no **Microsoft Graph** selecionando o **...** à direita da permissão e selecionando **remover permissão**. Selecione **Sim, remover** para confirmar.

1. Selecione o botão **conceder permissão de administrador para...** e, em seguida, selecione **Sim** para conceder consentimento de administrador para as permissões de aplicativo configuradas. A coluna **status** na tabela de **permissões configurada** é alterada para **concedido para..**..

    ![Uma captura de tela das permissões configuradas para o webhook com consentimento de administrador concedido](./images/configured-permissions.png)

1. Selecione **Certificados e segredos** sob **Gerenciar**. Selecione o botão **carregar certificado** . Navegue até o arquivo de chave pública do certificado e selecione **Adicionar**.

# <a name="powershell"></a>[PowerShell](#tab/powershell)

> [!NOTE]
> Você deve ter o SDK do Microsoft Graph PowerShell [instalado](installation.md) antes de seguir estas etapas.

Você pode estar se perguntando: "posso usar o SDK do PowerShell para registrar um aplicativo, para que eu possa usar o SDK do PowerShell?" Sim! Nesse caso, você está usando o SDK do PowerShell com acesso delegado, fazendo logon como administrador e criando o registro do aplicativo. Em seguida, usando esse registro de aplicativo, você é capaz de usar o SDK do PowerShell com acesso somente de aplicativo, permitindo scripts autônomos.

1. Use um editor de texto para criar um novo arquivo chamado **RegisterAppOnly.ps1**. Cole o código a seguir no arquivo.

    :::code language="powershell" source="RegisterAppOnly.ps1":::

1. Salve o arquivo. Abra o PowerShell no diretório que contém **RegisterAppOnly.ps1** e execute o comando a seguir.

    ```powershell
    .\RegisterAppOnly.ps1 -AppName "Graph PowerShell Script" -CertPath "PATH_TO_PUBLIC_KEY_FILE"
    ```

1. Abra o navegador conforme solicitado. Entre com uma conta de administrador e aceite as permissões.

1. Revise a saída do prompt `Please go to the following URL in your browser to provide admin consent` . Copie a URL fornecida e cole-a no navegador. Entre com uma conta de administrador para conceder o consentimento do administrador ao aplicativo recentemente registrado.

    > [!NOTE]
    > Após conceder o consentimento do administrador, o navegador exibirá um erro: `AADSTS500113: No reply address is registered for the application` . Isso ocorre porque o registro do aplicativo não inclui uma URL de redirecionamento. Esse erro pode ser ignorado.

1. Revise o restante da saída do PowerShell para o `Connect-Graph` comando previamente preenchido com os valores para o registro do aplicativo.

---

## <a name="authenticate"></a>Autenticar

Você deve ter três informações depois de concluir as etapas de configuração acima.

- Requerente do certificado do certificado carregado no registro de aplicativo do Azure AD.
- ID de aplicativo para o registro do aplicativo.
- Sua ID de locatário.

Vamos usá-los para testar a autenticação. Abra o PowerShell e execute o comando a seguir, substituindo os espaços reservados por suas informações.

```powershell
Connect-Graph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT
```

Se isso tiver êxito, você verá `Welcome To Microsoft Graph!` . Execute `Get-MgContext` para verificar se você se autenticou somente com o aplicativo. A saída deve ter a seguinte aparência.

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

## <a name="create-the-script"></a>Criar o script

Crie um novo arquivo chamado **GraphAppOnly.ps1** e adicione o código a seguir.

```powershell
# Authenticate
Connect-Graph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT

Write-Host "USERS:"
Write-Host "======================================================"
# List first 50 users
Get-MgUser -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

Write-Host "GROUPS:"
Write-Host "======================================================"
# List first 50 groups
Get-MgGroup -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

# Disconnect
Disconnect-Graph
```

Substitua os espaços reservados no `Connect-Graph` comando por suas informações. Salve o arquivo e, em seguida, abra o PowerShell no diretório em que você criou o arquivo. Execute o script com o comando a seguir.

```powershell
.\GraphAppOnly.ps1
```

O script gera uma lista de usuários e grupos semelhante à saída abaixo (truncada para obter brevidade).

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
