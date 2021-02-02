---
title: Trabalhar com o Explorador do Graph
description: Saiba como usar alguns dos recursos importantes no Explorador do Graph.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: b4c669ae6983efe2082b623c3de5b019a049311d
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072384"
---
# <a name="working-with-graph-explorer"></a>Trabalhar com o Explorador do Graph

[O Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta de desenvolvedor que permite que você faça convenientemente solicitações da API REST do Microsoft Graph e veja as respostas correspondentes. Este artigo descreve como usar alguns dos recursos importantes no Explorador do Graph.

## <a name="consent-to-permissions"></a>Consentimento para permissões

O usuário ou administrador deve conceder ao Explorador do Graph as permissões corretas por meio de um processo de consentimento para acessar dados no Microsoft Graph. Consentir com permissões no Explorador  do Graph por  meio da guia Modificar permissões ou da opção Selecionar permissões na engrenagem de configurações ao lado do seu perfil quando você estiver entrar. A **guia Modificar permissões** lista todas as permissões de que você precisa para executar a consulta na barra de endereços. 

Para consentir com permissões:

1.  Selecione uma consulta de exemplo e execute-a.
2.  Selecione a **guia Modificar permissões.**
3.  Consulte a lista de permissões necessárias para executar a consulta.
4.  Selecione o botão de consentimento ao lado da permissão que você deseja consentir. 

![Captura de tela do Explorador do Graph com as etapas de consentimento para permissões realçadas](./images/modify-permissions.png)

O **recurso Modificar permissões** está atualmente em visualização, e algumas consultas podem estar sem permissões. Se as permissões não estão disponíveis  para uma consulta, a opção Selecionar permissões na engrenagem de configurações ao lado do seu perfil contém a lista de todas as permissões disponíveis:

1.  Vá para a engrenagem de configurações e clique **na opção Selecionar** permissões. Essa opção contém a lista de todas as permissões disponíveis.
2.  Na lista de todas as permissões, consenta com as que você deseja.

![Captura de tela do Explorador do Graph com a opção Selecionar permissões realçada](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>Obter um token de acesso ou autenticação

O Explorador do Graph inclui uma **guia de token** do Access que mostra seu token de acesso quando você está entrar. Na guia **token do Access,** você pode copiar o token se precisar usá-lo em seu aplicativo cliente REST favorito.

![Captura de tela da guia Token de Acesso no Explorador do Graph com o botão Copiar realçada](./images/access-token.png)

## <a name="copy-code-snippets"></a>Copiar trechos de código

Para cada consulta da API REST que você selecionar ou inserir no Explorador do Graph, você pode descobrir como chamar essa API em cada um dos quatro idiomas mostrados na guia **Trechos** de Código - C#, Java, JavaScript e Objective-C. 

![Captura de tela do Explorador do Graph com a guia trechos de código realçada](./images/code-snippets.png)

## <a name="ui-component-integration"></a>Integração de componentes da interface do usuário

O Graph Explorer inclui vários recursos para facilitar a implementação da interface do usuário. Reutilizar esses componentes em seus aplicativos também.

### <a name="microsoft-graph-toolkit-integration"></a>Integração com o Microsoft Graph Toolkit

O [Microsoft Graph Toolkit](/graph/toolkit/overview) é uma coleção de componentes da Web reutilizáveis e sem estrutura e auxiliares para acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais, com provedores internos que autenticam e buscam dados do Microsoft Graph.

O Graph Explorer fornece exemplos de consultas à API REST que correspondem aos componentes do Kit de Ferramentas do Microsoft Graph. Um ponto azul na guia do componente **Toolkit** indica que o Kit de Ferramentas fornece um componente para a consulta à API REST especificada no momento no Graph Explorer. Você pode copiar convenientemente o código do componente para seu aplicativo.

A tabela a seguir lista as consultas de exemplo que atualmente incluem um componente do Kit de Ferramentas.

| **Consulta de exemplo do Graph Explorer** | **URL do iFrame de exemplo do Kit de Ferramentas** |
| --- | --- |
| GET meu perfil | [https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| GET pessoas com quem trabalho | [https://mgt.dev/iframe.html?id=components-mgt-people—people](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| OBTER todas as minhas tarefas de planejador | [https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| GET meus eventos para a próxima semana | [https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| GET minha foto | [https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Captura de tela mostrando a guia Componentes do Kit de Ferramentas com o código para gerar o componente realçado](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>Integração de cartões adaptáveis

[Cartões adaptáveis](https://adaptivecards.io/) são trechos de interface do usuário que não são de plataforma, de autoria em JSON, que aplicativos e serviços podem trocar de forma aberta. Quando você executar uma consulta e um cartão adaptável estiver disponível, um ponto azul aparecerá na **guia Cartões adaptáveis.**

![Captura de tela da guia cartões adaptáveis no Explorador do Graph com os detalhes da resposta realçadas](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>Personalizar o tema no Explorador do Graph

Escolha o tema do Explorador do Graph selecionando a **opção Alterar tema** na engrenagem de configurações. As opções de tema são Claro, Escuro e Alto contraste.

![Captura de tela da opção Alterar tema no Explorador do Graph com as opções de tema realçadas](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a>Armazenar e compartilhar consultas

As consultas que são executados no Explorador do Graph são salvas por 30 dias na **guia** Histórico. Na guia Histórico, você pode:

1.  Exportar todos os itens de histórico no formato .har.
2.  Exclua todos os itens do histórico.
3.  Exibir este item de histórico.
4.  Execute esta consulta.
5.  Exporte esse item de histórico no formato .har.
6.  Exclua este item de histórico.

![Captura de tela da guia Histórico com opções realçadas](./images/storing-and-sharing-queries.png)

Para compartilhar consultas que você executar, clique no botão compartilhar consulta no painel de resposta e clique em **copiar.** Isso copia um link para compartilhar e permite que outras pessoas vejam sua consulta e os resultados.

![Captura de tela do Explorador do Graph com as opções de Compartilhamento e Cópia realçadas](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a>Recursos da interface do usuário do Graph Explorer

Collapse and expand the sidebar component in Graph Explorer when you want to widen the request and response area. Para fechar o componente da barra lateral, selecione o ícone de hambúrguer na parte superior esquerda da barra lateral.

![Screenshot of Graph Explorer with the expand and collapse options highlighted](./images/expand-collapse-sidebar-component.png)

Expanda e collapse the response preview by selecting the expand arrow in the response preview window.

![Screenshot of the response pane with the expand and collapse options highlighted](./images/expand-collapse-response-preview.png)

Acesse convenientemente o site do Programa para Desenvolvedores do Microsoft 365 a partir da interface do usuário do Graph Explorer para obter uma área de segurança gratuita com dados de exemplo para experimentar. Na engrenagem de configuração, selecione **Obter uma área de segurança com dados de exemplo.**

![Screenshot of Graph Explorer with the Get a sandbox with sample data option highlighted](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>Próximas etapas

- Visite [o Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) e explore as consultas de exemplo.
- Explore a [documentação do Microsoft Graph Toolkit.](/graph/toolkit/overview)
- Contribuir ou fornecer comentários no repositório [gitHub do Explorador do Graph.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)
