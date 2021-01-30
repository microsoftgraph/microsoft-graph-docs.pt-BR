---
title: Criar um aplicativo no Azure Active Directory
description: Criar um registro de aplicativo do Azure Active Directory para se comunicar com o Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 821cd6981ddb24e3917a4c0720f1c8c524081f54
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059564"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>Criar um aplicativo do Azure Active Directory para usar com o Kit de Ferramentas do Microsoft Graph

O Microsoft Graph, a API que você usa para se conectar ao Microsoft 365, é protegido com o OAuth 2.0. Para conectar seu aplicativo ao Microsoft 365, você precisará criar um aplicativo no Azure Active Directory (Azure AD) e conceder permissões a esse aplicativo para acessar recursos específicos em nome da pessoa que está usando seu aplicativo. Este tópico descreve como registrar e configurar um aplicativo Web para usar com o Microsoft Graph Toolkit.

## <a name="add-new-application-registration-in-azure-active-directory"></a>Adicionar novo registro de aplicativo no Azure Active Directory

Para criar um aplicativo no Azure Active Directory, você precisa adicionar um novo registro de aplicativo e configurar um nome de aplicativo e um local de URL.

Para criar o aplicativo no Azure Active Directory:

1. Vá para o portal do Azure em https://portal.azure.com .
1. No menu, selecione **Azure Active Directory**.
1. No menu do Azure Active Directory, selecione **Registros de aplicativo.**
1. No menu superior, selecione o **botão Novo** registro.
1. Insira o nome do seu aplicativo; por exemplo, `My M365 app` .
1. Para o tipo de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (qualquer diretório do **Azure AD - Multi-tenant)** e contas pessoais da Microsoft (por exemplo, Skype, Xbox) .
1. No campo **Redirecionar URI,** na lista suspenso, selecione **Web** e, no campo URL, insira `http://localhost:3000` .
1. Confirme as alterações selecionando o **botão** Registrar.

## <a name="enable-oauth-implicit-flow"></a>Habilitar fluxo implícito do OAuth

Na maioria dos casos, você usará o Microsoft Graph Toolkit em aplicativos do lado do cliente que consistem apenas em código do lado do cliente. Como os aplicativos do lado do cliente não podem armazenar segredos com segurança, você precisa usar o fluxo implícito do [OAuth,](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)que pressuou a identidade de um aplicativo com base em sua ID e URL.

1. No Portal do Azure, abra seu registro de aplicativo recém-criado.
1. No menu, escolha **Autenticação.**
1. Na seção **Concessão implícita,** habilitar **tokens do Access** e **opções de tokens de ID.**
1. Confirme suas alterações escolhendo o **botão** Salvar.

## <a name="next-steps"></a>Próximas etapas

- [Criar um aplicativo Web](./build-a-web-app.md) (javascript de java de java)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Usar o Kit de Ferramentas com o React](./use-toolkit-with-react.md)
- [Usar o Kit de Ferramentas com o Angular](./use-toolkit-with-angular.md)
