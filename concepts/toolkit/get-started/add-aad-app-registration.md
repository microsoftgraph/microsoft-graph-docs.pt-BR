---
title: Criar um aplicativo do Azure Active Directory
description: Criar um registro de aplicativo do Azure Active Directory para se comunicar com o Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 13b3a876e80e5c2437eba3d264053cdbbcbb5909
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982319"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>Criar um aplicativo do Azure Active Directory para uso com o kit de ferramentas do Microsoft Graph

O Microsoft Graph, a API que você usa para se conectar ao Microsoft 365, é protegido com o OAuth 2,0. Para conectar seu aplicativo ao Microsoft 365, você precisará criar um aplicativo no Azure Active Directory (Azure AD) e conceder a este aplicativo permissões para acessar recursos específicos em nome da pessoa que está usando seu aplicativo. Este tópico descreve como registrar e configurar um aplicativo Web para usar com o Microsoft Graph Toolkit.

## <a name="add-new-application-registration-in-azure-active-directory"></a>Adicionar novo registro de aplicativo no Azure Active Directory

Para criar um aplicativo no Azure Active Directory, você precisa adicionar um novo registro de aplicativo e, em seguida, configurar o nome do aplicativo e o local da URL.

Para criar o aplicativo no Azure Active Directory:

1. Vá para o portal do Azure em https://portal.azure.com .
1. No menu, selecione **Azure Active Directory**.
1. No menu do Azure Active Directory, selecione **registros de aplicativos**.
1. No menu superior, selecione o botão **novo registro** .
1. Insira o nome do seu aplicativo; para exampe, `My M365 app` .
1. Para o tipo de [tipos de conta com suporte](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), selecione **contas em qualquer diretório organizacional (qualquer diretório do Azure ad-multilocatário) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.
1. No campo **URI de redirecionamento** , na lista suspensa, selecione **Web** e, no campo URL, digite `https://localhost:3000` .
1. Confirme as alterações selecionando o botão **registrar** .

## <a name="enable-oauth-implicit-flow"></a>Habilitar o fluxo implícito do OAuth

Na maioria dos casos, você usará o Microsoft Graph Toolkit em aplicativos do lado do cliente que consistem apenas em código do lado do cliente. Como os aplicativos do lado do cliente não podem armazenar segredos com segurança, você precisa usar o [fluxo implícito do OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), que assume a identidade de um aplicativo com base em sua ID e URL.

1. No portal do Azure, abra seu registro de aplicativo recém-criado.
1. No menu, escolha **autenticação**.
1. Na seção **concessão implícita** , habilite os **tokens de acesso** e as opções de **token de ID** .
1. Confirme suas alterações escolhendo o botão **salvar** .

## <a name="next-steps"></a>Próximas etapas

- [Criar um aplicativo Web](./build-a-web-app.md) (JavaScript de baunilha)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Usar o kit de ferramentas reagir](./use-toolkit-with-react.md)
- [Usar o kit de ferramentas com angular](./use-toolkit-with-angular.md)
