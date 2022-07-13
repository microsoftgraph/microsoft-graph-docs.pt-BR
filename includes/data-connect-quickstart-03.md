---
ms.localizationpriority: medium
ms.openlocfilehash: 1fbb4d9778252b743e56b505683ed1d84fe4180e
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768188"
---
<!-- markdownlint-disable MD002 MD041 -->

Neste exercício, você criará, executará e aprovará um pipeline do Azure Data Factory para extrair dados do Microsoft 365 para um Blob de Armazenamento do Azure para processamento adicional.

## <a name="create-a-microsoft-azure-active-directory-application-registration"></a>Criar um registro Microsoft Azure Active Directory aplicativo

A primeira etapa é criar um aplicativo Azure AD que será usado como a entidade de segurança para executar o processo de extração de dados.

1. Abra um navegador e vá para o [Portal do Azure](https://portal.azure.com/).

1. Entre usando uma conta com direitos **Administrador global** seus locatários do Azure e do Microsoft 365.

1. Na barra lateral de navegação, selecione **Azure Active Directory** (Azure AD).

1. Na página Azure AD Visão geral, selecione **Registros de aplicativo** **na seção Gerenciar** do menu.

1. Selecione o **botão Novo registro** .

    ![Uma captura de tela mostrando Registros de aplicativo no serviço do Azure Active Directory no portal do Azure.](../concepts/images/data-connect-azure-aad-app-reg.png)

1. Use os valores a seguir para criar um novo aplicativo Azure AD e selecione **Registrar**.

   - **Nome**: Transferência de Dados do Microsoft Graph Data Connect
   - **Tipos de conta com suporte**: contas somente neste diretório organizacional.
   - **URI de redirecionamento**: deixe os valores padrão.

    ![Uma captura de tela mostrando as etapas para registrar um novo registro de aplicativo no portal do Azure.](../concepts/images/data-connect-aad-redirect-uri.png)

1. Localize **a ID do Aplicativo (cliente)** e copie-a, pois você precisará dela posteriormente neste tutorial. Isso será chamado de ID da entidade de serviço.

1. Localize **a ID do Diretório (** locatário) e copie-a, pois você precisará dela posteriormente neste tutorial. Isso será chamado de ID de locatário.

1. Na navegação da barra lateral, selecione **Certificados e segredos em** **Gerenciar**.

1. Selecione o **botão Novo segredo do cliente**. *Defina a* Descrição como qualquer nome, **defina Expira** como qualquer valor na lista suspensa e escolha **Adicionar**.

    ![Uma captura de tela mostrando o processo para criar um novo segredo do cliente no portal do Azure.](../concepts/images/data-connect-aad-certs-secrets.png)

    - Depois que o segredo do cliente for criado, salve o Valor  em algum lugar seguro, pois ele não estará mais disponível posteriormente e você precisará criar um novo.
    - Isso será referenciado como a chave de entidade de serviço.

1. Na barra lateral de navegação do aplicativo, selecione **Proprietários**.

1. Verifique se sua conta está listada como proprietário do aplicativo. Se ele não estiver listado como proprietário, adicione-o.

    ![Uma captura de tela mostrando um usuário verificando se sua conta está definida como proprietário para o registro de aplicativo no portal do Azure.](../concepts/images/data-connect-aad-app-owners.png)
