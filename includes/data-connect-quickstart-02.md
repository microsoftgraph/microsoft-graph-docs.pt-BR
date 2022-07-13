---
ms.localizationpriority: medium
ms.openlocfilehash: e34c0fb669d87c130181e1af13ca97ca84e58497
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768200"
---
<!-- markdownlint-disable MD002 MD041 -->

Antes de usar o Microsoft Graph Data Connect pela primeira vez, você precisa configurar seu locatário do Microsoft 365. Isso envolve ativar o serviço e configurar um grupo de segurança com permissões para aprovar solicitações de extração de dados.

## <a name="grant-azure-ad-users-the-global-administrator-role"></a>Conceder aos Azure AD usuários a Administrador global função

Nesta etapa, você garantirá que dois usuários em seu locatário do Microsoft 365 tenham a **função Administrador global** habilitada.

- [Função interna de Administrador Global](/azure/active-directory/roles/permissions-reference#global-administrator).
- [Eleve o acesso para obter a função de Administrador Global](/azure/role-based-access-control/elevate-access-global-admin).

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a>Configurar o grupo aprovador de solicitação de consentimento do Microsoft Graph Data Connect

Nesta etapa, você configurará seu locatário do Microsoft 365 para habilitar o uso do Microsoft Graph Data Connect.

1. Abra um navegador e vá para o [Administração Microsoft 365 Portal](https://admin.microsoft.com/).

1. Na barra lateral de navegação, selecione **Grupos Ativos**.

    ![Uma captura de tela mostrando os grupos ativos no Centro de administração do Microsoft 365.](../concepts/images/data-connect-m365-act-grp.png)

1. Selecione o **botão Adicionar um** grupo.

1. Use o seguinte para criar o novo grupo **de segurança** habilitado para email e selecione o **botão** Adicionar.
   - **Tipo**: segurança habilitada para email

    ![Uma captura de tela mostrando um usuário selecionando a segurança habilitada para email para um novo grupo no Centro de administração do Microsoft 365.](../concepts/images/data-connect-m365-mail-sec.png)

   - **Nome**: Aprovadores de Solicitação de Consentimento

    ![Uma captura de tela mostrando que um usuário está dando ao grupo um nome de "Aprovadores de Solicitação de Consentimento" no Centro de administração do Microsoft 365.](../concepts/images/data-connect-m365-cons-apprv.png)

   - **Prefixo de Email**: consentrequestapprovers

    ![Uma captura de tela mostrando um usuário criando o endereço de email para o grupo criado anteriormente no Centro de administração do Microsoft 365.](../concepts/images/data-connect-m365-cons-apprv-pref.png)

1. **Pode levar até uma hora até que** o grupo recém-criado seja exibido na lista. Quando o grupo tiver sido criado, selecione-o.

1. Vá para **a opção Grupos ativos** novamente e pesquise o grupo que você acabou de criar.

1. Selecione o grupo e, na guia **Membros** , selecione **Exibir tudo e gerenciar membros**.

1. Adicione os dois usuários que você habilitou **a Administrador global** a esse novo grupo.

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a>Habilitar o Microsoft Graph Data Connect em seu locatário do Microsoft 365

Nesta etapa, você habilitará o serviço Microsoft Graph Data Connect em seu locatário do Microsoft 365.

1. Enquanto você ainda estiver conectado ao portal do Administração Microsoft 365, selecione o item de menu Configurações **> Organização**.

1. Selecione o **serviço Microsoft Graph Data Connect** .

    ![Uma captura de tela mostrando os "Serviços" na folha "Configurações da organização". Um usuário está alternando no serviço Microsoft Graph Data Connect no Centro de administração do Microsoft 365.](../concepts/images/data-connect-m365-mgdc-toggle.png)

1. Marque a caixa de seleção que diz ativar ou desativar o **Microsoft Graph Data Connect para toda a organização** habilitar o Data Connect.

    ![Uma captura de tela mostrando a caixa de seleção que você precisa marcar para habilitar o Data Connect para toda a organização.](../concepts/images/data-connect-m365-enable-mgdc-for-org.png)

1. Insira **aprovadores de** solicitação de consentimento (ou o nome do grupo criado anteriormente)  no grupo de usuários para tomar decisões de aprovação e selecione **Salvar**.
