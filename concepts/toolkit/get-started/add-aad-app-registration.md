---
title: Criar um aplicativo no Azure Active Directory
description: Criar um registro Azure Active Directory aplicativo para se comunicar com Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 4038b1dbdd124923f949cc48c4ebda75106365d74bd97dfee87466a58c34ea28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159663"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>Criar um Azure Active Directory para usar com o microsoft Graph Toolkit

O microsoft Graph, a API que você usa para se conectar ao Microsoft 365, está protegida com o OAuth 2.0. Para conectar seu aplicativo ao Microsoft 365, você precisará criar um aplicativo no Azure Active Directory (Azure AD) e conceder a esse aplicativo permissões para acessar recursos específicos em nome da pessoa que está usando seu aplicativo. Este tópico descreve como registrar e configurar um aplicativo Web a ser usado com o Microsoft Graph Toolkit.

## <a name="add-new-application-registration-in-azure-active-directory"></a>Adicionar novo registro de aplicativo no Azure Active Directory

Para criar um aplicativo no Azure Active Directory, você precisa adicionar um novo registro de aplicativo e configurar um nome de aplicativo e um local de URL.

Para criar o aplicativo em Azure Active Directory:

1. Vá para o portal do Azure em https://portal.azure.com .
1. No menu, selecione **Azure Active Directory**.
1. No menu Azure Active Directory, selecione **Registros de aplicativos**.
1. No menu superior, selecione o **botão Novo registro.**
1. Insira o nome do seu aplicativo; por exemplo, `My M365 app` .
1. Para o tipo de tipos de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (Qualquer diretório **do Azure AD - Multitenant) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.
1. No campo **Redirecionar URI,** no menu suspenso, selecione Aplicativo de Página Única **(SPA)** e, no campo URL, insira `http://localhost:3000` . Observação: se você estiver usando o Provedor MSAL e não o Provedor MSAL 2.0, precisará selecionar **Web** em vez de **SPA**.
1. Confirme as alterações selecionando o **botão Registrar.**

## <a name="enable-oauth-implicit-flow-only-for-msal-10-provider"></a>Habilitar o fluxo implícito OAuth (somente para provedor MSAL 1.0)

Na maioria dos casos, você usará o Microsoft Graph Toolkit em aplicativos do lado do cliente que consistem apenas em código do lado do cliente. Como os aplicativos do lado do cliente não podem armazenar segredos com segurança, você precisa usar o fluxo implícito [OAuth,](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)que pressu assume a identidade de um aplicativo com base em sua ID e URL.

1. No Portal do Azure, abra seu registro de aplicativo recém-criado.
1. No menu, escolha **Autenticação**.
1. Na seção **Concessão implícita,** habilita as **opções tokens do Access** e **tokens de ID.**
1. Confirme suas alterações escolhendo o **botão Salvar.**

## <a name="next-steps"></a>Próximas etapas

- [Criar um aplicativo Web](./build-a-web-app.md) (javaScript de baunilha)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Use o Toolkit com React](./use-toolkit-with-react.md)
- [Use o Toolkit com Angular](./use-toolkit-with-angular.md)
