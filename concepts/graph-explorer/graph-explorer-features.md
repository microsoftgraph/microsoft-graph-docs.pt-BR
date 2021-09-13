---
title: Trabalhar com Graph Explorer
description: Saiba como usar alguns dos recursos importantes no Graph Explorer.
ms.localizationpriority: medium
author: bettirosengugi
ms.openlocfilehash: 97c4f3ccd0fdfd08da7f4696419df813f19840e3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59014325"
---
# <a name="working-with-graph-explorer"></a>Trabalhar com Graph Explorer

[Graph Explorer é](https://developer.microsoft.com/graph/graph-explorer/) uma ferramenta de desenvolvedor que permite que você faça convenientemente solicitações de API REST da Microsoft Graph exibir respostas correspondentes. Este artigo descreve como usar alguns dos recursos importantes no Graph Explorer.

## <a name="consent-to-permissions"></a>Consentimento para permissões

O usuário ou administrador deve conceder Graph permissões corretas ao Explorer por meio de um processo de consentimento para acessar dados no Microsoft Graph. Consenta com permissões no Graph Explorer  por meio da  guia Modificar permissões ou da opção Selecionar permissões na engrenagem de configurações ao lado do seu perfil quando você estiver dentro. A **guia Modificar permissões** lista todas as permissões que você precisa para executar a consulta na barra de endereços. 

Para consentir as permissões:

1.  Selecione uma consulta de exemplo e execute-a.
2.  Selecione a **guia Modificar permissões.**
3.  Consulte a lista de permissões necessárias para executar a consulta.
4.  Selecione o botão de consentimento ao lado da permissão que você deseja consentir. 

![Captura de tela do Graph Explorer com as etapas de consentimento para permissões realçadas](./images/modify-permissions.png)

O **recurso Modificar permissões** está atualmente em visualização, e algumas consultas podem estar faltando permissões. Se não há permissões para uma consulta, a opção **Selecionar** permissões na engrenagem de configurações ao lado do seu perfil contém a lista de todas as permissões disponíveis:

1.  Vá para a engrenagem de configurações e clique na **opção Selecionar** permissões. Essa opção contém a lista de todas as permissões disponíveis.
2.  Na lista de todas as permissões, consenta com as que você deseja.

![Captura de tela do Graph Explorer com a opção Selecionar permissões realçada](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>Obter um token de acesso ou autenticação

Graph O Explorer inclui uma **guia de tokens do Access** que mostra seu token de acesso quando você está dentro. Na guia **Token de Acesso,** você pode copiar o token se precisar usá-lo em seu aplicativo cliente REST favorito.

![Captura de tela da guia Token de Acesso no Graph Explorer com o botão Copiar realçada](./images/access-token.png)

## <a name="copy-code-snippets"></a>Copiar trechos de código

Para cada consulta da API REST que você selecionar ou inserir no Graph Explorer, você pode encontrar como chamar essa API em cada um dos quatro idiomas exibidos na guia **Trechos** de código - C#, Java, JavaScript e Objective-C. 

![Captura de tela do Graph Explorer com a guia trechos de código realçadas](./images/code-snippets.png)

## <a name="ui-component-integration"></a>Integração de componentes da interface do usuário

Graph O Explorer inclui vários recursos para facilitar a implementação da interface do usuário. Reutilizar esses componentes em seus aplicativos também.

### <a name="microsoft-graph-toolkit-integration"></a>Integração Graph Toolkit Microsoft

O [Microsoft Graph Toolkit](../toolkit/overview.md) é uma coleção de componentes web reutilizáveis e agnósticos e auxiliares para acessar e trabalhar com o Microsoft Graph. Os componentes são totalmente funcionais, com provedores internos que se autenticam com e buscar dados da Microsoft Graph.

Graph O Explorer fornece consultas de API REST de exemplo que correspondem aos componentes Graph Toolkit Microsoft. Um ponto azul na guia **Toolkit componente** indica que o Toolkit fornece um componente para a consulta da API REST especificada no Graph Explorer. Você pode copiar convenientemente o código do componente para seu aplicativo.

A tabela a seguir lista as consultas de exemplo que atualmente incluem um Toolkit componente.

| **Graph Consulta de exemplo do Explorer** | **Toolkit exemplo de URL iFrame** |
| --- | --- |
| GET meu perfil | [https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| OBTER pessoas com quem trabalho | [https://mgt.dev/iframe.html?id=components-mgt-people—people](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| OBTER todas as minhas tarefas do planejador | [https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| OBTER meus eventos para a próxima semana | [https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| GET minha foto | [https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Captura de tela mostrando a guia Toolkit componentes com o código para gerar o componente realçado](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>Integração de cartões adaptáveis

[Cartões adaptáveis](https://adaptivecards.io/) são trechos de plataforma agnósticos da interface do usuário, de autoria do JSON, que aplicativos e serviços podem trocar abertamente. Quando você executar uma consulta e um cartão adaptável estiver disponível, um ponto azul aparecerá na **guia Cartões Adaptáveis.**

![Captura de tela da guia cartões adaptáveis no Graph Explorer com os detalhes da resposta realçados](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>Personalizar o tema no Graph Explorer

Escolha o tema do Graph Explorer selecionando a opção **Alterar tema** na engrenagem de configurações. As opções de tema são Light, Dark e High contrast.

![Captura de tela da opção Alterar tema no Graph Explorer com as opções de tema realçadas](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a>Armazenar e compartilhar consultas

As consultas são Graph Explorer são salvas por 30 dias na **guia** Histórico. Na guia Histórico, você pode:

1.  Exportar todos os itens de histórico no formato .har.
2.  Exclua todos os itens de histórico.
3.  Exibir esse item de histórico.
4.  Execute essa consulta.
5.  Exporte esse item de histórico no formato .har.
6.  Exclua esse item de histórico.

![Captura de tela da guia Histórico com opções realçadas](./images/storing-and-sharing-queries.png)

Para compartilhar consultas que você executar, clique no botão compartilhar consulta no painel de resposta e clique em **copiar**. Isso copia um link para compartilhar e permitir que outras pessoas vejam sua consulta e os resultados.

![Captura de tela do Graph Explorer com as opções Compartilhar e Copiar realçadas](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a>Graph Recursos da interface do usuário do Explorer

Rebaixe e expanda o componente da barra lateral no Graph Explorer quando quiser ampliar a área de solicitação e resposta. Para fechar o componente da barra lateral, selecione o ícone de hambúrguer na parte superior esquerda da barra lateral.

![Captura de tela do Graph Explorer com as opções de expansão e colapso realçadas](./images/expand-collapse-sidebar-component.png)

Expanda e ressule a visualização de resposta selecionando a seta de expansão na janela de visualização de resposta.

![Captura de tela do painel de resposta com as opções de expansão e colapso realçadas](./images/expand-collapse-response-preview.png)

Convenientemente, acesse o site Microsoft 365 programa de desenvolvedor da interface do usuário do Graph Explorer para obter uma área de segurança gratuita com dados de exemplo para testar. Na engrenagem de configuração, selecione **Obter uma área de segurança com dados de exemplo.**

![Captura de tela do Graph Explorer com a opção Obter uma área de proteção com dados de exemplo realçada](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>Próximas etapas

- Visite [Graph Explorer e](https://developer.microsoft.com/graph/graph-explorer/) explore as consultas de exemplo.
- Explore a [documentação do Microsoft Graph Toolkit](../toolkit/overview.md).
- Contribuir ou fornecer comentários no [Graph Explorer GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
