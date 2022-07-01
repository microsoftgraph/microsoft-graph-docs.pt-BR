---
title: visão geral do Kit de ferramentas do Microsoft Graph
description: Use o Kit de Ferramentas do Microsoft Graph para encontrar provedores de autenticação e componentes Web reutilizáveis e independentes de estrutura para acessar e trabalhar com o Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: a448d79a789f142a2e05bca0e4096db9df127158
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577802"
---
# <a name="microsoft-graph-toolkit-overview"></a>visão geral do Kit de ferramentas do Microsoft Graph 

Kit de ferramentas do Microsoft Graph é uma coleção de componentes e fornecedores de autenticação reutilizáveis e agnósticos de quadro para acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais de fábrica, com fornecedores integrados que se autenticam com e buscam dados do Microsoft Graph.

O Kit de ferramentas do Microsoft Graph facilita o uso do Microsoft Graph em sua aplicação. No exemplo a seguir, um usuário conectado e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes [Logon](./components/login.md) e [Agenda](./components/agenda.md) .

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs).

## <a name="whats-in-microsoft-graph-toolkit"></a>O que há no Kit de Ferramentas do Microsoft Graph?

### <a name="components"></a>Componentes

O Kit de Ferramentas do Microsoft Graph inclui uma coleção de componentes da Web para as experiências mais comumente criadas alimentadas pelas APIs do Microsoft Graph.

Os componentes também estão disponíveis como [React componentes](./get-started/mgt-react.md).

|Componente|Descrição|
|---------|-----------|
|[Logon](./components/login.md)|Um botão e um controle de submenu para autenticar um usuário com a plataforma de Identidade da Microsoft e exibir as informações de perfil do usuário ao entrar.|
|[Pessoa](./components/person.md)|Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.|
|[Pessoas](./components/people.md)|Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.|
|[Agenda](./components/agenda.md)|Exibe eventos no calendário de um usuário ou grupo.|
|[Seletor de pessoas](./components/people-picker.md)|Fornece a capacidade de pesquisar por pessoas e renderiza a lista de resultados.|
|[Cartão pessoal](./components/person-card.md)|Um submenu usado no componente pessoa para exibir mais informações de perfil sobre um usuário.|
|[Arquivo](./components/file.md)|Representa um arquivo ou pasta com um ícone, um nome de arquivo, um autor e muito mais.|
|[Lista de arquivos](./components/file-list.md)|Exibe uma lista de vários arquivos ou pastas.|
|[Get](./components/get.md)|Permite que você faça uma consulta GET para qualquer microsoft API do Graph diretamente em seu HTML.|
|[Seletor de canal](./components/teams-channel-picker.md)|Fornece a capacidade de pesquisar canais do Microsoft Teams para selecionar um canal em uma lista renderizada de resultados.|
|[To Do](./components/todo.md)|Exibe e habilita a adição, remoção, conclusão ou edição de tarefas do Microsoft To Do.|
|[Tarefas](./components/tasks.md)|Exibe e habilita a adição, remoção, conclusão ou edição de tarefas do Microsoft Planner ou Microsoft To Do.|

### <a name="providers"></a>Provedores

[Os provedores](./providers/providers.md) habilitam a autenticação, fornecem a implementação para adquirir tokens de acesso em várias plataformas e expõem um cliente do Microsoft Graph para chamar as APIs do Microsoft Graph. Os componentes funcionam melhor quando usados com um provedor, mas os provedores podem ser usados por conta própria.

|Provedores|Descrição|
|---------|-----------|
|[MSAL](./providers/msal.md)|Usa msal.js para conectar usuários e adquirir tokens para usar com o Microsoft Graph.|
|[MSAL2](./providers/msal2.md)| Usa o msal-browser para conectar usuários e adquirir tokens para usar com o Microsoft Graph.|
|[Elétron](./providers/electron.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro de aplicativos Electron.|
|[SharePoint](./providers/sharepoint.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro de Web Parts do SharePoint.|
|[Teams](./providers/teams.md)|Usa msal.js para conectar usuários e adquirir tokens no cliente nas guias do Microsoft Teams.|
|[Teams MSAL2](./providers/teams-msal2.md)|Usa o msal-browser para conectar usuários e adquirir tokens nas guias do Microsoft Teams. Dá suporte ao SSO (logon único) com um back-end personalizado. |
|[Proxy](./providers/proxy.md)|Permite o uso da autenticação de back-end roteando todas as chamadas para o Microsoft Graph por meio do back-end.|
|[Personalizados](./providers/custom.md)|Cria um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph usando o código de autenticação existente do aplicativo.|

## <a name="why-use-microsoft-graph-toolkit"></a>Por que usar o Kit de Ferramentas do Microsoft Graph?

O Kit de Ferramentas do Microsoft Graph permite que você integre de forma rápida e fácil experiências comuns da plataforma Microsoft Graph em seu próprio aplicativo. O kit de ferramentas:

- **Reduz o tempo de desenvolvimento**. O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece e se parece com uma experiência do Microsoft 365 é feito para você, sem necessidade de personalização.

- **Funciona em todos os lugares**. Todos os componentes são baseados em padrões da Web e funcionam perfeitamente com qualquer navegador moderno e estrutura da Web (como React, Angular ou Vue). 

- **É bonita, mas flexível**. Os componentes são projetados para parecer experiências do Microsoft 365, mas também são personalizáveis usando propriedades [personalizadas css](./customize-components/style.md) e [modelagem](./customize-components/templates.md).

## <a name="who-should-use-it"></a>Quem deve usá-lo?

O Kit de Ferramentas do Microsoft Graph é ótimo para desenvolvedores de todos os níveis de experiência que querem desenvolver um aplicativo que se conecta e acessa dados do Microsoft Graph, como:
- Aplicativo Web
- Guia Microsoft Teams
- PWA (Aplicativo Web Progressivo)
- Aplicativo electron
- Web Part do SharePoint

## <a name="where-can-i-use-it"></a>Onde posso usá-lo?

O Kit de Ferramentas do Microsoft Graph tem suporte nos seguintes navegadores:

|![Borda](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Borda**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Próximos passos

- Experimente os componentes do [playground](https://mgt.dev).
- [Introdução ao](./get-started/overview.md) Kit de Ferramentas do Microsoft Graph.
- Confira o Kit de Ferramentas do Microsoft Graph [no GitHub](https://aka.ms/mgt).
