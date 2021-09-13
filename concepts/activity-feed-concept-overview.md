---
title: Usar a API do feed de atividades no Microsoft Graph para habilitar experiências entre dispositivos
description: Quando você usa atividades, essas experiências da Microsoft podem começar a gerar interações com seu aplicativo. Você também pode exibir as atividades nos seus aplicativos para ajudar os usuários retomarem o que estavam fazendo em qualquer dispositivo e qualquer plataforma, incluindo Windows, Android e iOS.
ms.localizationpriority: medium
ms.prod: project-rome
ms.openlocfilehash: 4e820a4aeb5e99de709a1cb7d9f40bd5c38c200c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136205"
---
# <a name="using-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>Usar a API do feed de atividades no Microsoft Graph para habilitar experiências entre dispositivos

Atividades tornam os usuários mais produtivos ao ajudá-los a retomar rapidamente tarefas importantes em seu aplicativo entre dispositivos. A Microsoft ajuda a aumentar a produtividade dos usuários com seus aplicativos por meio de experiências como a Linha do Tempo do Windows, os Conjuntos do Windows, o recurso Continuar de onde parei da Cortana e o Microsoft Launcher, que são capacitados pelo feed de atividades.  Quando você usa atividades, essas experiências da Microsoft podem começar a gerar interações com seu aplicativo. Você também pode exibir as atividades nos seus aplicativos para ajudar os usuários retomarem o que estavam fazendo em qualquer dispositivo e qualquer plataforma, incluindo Windows, Android e iOS.

## <a name="why-integrate-with-activities"></a>Por que se integrar com atividades?
### <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>Possibilite experiências com fluxo perfeito entre dispositivos Windows, Android, Linux e iOS 
Bons aplicativos ajudam os usuários a fazerem coisas boas, possibilitando uma grande variedade de cenários de criatividade, produtividade e entretenimento. Retornar a uma tarefa pode ser um desafio, especialmente quando uma pessoa quer continuar a tarefa em um dispositivo ou uma plataforma diferente. Ao incorporar atividades em aplicativos, você pode ajudar os usuários a retornarem a tarefas recentes rapidamente usando qualquer tela que esteja disponível. É possível mover da Web para um dispositivo móvel, para um computador desktop e de volta para a Web. Com itens de histórico, os usuários podem ver facilmente quais atividades usaram mais recentemente, quando e por quanto tempo.   

Cada atividade do usuário representa um único destino no seu aplicativo: uma página de produto, um programa de TV, um documento ou uma campanha atual em um jogo. Basta ter um link profundo para retomar a atividade em seu aplicativo. Use o recurso [obter atividades recentes](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0) para criar uma lista de produtos visualizados recentemente para um aplicativo de compras ou uma lista de leitura atual para livros e artigos de notícias. 

### <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>Crie atividades mais completas para qualquer experiência com Cartões adaptáveis
Ao renderizar atividades em experiências da Microsoft como a Linha do Tempo do Windows, elas são exibidas usando a estrutura [Cartão adaptável](https://adaptivecards.io/), que permite que você crie cartões belos e avançados para mostrar as atividades do seu aplicativo. Você também pode usar o SDK de Cartão adaptável para renderizar cartões avançados em seu próprio aplicativo. Se você não fornecer um cartão adaptável para cada atividade, criaremos automaticamente um cartão de atividades simples com base no nome e no ícone do seu aplicativo, o campo Título obrigatório e um campo opcional Descrição. 

### <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>Permitir que a Microsoft ajude a gerar mais uso para seu aplicativo com recursos que alcançam centenas de milhões de clientes
A integração com as atividades do usuário permite que os usuários retomem facilmente atividades em seu aplicativo e também utilizem um conjunto crescente de experiências da Microsoft para o Windows, o iOS e o Android: experiências projetadas para aumentar a produtividade do usuário e ajudar os usuários a interagir com seu aplicativo em todos os dispositivos. Ao usar o Microsoft Graph, é possível integrar-se com atividades de usuários apenas uma vez e alcançar centenas de milhões de clientes e dezenas de milhões de clientes em organizações que usam o Windows, além de produtos da Microsoft para dispositivos iOS e Android.

## <a name="see-also"></a>Confira também

- [Experiências entre dispositivos no Microsoft Graph](cross-device-concept-overview.md)
- [Usar a API de feed de atividades para retomar as atividades de um usuário entre dispositivos](/graph/api/resources/activity-feed-api-overview?view=graph-rest-1.0)
- [Publicar atividades e itens de histórico com uma solicitação usando deep insert](/graph/api/projectrome-put-activity?view=graph-rest-1.0#example-2---deep-insert)
- [Saiba mais sobre o Project Rome](/windows/project-rome/)
