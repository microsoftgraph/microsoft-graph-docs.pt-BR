---
title: Autorização para APIs lerem os relatórios de uso do Microsoft 365.
description: Os dados de relatórios acessíveis por meio da API de relatórios do Microsoft Graph são confidenciais e protegidos por permissões e funções do Azure AD (Azure Active Directory).
author: kszb
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 8f02807287771607d327c46fc27949132e6a85e313f99620c76be2107ec85996
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54151722"
---
# <a name="authorization-for-apis-to-read-microsoft-365-usage-reports"></a>Autorização para APIs lerem os relatórios de uso do Microsoft 365.

Os dados do relatório acessíveis por meio da API de relatórios do Microsoft Graph são confidenciais. Em particular, os relatórios de uso do Microsoft 365 são protegidos tanto pelas permissões quanto pelas funções do Azure Active Directory (Azure AD). As informações neste artigo se aplicam à API de relatórios que lê os relatórios de uso do Microsoft 365.

As APIs que leem os relatórios de uso do Microsoft 365 oferecem suporte a dois tipos de autorização:

- **Autorização no nível do aplicativo** – permite que um aplicativo leia todos os relatórios de uso de serviço sem um usuário conectado. As permissões concedidas ao aplicativo determinam a autorização.
- **Permissão delegada pelo usuário** – permite que um aplicativo leia todos os relatórios de uso de serviço em nome do usuário conectado. Além do aplicativo ter recebido as permissões necessárias, o usuário deve ser membro de uma função de administrador limitada do Azure AD. Essa pode ser uma das seguintes funções: administrador da empresa, administrador do Exchange, administrador do SharePoint, administrador do Lync, Administrador de Serviço do Teams, Administrador de Comunicações do Teams, leitor global ou leitor de relatórios.

Se você estiver chamando as APIs do Explorador do Graph:

- O administrador de locatário do Azure AD deve conceder explicitamente o consentimento das permissões solicitadas ao aplicativo do Explorador do Graph.
- O usuário deve ser membro de uma função de administrador limitada no Azure AD, listada acima para autorização delegada pelo usuário.

>**Observação**: O Explorador do Graph não oferece suporte a autorização no nível de aplicativo.

Se você estiver chamando as APIs de um aplicativo:

- O administrador de locatário do Azure AD deve conceder explicitamente o consentimento ao aplicativo. Isso é necessário para autorização no nível de aplicativo e autorização delegada pelo usuário.
- Se você estiver usando uma autorização delegada pelo usuário, o usuário conectado deverá ser membro de uma função de administrador limitada no Azure AD.

## <a name="assign-azure-ad-roles-to-users"></a>Atribuir funções do Microsoft Azure AD aos usuários

Depois que um aplicativo receber permissões, todas as pessoas com acesso ao aplicativo (ou seja, membros do locatário do Azure AD) receberão as permissões concedidas. Para proteger ainda mais os dados de relatórios confidenciais, os administradores de locatários devem atribuir aos usuários do aplicativo as funções apropriadas do Azure AD. Para obter detalhes, confira [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles-azure-portal) e [Atribuir funções de administrador e não-administrador aos usuários com o Azure Active Directory](/azure/active-directory/active-directory-users-assign-role-azure-portal).

>**Observação:** você precisa ser um administrador de locatários para executar esta etapa.

Para atribuir uma função a um usuário:

1. Entre no [portal do Azure](https://portal.azure.com) (https://portal.azure.com).
2. Clique no ícone no canto superior esquerdo para expandir o menu do portal do Azure. Selecione **Azure Active Directory** > **Usuários**.
3. Clique no nome do usuário.
4. Escolha **Funções atribuídas** e, em seguida, **Adicionar atribuição**.
5. Escolha a função apropriada e clique em **Adicionar**.