---
title: Experiências entre dispositivos no Microsoft Graph
description: Use o Microsoft Graph para acessar as atividades e dispositivos que pertencem aos seus clientes e habilitar experiências avançadas centradas em humanos que cruzam dispositivos e plataformas.
ms.localizationpriority: high
ms.prod: project-rome
ms.custom: scenarios:getting-started
ms.openlocfilehash: a7f291efd527883a5cb37d377a8358471bebb834
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440919"
---
# <a name="cross-device-experiences-in-microsoft-graph"></a>Experiências entre dispositivos no Microsoft Graph

No mundo atual, com tantos dispositivos, a forma como os clientes usam os dispositivos abrange diferentes plataformas e formatos: eles podem ler as notícias de manhã no tablet, ler os emails no celular no caminho para o trabalho e usar computadores de mesa no trabalho. À noite, podem assistir a filmes em seus consoles de mídia domésticos e usar alto-falantes inteligentes para ouvir as notícias do dia. O cliente comum utiliza diversos dispositivos e plataformas ao longo do dia.

No passado, o formato gerava tipos diferentes de comportamento entre os clientes. No entanto, os clientes de hoje, que usam diversos dispositivos, realizam todas as atividades em todos os seus dispositivos. As tarefas executadas diariamente (seja em casa com a família ou no trabalho com colegas) não são inerentemente centradas no dispositivo, mas, em vez disso, **centradas em humanos**. Os clientes querem poder usar qualquer tela que esteja disponível, independentemente da origem da entrada. Na verdade, eles geralmente acham que todo dispositivo tem um limite claro e usar vários dispositivos para executar uma tarefa requer ações artificiais, como enviar um email para si mesmo ou usar pen drives. Os clientes se desgastam ao passar de um dispositivo para outro e, às vezes, tarefas importantes são perdidas devido a essa mudança de contexto. Isso também é um desafio para desenvolvedores, pois, quando os clientes sentem esse desgaste ao usar um aplicativo, envolvem-se menos com ele.

A Microsoft está criando uma plataforma para possibilitar experiências que vão além de um único dispositivo, para que o cliente possa harmonizar os vários dispositivos &mdash;permitindo que você crie cenários **centrados em humanos** que se movem com o usuário e reduzem os limites entre os dispositivos, independentemente do formato ou da plataforma. O Microsoft Graph fornece um ponto de extremidade unificado para dar a você acesso aos dados do Azure Active Directory e do Microsoft 365. Agora, por meio do Microsoft Graph, você pode também acessar as atividades e os dispositivos que pertencem aos seus clientes e gerar experiências centradas em humanos que sejam executadas em vários dispositivos e plataformas.

## <a name="why-invest-in-cross-device-experiences"></a>Por que investir em experiências em diversos dispositivos?

### <a name="let-customers-pick-up-where-they-leave-off-with-the-activity-feed-api"></a>Permita que os clientes retomem o trabalho de onde pararam com a API do feed de atividades

Com as atividades, você pode capturar as tarefas exclusivas dos usuários do seu aplicativo, que são transmitidas facilmente para qualquer plataforma e dispositivo, permitindo que eles retomem o trabalho na tela de sua preferência. Usando o feed de atividades, você pode criar um modo de exibição, voltado para as necessidades humanas, das tarefas mais importantes para os usuários, ajudando a reduzir o desgaste de se passar da Web para dispositivos móveis, para o PC ou para outros dispositivos.

### <a name="build-rich-cross-device-experiences-by-using-the-device-relay-api"></a>Criar experiências avançadas em vários dispositivos usando a API de retransmissão de dispositivo

Além dos dispositivos da Microsoft (PCs, Windows Phone, Xbox, IoT, HoloLens e muito mais), a API de retransmissão de dispositivo também abrange dispositivos Android e iOS. Isso possibilita que você reduza os limites entre os dispositivos dos usuários. Você pode criar aplicativos que utilizam o ambiente do usuário e criar experiências avançadas que vão além de um único dispositivo em tempo real.

## <a name="api-reference"></a>Referência da API

Procurando a referência de API para estes serviços?

- [API para experiências entre dispositivos no Microsoft Graph versão 1.0](/graph/api/resources/project-rome-overview?view=graph-rest-1.0&preserve-view=true)
- [API para experiências entre dispositivos no Microsoft Graph beta](/graph/api/resources/project-rome-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Próximas etapas

- [Saiba mais sobre a API do feed de atividades no Microsoft Graph](activity-feed-concept-overview.md)
- [Saiba mais sobre a API de retransmissão de dispositivo no Microsoft Graph](device-relay-concept-overview.md)
