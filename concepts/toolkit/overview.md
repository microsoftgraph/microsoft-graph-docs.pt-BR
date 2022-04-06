---
title: 'Microsoft Graph Toolkit: Componentes da interface do usuário e provedores de autenticação para o Microsoft Graph'
description: O Microsoft Graph Toolkit é uma coleção de provedores de autenticação e componentes web reutilizáveis e agnósticos da estrutura para acessar e trabalhar com o Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 91de94be7ba84ead7d84c3eff0d10c89fc248b9c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589307"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a>Microsoft Graph Toolkit: Componentes da interface do usuário e provedores de autenticação para o Microsoft Graph 

O Microsoft Graph Toolkit é uma coleção de componentes e provedores de autenticação reutilizáveis e agnósticos para acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais imediatamente, com provedores internos que se autenticam com e buscam dados do Microsoft Graph.

O microsoft Graph Toolkit torna mais fácil usar o Microsoft Graph em seu aplicativo. No exemplo a seguir, um usuário e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes [Login](./components/login.md) e [Agenda](./components/agenda.md) .

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>O que há no microsoft Graph Toolkit?

### <a name="components"></a>Componentes

O microsoft Graph Toolkit inclui uma coleção de componentes da Web para as experiências mais comumente criadas com o microsoft Graph APIs. 

Os componentes também estão disponíveis como [React componentes](./get-started/mgt-react.md).

|Componente|Descrição|
|---------|-----------|
|[Logon](./components/login.md)|Um botão e um controle de sobrevoo para autenticar um usuário com a plataforma Microsoft Identity e exibir as informações de perfil do usuário ao entrar.|
|[Pessoa](./components/person.md)|Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.|
|[Pessoas](./components/people.md)|Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.|
|[Agenda](./components/agenda.md)|Exibe eventos no calendário de um usuário ou grupo.|
|[Se picker de pessoas](./components/people-picker.md)|Fornece a capacidade de pesquisar por pessoas e renderiza a lista de resultados.|
|[Cartão pessoal](./components/person-card.md)|Um flyout usado no componente da pessoa para exibir mais informações de perfil sobre um usuário.|
|[Arquivo](./components/file.md)|Representa um arquivo ou pasta com ícone, nome do arquivo, autor e muito mais.|
|[Lista de arquivos](./components/file-list.md)|Exibe uma lista de vários arquivos ou pastas.|
|[Get](./components/get.md)|Faça uma consulta GET para qualquer microsoft API do Graph diretamente em seu HTML.|
|[Se picker de canal](./components/teams-channel-picker.md)|Fornece a capacidade de pesquisar Microsoft Teams canais para selecionar um canal em uma lista renderizada de resultados.|
|[To Do](./components/todo.md)|Exibe e habilita a adição, remoção, conclusão ou edição de tarefas de Microsoft To Do.|
|[Tarefas](./components/tasks.md)|Exibe e habilita a adição, remoção, conclusão ou edição de tarefas de Microsoft Planner ou Microsoft To Do.|

### <a name="providers"></a>Provedores

[Os provedores](/providers/providers.md) habilitam a autenticação e fornecem a implementação para adquirir tokens de acesso em várias plataformas e expõem um cliente do Microsoft Graph para chamar as APIs do Microsoft Graph. Os componentes funcionam melhor quando usados com um provedor, mas os provedores podem ser usados por conta própria.

|Provedores|Descrição|
|---------|-----------|
|[MSAL](./providers/msal.md)|Usa msal.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.|
|[MSAL2](./providers/msal2.md)| Usa o msal-browser para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.|
|[Tron](./providers/electron.md)|Autentica e fornece à Microsoft Graph acesso a componentes dentro de aplicativos Detron|
|[SharePoint](./providers/sharepoint.md)|Autentica e fornece à Microsoft Graph acesso a componentes dentro de SharePoint Web Parts.|
|[Teams](./providers/teams.md)|Usa msal.js para entrar em usuários e adquirir tokens no cliente em Microsoft Teams guias.|
|[Teams MSAL2](./providers/teams-msal2.md)|Usa o msal-browser para entrar em usuários e adquirir tokens Microsoft Teams guias. Oferece suporte a Sign-On com back-back-back personalizado. |
|[Proxy](./providers/proxy.md)|Permite o uso da autenticação de back-end roteamento de todas as chamadas para a Microsoft Graph seu back-end.|
|[Personalizados](./providers/custom.md)|Crie um provedor personalizado para habilitar a autenticação e o acesso à Microsoft Graph com o código de autenticação existente do aplicativo.|

## <a name="why-use-the-microsoft-graph-toolkit"></a>Por que usar o microsoft Graph Toolkit?

O microsoft Graph Toolkit torna a integração de experiências comuns fornecidas pela Microsoft Graph em seu próprio aplicativo de forma rápida e fácil.

:::row:::
   :::column span="":::
    **Reduzir o tempo de desenvolvimento**

    O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece e parece uma experiência do Microsoft365 é feito para você, sem nenhuma personalização necessária.
  :::column-end:::
  :::column span="":::
    **Funciona em todos os lugares**

    Todos os componentes são baseados em padrões web e funcionam perfeitamente com qualquer navegador moderno e estrutura da Web (React, Angular, Vue etc.). 
  :::column-end:::
  :::column span="":::
    **Belo, mas flexível**

    Os componentes foram projetados para parecer experiências do Microsoft365, mas também são personalizáveis usando [propriedades personalizadas CSS](./customize-components/style.md) e [templating](./customize-components/templates.md).
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Who deve usá-lo?

O Microsoft Graph Toolkit é ótimo para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo que se conecta e acessa dados do Microsoft Graph, como:
- Aplicativo Web
- Microsoft Teams guia
- Aplicativo Web Progressivo (PWA)
- Aplicativo Detron
- SharePoint Web Part

## <a name="where-can-i-use-it"></a>Onde posso usá-lo?

O microsoft Graph Toolkit é suportado nos seguintes navegadores.

|![Borda](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Borda**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Próximas etapas

- Experimente os componentes do [playground](https://mgt.dev).
- [Introdução](./get-started/overview.md) com o microsoft Graph Toolkit.
- Confira o microsoft Graph Toolkit no [GitHub](https://aka.ms/mgt).
