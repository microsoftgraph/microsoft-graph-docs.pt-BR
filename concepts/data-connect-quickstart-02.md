---
ms.localizationpriority: medium
ms.openlocfilehash: 83869d63084f19e8c93e61dc0d4524a53217c30c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289503"
---
<!-- markdownlint-disable MD002 MD041 -->

Antes de usar Conexão de Dados do Microsoft Graph pela primeira vez, você precisa configurar seu Microsoft 365 locatário. Isso envolve a adição do serviço e a configuração de um grupo de segurança com permissões para aprovar solicitações de extração de dados.

## <a name="grant-azure-ad-users-the-global-administrator-role"></a>Conceder aos usuários do Azure AD a função de administrador global

Nesta etapa, você garantirá que dois usuários em seu Microsoft 365 locatário tenham a **função de** administrador global habilitada.

- [Função de administrador global integrado](/azure/active-directory/roles/permissions-reference#global-administrator).
- [Elevar o acesso para obter a função administrador global](/azure/role-based-access-control/elevate-access-global-admin).

## <a name="configure-microsoft-graph-data-connect-consent-request-approver-group"></a>Configurar Conexão de Dados do Microsoft Graph grupo aprovador de solicitação de consentimento

Nesta etapa, você configurará seu locatário Microsoft 365 para habilitar o uso de Conexão de Dados do Microsoft Graph.

1. Abra um navegador e vá para seu [Administração Microsoft 365 Portal](https://admin.microsoft.com/).

1. Na navegação da barra lateral, selecione **Grupos ativos**.

    ![Uma captura de tela mostrando os grupos ativos no Centro de administração do Microsoft 365.](images/data-connect-m365-act-grp.png)

1. Selecione o **botão Adicionar um grupo.**

1. Use o seguinte para criar o novo grupo de segurança habilitado para **email** e selecione o **botão Adicionar.**
   - **Tipo**: segurança habilitada para email

    ![Uma captura de tela mostrando um usuário selecionando a segurança habilitada para email para um novo grupo no Centro de administração do Microsoft 365.](images/data-connect-m365-mail-sec.png)

   - **Nome**: Aprovadores de Solicitação de Consentimento

    ![Uma captura de tela mostrando um usuário está dando ao grupo um nome de "Aprovadores de Solicitação de Consentimento" no Centro de administração do Microsoft 365.](images/data-connect-m365-cons-apprv.png)

   - **Prefixo de Email**: consentrequestapprovers

    ![Uma captura de tela mostrando um usuário criando o endereço de email para o grupo criado anteriormente no Centro de administração do Microsoft 365.](images/data-connect-m365-cons-apprv-pref.png)

1. **Pode levar até uma hora até** o grupo recém-criado aparecer na lista. Quando o grupo tiver sido criado, selecione-o.

1. Vá para a **opção Grupos ativos** novamente e procure o grupo que você acabou de criar.

1. Selecione o grupo e, na guia **Membros,** selecione **Exibir tudo e gerenciar membros**.

1. Adicione os dois usuários que você habilitaram a **função de** administrador global a esse novo grupo.

## <a name="enable-microsoft-graph-data-connect-in-your-microsoft-365-tenant"></a>Habilitar Conexão de Dados do Microsoft Graph no seu locatário Microsoft 365 usuário

Nesta etapa, você habilita o serviço Conexão de Dados do Microsoft Graph em seu locatário Microsoft 365 cliente.

1. Enquanto você ainda estiver Administração Microsoft 365 portal, selecione o item de menu configurações **Configurações > Org.**

1. Selecione o **Conexão de Dados do Microsoft Graph** serviço.

    ![Uma captura de tela mostrando o "Serviços" na folha "Configurações da organização". Um usuário está toggling on the Conexão de Dados do Microsoft Graph service in the Centro de administração do Microsoft 365.](images/data-connect-m365-mgdc-toggle.png)

1. Selecione a caixa de seleção que diz **Conexão de Dados do Microsoft Graph ativar ou** desativar para toda a sua organização habilitar dados Conexão.

    ![Uma captura de tela mostrando a caixa de seleção que você precisa marcar para habilitar a Conexão dados para toda a sua organização.](images/data-connect-m365-enable-mgdc-for-org.png)

1. Insira **Aprovadores de** Solicitação de Consentimento (ou o  nome do grupo criado anteriormente) no grupo de usuários para tomar decisões de aprovação e selecione **Salvar**.
