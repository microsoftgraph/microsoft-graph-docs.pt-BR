---
title: 'Kit de ferramentas do Microsoft Graph: Web Components da plataforma Microsoft Graph'
description: O kit de ferramentas do Microsoft Graph é uma coleção de resuable, componentes da Web e auxiliares de estrutura independente para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 348e08212010f66fdde5ee3b752fe901699fbaa9
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639546"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a>Kit de ferramentas do Microsoft Graph: Web Components da plataforma Microsoft Graph

O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares reutilizáveis da estrutura, que podem acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais à direita da caixa, com provedores internos que autenticam e buscam dados do Microsoft Graph.

O Microsoft Graph Toolkit torna fácil usar o Microsoft Graph em seu aplicativo. No exemplo abaixo, Confira como um usuário conectado e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes de [login](./components/login.md) e [agenda](./components/agenda.md) .

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>O que há no Microsoft Graph Toolkit?

### <a name="components"></a>Componentes

O kit de ferramentas do Microsoft Graph inclui uma coleção de componentes Web para as experiências mais compiladas com as APIs do Microsoft Graph.

|Componente|Descrição|
|---------|-----------|
|[Logon](./components/login.md)|Um botão e um controle de submenu para autenticar um usuário com a plataforma de identidade da Microsoft e exibir as informações de perfil do usuário em entrar.|
|[Pessoa](./components/person.md)|Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.|
|[Pessoas](./components/people.md)|Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.|
|[Agenda](./components/agenda.md)|Exibe eventos no calendário de um usuário ou grupo.|
|[Tarefas](./components/tasks.md)|Exibe e permite adicionar, remover, concluir ou editar tarefas do Microsoft Planner ou do Microsoft to-do.|
|[Seletor de pessoas](./components/people-picker.md)|Fornece a capacidade de Pesquisar pessoas e renderizar a lista de resultados.|
|[Cartão de pessoa](./components/person-card.md)|Um submenu usado no componente Person para exibir mais informações de perfil sobre um usuário.|
|[Get](./components/get.md)|Faça uma consulta GET para qualquer API do Microsoft Graph diretamente no HTML.|

### <a name="providers"></a>Provedores

Os componentes funcionam melhor quando usados com um [provedor](/providers/providers.md). Os provedores habilitam a autenticação e fornecem a implementação para adquirir os tokens de acesso para chamar as APIs do Microsoft Graph.

|Provedores|Descrição|
|---------|-----------|
|[MSAL](./providers/msal.md)|Usa MSAL. js para entrar em usuários e adquirir tokens para uso com o Microsoft Graph.|
|[SharePoint](./providers/sharepoint.md)|Autentica e fornece acesso do Microsoft Graph aos componentes dentro de Web Parts do SharePoint.|
|[Teams](./providers/teams.md)|Autentica e fornece acesso do Microsoft Graph aos componentes dentro das guias do Microsoft Teams.|
|[Acionista](./providers/proxy.md)|Permite o uso da autenticação de backend ao rotear todas as chamadas para o Microsoft Graph por meio do seu back-end.|
|[Personalizados](./providers/custom.md)|Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do seu aplicativo.|

## <a name="why-use-the-microsoft-graph-toolkit"></a>Por que usar o kit de ferramentas do Microsoft Graph?

O kit de ferramentas do Microsoft Graph disponibiliza a integração de experiências comuns que o Microsoft Graph em seu próprio aplicativo rápido e fácil.

:::row:::
   :::column span="":::
    **Tempo de desenvolvimento reduzido**

    O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece uma experiência de Microsoft365 é feita para você, sem a necessidade de personalização.
  :::column-end:::
  :::column span="":::
    **Funciona em qualquer lugar**

    Todos os componentes são baseados nos padrões da Web e funcionam de forma perfeita com qualquer navegador e Web Framework modernos (reagir, angulares, Vue, etc.). 
  :::column-end:::
  :::column span="":::
    **Linda, mas flexível**

    Os componentes foram projetados para serem parecidos com as experiências do Microsoft365, mas também podem ser personalizáveis usando [as propriedades personalizadas](./style.md) e [Templating](./templates.md)de CSS.
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Quem deve usá-lo?

O Microsoft Graph Toolkit é excelente para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo Web, guia do Microsoft Teams ou Web Part do SharePoint que se conecta e acessa os dados do Microsoft Graph.

## <a name="where-can-i-use-it"></a>Onde posso usá-lo?

O kit de ferramentas do Microsoft Graph é suportado nos seguintes navegadores.

|![Borda](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Borda**|**IE 11**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Próximas etapas

- Experimente os componentes no [playground](https://mgt.dev).
- [Introdução](get-started.md) ao Microsoft Graph Toolkit.
