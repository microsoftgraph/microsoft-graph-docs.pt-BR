---
title: Provedor de eletrônica
description: O provedor MSAL para o Eletrônica usa o msal-node para entrar nos usuários e adquirir tokens para usar com o Microsoft Graph.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: a9e391f96988f8beaf8395e872a6efa08efca8f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471419"
---
# <a name="electron-provider"></a>Provedor de eletrônica

O provedor Demão usa [o nó msal](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph em um aplicativo Demão.

Para saber mais sobre provedores de autenticação, consulte [provedores](./providers.md).

## <a name="get-started"></a>Introdução
### <a name="install-the-packages"></a>Instalar os pacotes

```bash
npm install @microsoft/mgt-element @microsoft/mgt-electron-provider
```
Você precisa inicializar oTronProvider no processo de renderização (front-end) e oTronAuthenticator no processo principal (back-end).


### <a name="initializing-electronprovider-in-the-renderer-process-rendererts"></a>Inicializando oTronProvider no processo de renderizador (renderer.ts)

OTronProvider é responsável por se comunicar com oTronAuthenticator (no processo principal) para solicitar tokens de acesso e receber informações sobre o estado conectado que são necessárias para que os componentes funcionem. 

```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-the-main-process-maints"></a>Inicializando o EletrônicaAuthenticator no processo principal (main.ts)

OTronAuthenticator é responsável por configurar as variáveis de configuração para autenticação MSAL, adquirir tokens de acesso e se comunicar com oTronProvider.
Inicializar oTronAuthenticator no processo principal e configurar as variáveis de configuração, como id do cliente.

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 

let config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  authority: '<your_authority_url>', //optional
  mainWindow: mainWindow, 
  scopes: ['user.read'] //We recommend pre-consenting all the required scopes on the Azure portal
};

ElectronAuthenticator.initialize(config);
```
 
| Atributo    | Descrição                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| clientId    | ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente). Obrigatório.                                                                                                                                                                                                           |                                                                                                                                                                               |
| escopos       | Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar. Recomendado.                                                                                                                                                                                     |
| authority    | Cadeia de caracteres de autoridade - padrão é a autoridade comum. Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |                                                                                                                                                                                          |
| mainWindow  | Instância do BrowserWindow principal que requer autenticação.|
| cachePlugin | Plug-in de cache que você gostaria de usar para armazenamento persistente de tokens. Consulte [Extensões de Autenticação da Microsoft para Nó](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions). Opcional. | 

>**Observação:** Atualmente, o provedor não dá suporte a suporte incremental. Como prática prática, certifique-se de concordar com todos os escopos necessários aos componentes.
    
## <a name="create-an-appclient-id"></a>Criar uma ID de aplicativo/cliente

### <a name="add-new-application-registration-in-azure-active-directory-to-get-a-client-id"></a>Adicionar novo registro de aplicativo no Azure Active Directory para obter uma ID do cliente

Para criar um aplicativo no Azure Active Directory, adicione um novo registro de aplicativo e configure um nome de aplicativo e URI de redirecionamento.

Para criar o aplicativo no Azure Active Directory:

1. Vá para o [portal do Azure](https://portal.azure.com).
1. No menu, selecione **Azure Active Directory**.
1. No menu do Azure Active Directory, selecione **Registros de aplicativos**.
1. No menu superior, selecione o **botão Novo registro.**
1. Insira o nome do seu aplicativo; por exemplo, `My Electron-App` .
1. Para o tipo de tipos de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (Qualquer diretório do **Azure AD - Multitenant) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.
1. No campo **Redirecionar URI,** no menu suspenso, selecione **Cliente público/nativo (área** de trabalho móvel &) e, no campo URL, digite `msal://redirect` .
1. Confirme as alterações selecionando o **botão Registrar.**

## <a name="next-steps"></a>Próximas etapas

* Confira o tutorial passo a passo para [criar um aplicativo de eletrônica.](../get-started/build-an-electron-app.md)
* Dê uma olhada em um [aplicativo Detron de](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) exemplo que mostra como usar o provedor Demão.
