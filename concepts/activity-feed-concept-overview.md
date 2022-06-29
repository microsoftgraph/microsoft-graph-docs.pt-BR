---
title: Usar a API do feed de atividades para habilitar experiências entre dispositivos
description: Usando o Microsoft Graph, você pode habilitar experiências que fluem perfeitamente entre dispositivos, criar atividades mais avançadas com Cartões Adaptáveis e ajudar a impulsionar o uso do aplicativo.
ms.localizationpriority: medium
ms.prod: project-rome
ms.openlocfilehash: dfe47f0d41ca978bac04a3ce1bb2a5c8889491b4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437034"
---
# <a name="use-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>Usar a API do feed de atividades no Microsoft Graph para habilitar experiências entre dispositivos

Atividades tornam os usuários mais produtivos ao ajudá-los a retomar rapidamente tarefas importantes em seu aplicativo entre dispositivos. A Microsoft ajuda a impulsionar a produtividade do usuário com seus aplicativos por meio de experiências como Linha do Tempo do Windows, Conjuntos do Windows, Cortana Pick up Where I left off e Microsoft Launcher, que são todos alimentados pelo feed de atividades.  Quando você usa atividades, essas experiências da Microsoft podem começar a gerar interações com seu aplicativo. Você também pode exibir as atividades nos seus aplicativos para ajudar os usuários retomarem o que estavam fazendo em qualquer dispositivo e qualquer plataforma, incluindo Windows, Android e iOS.

As seções a seguir descrevem os benefícios da integração com atividades.

## <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>Possibilite experiências com fluxo perfeito entre dispositivos Windows, Android, Linux e iOS

Ótimos aplicativos ajudam os usuários a fazer grandes coisas&mdash;, permitindo uma ampla variedade de cenários de criatividade, produtividade e entretenimento. Retornar a uma tarefa pode ser um desafio, especialmente quando uma pessoa quer continuar a tarefa em um dispositivo ou uma plataforma diferente. Incorporando atividades em aplicativos,&mdash;você pode ajudar os usuários a retornar às tarefas recentes rapidamente usando qualquer tela que seja útil, eles podem mudar da Web para o celular para a área de trabalho e voltar novamente. Com itens de histórico, os usuários podem ver facilmente quais atividades usaram mais recentemente, quando e por quanto tempo.

Cada atividade do usuário representa um único destino no seu aplicativo: uma página de produto, um programa de TV, um documento ou uma campanha atual em um jogo. Basta ter um link profundo para retomar a atividade em seu aplicativo. Use [obter atividades recentes para](/graph/api/projectrome-get-recent-activities) criar uma lista de produtos exibidos recentemente para seu aplicativo de compras ou uma lista de leitura atual para livros e artigos de notícias.

## <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>Crie atividades mais completas para qualquer experiência com Cartões adaptáveis

Ao renderizar atividades em experiências da Microsoft como a Linha do Tempo do Windows, elas são exibidas usando a estrutura [Cartão adaptável](https://adaptivecards.io/), que permite que você crie cartões belos e avançados para mostrar as atividades do seu aplicativo. Você também pode usar o SDK de Cartão Adaptável para renderizar cartões avançados em seu próprio aplicativo. Se você não fornecer um cartão adaptável para cada atividade, criaremos automaticamente um cartão de atividades simples com base no nome e no ícone do seu aplicativo, o campo Título obrigatório e um campo opcional Descrição.

## <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>Permitir que a Microsoft ajude a gerar mais uso para seu aplicativo com recursos que alcançam centenas de milhões de clientes

A integração com as atividades do usuário não só permite que os usuários retomem atividades em seu aplicativo perfeitamente, mas também um conjunto cada vez maior de experiências da Microsoft para Windows, iOS e Android&mdash;projetadas para impulsionar a produtividade do usuário e ajudar os usuários a interagir com seu aplicativo em todos os dispositivos. Ao usar o Microsoft Graph, é possível integrar-se com atividades de usuários apenas uma vez e alcançar centenas de milhões de clientes e dezenas de milhões de clientes em organizações que usam o Windows, além de produtos da Microsoft para dispositivos iOS e Android.

## <a name="see-also"></a>Confira também

- [Experiências entre dispositivos no Microsoft Graph](cross-device-concept-overview.md)
- [Usar a API de feed de atividades para retomar as atividades de um usuário entre dispositivos](/graph/api/resources/activity-feed-api-overview)
- [Publicar atividades e itens de histórico com uma solicitação usando deep insert](/graph/api/projectrome-put-activity#example-2---deep-insert)
- [Saiba mais sobre o Project Rome](/windows/project-rome/)
