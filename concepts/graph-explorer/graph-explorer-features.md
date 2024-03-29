---
title: Trabalhar com o Explorador do Graph
description: Utilize o Graph Explorer para fazer solicitações da API REST do Microsoft Graph e exibir as respostas correspondentes. Saiba como usar alguns dos recursos importantes no Explorador do Graph.
ms.localizationpriority: high
author: RabebOthmani
ms.openlocfilehash: 925bf7d42068be9141bc1b95c58edcd01ddfc8c8
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555797"
---
# <a name="work-with-graph-explorer"></a>Trabalhar com o Explorador do Graph

O [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta para desenvolvedores que permite fazer solicitações de API REST do Microsoft Graph de maneira conveniente e visualizar as respostas correspondentes. Este artigo descreve como usar alguns dos recursos importantes do Explorador do Graph.

Para obter uma visão geral, consulte [Usar o Explorador do Graph para experimentar as APIs do Microsoft Graph](/graph/graph-explorer/graph-explorer-overview).

## <a name="consent-to-permissions"></a>Consentimento para permissões

O usuário ou administrador deve conceder ao Explorador do Graph as permissões corretas utilizando um processo de consentimento para acessar dados no Microsoft Graph. Você pode consentir com as permissões no Explorador do Graph escolhendo a guia **Modificar permissões** ou a opção **Selecionar permissões** na engrenagem de configurações ao lado do seu perfil quando estiver conectado. A guia **Modificar permissões** lista todas as permissões necessárias para executar a consulta na barra de endereços. 

Para consentir as permissões:

1. Selecione uma consulta de exemplo e execute-a.
2. Selecione a guia **Modificar permissões**.
3. Consulte a lista de permissões necessárias para executar a consulta.
4. Selecione o botão **Consentimento** ao lado da permissão que você deseja consentir.

![Captura de tela do Explorador do Graph com as etapas de consentimento para permissões realçadas](./images/modify-permissions.png)

O recurso **Modificar permissões** está atualmente na versão prévia, e algumas consultas podem não ter permissões. Se não há permissões para uma consulta, a opção **Selecionar permissões** na engrenagem de configurações ao lado do seu perfil contém a lista de todas as permissões disponíveis:

1. Vá para a engrenagem de configurações e escolha a opção **Selecionar permissões**. Essa opção contém a lista de todas as permissões disponíveis.
2. Na lista de todas as permissões, concorde com as que deseja.

![Captura de tela do Explorador do Graph com a opção Selecionar permissões realçada](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>Obter um token de acesso ou autenticação

O Explorador do Graph inclui uma guia **Token de acesso** que mostra o token de acesso quando você está conectado. Na guia **Token de acesso**, você pode copiar o token se precisar usá-lo em seu aplicativo cliente REST favorito.

![Captura de tela da guia Token de acesso no Explorador do Graph com o botão Copiar realçado](./images/access-token.png)

## <a name="copy-code-snippets"></a>Copiar trechos de código

Para cada consulta da API REST que você selecionar ou inserir no Explorador do Graph, você pode encontrar como chamar essa API em cada um dos quatro idiomas exibidos na guia **Trechos de código**: C#, Java, JavaScript e Objective-C.

![Captura de tela do Explorador do Graph com a guia trechos de código realçada](./images/code-snippets.png)

## <a name="integrate-ui-components"></a>Integrar componentes da interface do usuário

O Explorador do Graph inclui vários recursos para facilitar a implementação da interface do usuário. Reutilize esses componentes em seus aplicativos também.

### <a name="microsoft-graph-toolkit-integration"></a>Integração do Kit de ferramentas do Microsoft Graph

O [Kit de ferramentas do Microsoft Graph](../toolkit/overview.md) é uma coleção de componentes da Web reutilizáveis e independentes de estrutura e auxiliares para acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais, com fornecedores internos que se autenticam e buscam dados do Microsoft Graph.

O Explorador do Graph fornece consultas de API REST de exemplos que correspondem aos componentes do Kit de ferramentas do Microsoft Graph. Um ponto azul na guia **Componente do kit de ferramentas** indica que o kit de ferramentas fornece um componente para a consulta de API REST atualmente especificada no Explorador do Graph. Você pode copiar facilmente o código do componente em seu aplicativo.

A tabela a seguir lista as consultas de exemplo que atualmente incluem um componente do kit de ferramentas.

| **Consulta de exemplo do Explorador do Graph** | **URL do iFrame de exemplo do kit de ferramentas** |
| --- | --- |
| GET meu perfil | [https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| OBTER pessoas com quem trabalho | [https://mgt.dev/iframe.html?id=components-mgt-people—people](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| OBTER todas as minhas tarefas do Planner | [https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| OBTER meus eventos da próxima semana | [https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| GET minha foto | [https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Captura de tela mostrando a guia Componente do kit de ferramentas com o código para gerar o componente realçado](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>Integração de cartões adaptáveis

Os [Cartões adaptáveis](https://adaptivecards.io/) são trechos da interface de usuário que não dependem da plataforma, criados em JSON, que os aplicativos e serviços podem dividir. Quando você executa uma consulta e um cartão adaptável está disponível, um ponto azul é exibido na guia **Cartões adaptáveis**.

![Captura de tela da guia cartões adaptáveis no Explorador do Graph com os detalhes da resposta realçados](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>Personalizar o tema do Explorador do Graph

Escolha o tema do Explorador do Graph selecionando a opção **Alterar tema** na engrenagem de configurações. As opções de tema são **Claro**, **Escuro** e **Alto contraste**.

![Captura de tela da opção Alterar tema no Explorador do Graph com as opções de tema realçadas](./images/change-theme.png)

## <a name="store-and-share-queries"></a>Armazenar e compartilhar consultas

As consultas executadas no Explorador do Graph são salvas por 30 dias na guia **Histórico**. Na guia **Histórico**, você pode:

1. Exportar todos os itens do histórico no formato `.har`.
2. Excluir todos os itens do histórico.
3. Visualizar um item do histórico.
4. Executar uma consulta.
5. Exportar um item do histórico no formato `.har`.
6. Excluir um item do histórico.

![Captura de tela da guia Histórico com opções realçadas](./images/storing-and-sharing-queries.png)

Para compartilhar as consultas que você executa, selecione o botão **Compartilhar** no painel de respostas e, em seguida, selecione **Copiar**. Isso copia um link para compartilhar que permite que outras pessoas vejam sua consulta e os resultados.

![Captura de tela do Explorador do Graph com as opções Compartilhar e Copiar realçadas](./images/share-query.png)

## <a name="use-graph-explorer-ui-features"></a>Usar os recursos da Interface do Usuário do Explorador do Graph

Para ampliar a área de solicitação e resposta, recolha e expanda o componente da barra lateral no Explorador do Graph. Para recolher o componente da barra lateral, selecione o ícone de hambúrguer na parte superior esquerda da barra lateral.

![Captura de tela do Explorador do Graph com as opções Expandir e Recolher realçadas](./images/expand-collapse-sidebar-component.png)

Para expandir e recolher a visualização da resposta, selecione a seta de expansão na janela de visualização da resposta.

![Captura de tela do painel de resposta com as opções Expandir e Recolher realçadas](./images/expand-collapse-response-preview.png)

Acesse convenientemente o site do Programa de Desenvolvedor do Microsoft 365 na interface do usuário do Explorador do Graph para obter uma área restrita gratuita com dados de exemplo para experimentar. Na engrenagem de configurações, selecione **Obter uma área restrita com dados de exemplo**.

![Captura de tela do Explorador do Graph com a opção Obter uma área de proteção com dados de exemplo realçada](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>Próximas etapas

- Visite [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) e explore as consultas de exemplo.
- Explore a [Documentação do Kit de ferramentas do Microsoft Graph](../toolkit/overview.md).
- Contribua ou forneça comentários no [Repositório GitHub do Explorador do Graph](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
