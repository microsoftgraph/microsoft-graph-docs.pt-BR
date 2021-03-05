---
title: 'Microsoft Graph Toolkit: Componentes da interface do usuário e provedores de autenticação para o Microsoft Graph'
description: O microsoft graph Toolkit é uma coleção de provedores de autenticação e componentes web reutilizáveis e agnósticos da estrutura para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 01f406c288ebca1dde5c6b1577fd2acdc7631d5b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470533"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a>Microsoft Graph Toolkit: Componentes da interface do usuário e provedores de autenticação para o Microsoft Graph 

O microsoft graph Toolkit é uma coleção de componentes reutilizáveis, componentes de estrutura e provedores de autenticação para acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais imediatamente, com provedores internos que se autenticam com e buscam dados do Microsoft Graph.

A Toolkit do Microsoft Graph facilita o uso do Microsoft Graph em seu aplicativo. No exemplo a seguir, um usuário e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes [Login](./components/login.md) e [Agenda.](./components/agenda.md)

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>O que há no microsoft graph Toolkit?

### <a name="components"></a>Componentes

O microsoft graph Toolkit inclui uma coleção de componentes da Web para as experiências mais comumente criadas com as APIs do Microsoft Graph. 

Os componentes também estão disponíveis como [componentes do React.](./get-started/mgt-react.md)

|Componente|Descrição|
|---------|-----------|
|[Logon](./components/login.md)|Um botão e um controle de sobrevoo para autenticar um usuário com a plataforma Microsoft Identity e exibir as informações de perfil do usuário ao entrar.|
|[Pessoa](./components/person.md)|Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.|
|[Pessoas](./components/people.md)|Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.|
|[Agenda](./components/agenda.md)|Exibe eventos no calendário de um usuário ou grupo.|
|[Tarefas](./components/tasks.md)|Exibe e habilita a adição, remoção, conclusão ou edição de tarefas do Microsoft Planner ou Microsoft To Do.|
|[Seletor de pessoas](./components/people-picker.md)|Fornece a capacidade de pesquisar por pessoas e renderiza a lista de resultados.|
|[Cartão pessoal](./components/person-card.md)|Um flyout usado no componente da pessoa para exibir mais informações de perfil sobre um usuário.|
|[Get](./components/get.md)|Faça uma consulta GET para qualquer API do Microsoft Graph diretamente em seu HTML.|
|[Se picker de canal](./components/teams-channel-picker.md)|Fornece a capacidade de pesquisar canais do Microsoft Teams para selecionar um canal em uma lista renderizada de resultados.|
|[To Do](./components/todo.md)|Exibe e habilita a adição, remoção, conclusão ou edição de tarefas do Microsoft To Do.|

### <a name="providers"></a>Provedores

[Os provedores](/providers/providers.md) habilitam a autenticação e fornecem a implementação para adquirir tokens de acesso em várias plataformas e expõem um cliente do Microsoft Graph para chamar as APIs do Microsoft Graph. Os componentes funcionam melhor quando usados com um provedor, mas os provedores podem ser usados por conta própria.

|Provedores|Descrição|
|---------|-----------|
|[Msal](./providers/msal.md)|Usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.|
|[Tron](./providers/electron.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro de aplicativos Detron|
|[SharePoint](./providers/sharepoint.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro das Web Parts do SharePoint.|
|[Teams](./providers/teams.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro das guias do Microsoft Teams.|
|[Proxy](./providers/proxy.md)|Permite o uso da autenticação de back-end roteamento de todas as chamadas para o Microsoft Graph por meio do back-end.|
|[Personalizados](./providers/custom.md)|Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do aplicativo.|

## <a name="why-use-the-microsoft-graph-toolkit"></a>Por que usar o microsoft graph Toolkit?

A Toolkit do Microsoft Graph torna a integração de experiências comuns fornecidas pelo Microsoft Graph em seu próprio aplicativo de forma rápida e fácil.

:::row:::
   :::column span="":::
    **Reduzir o tempo de desenvolvimento**

    O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece e parece uma experiência do Microsoft365 é feito para você, sem nenhuma personalização necessária.
  :::column-end:::
  :::column span="":::
    **Funciona em todos os lugares**

    Todos os componentes são baseados em padrões da Web e funcionam perfeitamente com qualquer navegador moderno e estrutura da Web (React, Angular, Vue etc.). 
  :::column-end:::
  :::column span="":::
    **Belo, mas flexível**

    Os componentes são projetados para parecer experiências do Microsoft365, mas também são personalizáveis usando [propriedades personalizadas CSS](./customize-components/style.md) e [templating](./customize-components/templates.md).
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Quem deve usá-lo?

O microsoft graph Toolkit é ótimo para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo que se conecta e acessa dados do Microsoft Graph, como:
- Aplicativo Web
- Guia Microsoft Teams
- Aplicativo Web Progressivo (PWA)
- Aplicativo Detron
- Web Part do SharePoint

## <a name="where-can-i-use-it"></a>Onde posso usá-lo?

O microsoft graph Toolkit é suportado nos seguintes navegadores.

|![Borda](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Borda**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Próximas etapas

- Experimente os componentes no [playground](https://mgt.dev).
- [Começar a](./get-started/overview.md) trabalhar com o Microsoft Graph Toolkit.
- Confira o microsoft graph Toolkit [github](https://aka.ms/mgt).
