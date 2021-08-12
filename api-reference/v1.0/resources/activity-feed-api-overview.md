---
title: Usar a API REST do feed de atividades
description: 'Você pode usar a API de feed de atividade no Microsoft Graph para retomar a atividade de um usuário em dispositivos e plataformas. As solicitações de API de feed de atividade são executadas em nome de um usuário por meio de permissões delegadas e da permissão de atividade do usuário, que podem ser usadas com contas pessoais ou de trabalho e de estudante. '
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: conceptualPageType
ms.openlocfilehash: 82724552fffb7b9d9832fa5d131dde145eeed22e76cbb4afde2d25e08399ea7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178623"
---
# <a name="use-the-activity-feed-rest-api"></a>Usar a API REST do feed de atividades

Namespace: microsoft.graph

Você pode usar a API de feed de atividade no Microsoft Graph para retomar a atividade de um usuário em dispositivos e plataformas. As solicitações de API de feed de atividade são [executadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) em nome de um usuário por meio de permissões delegadas e a permissão de atividade do usuário [,](/graph/permissions-reference)que pode ser usada com contas pessoais ou de trabalho e de estudante.

As atividades do usuário são representadas pelo recurso [de](/graph/api/resources/projectrome-activity) atividade e são organizadas em um feed baseado em tempo representado pela coleção me/activities.
<!-- Add missing content.
Each activity represents a unique...
-->
## <a name="what-makes-a-great-user-activity"></a>O que torna uma ótima atividade do usuário?

As atividades do usuário não iniciam apenas aplicativos — eles são links profundos para conteúdo específico em seu aplicativo. As atividades do usuário que você cria podem não apenas ser usadas em seu próprio aplicativo, mas também aparecerão no Cortana e na linha do tempo do Windows — impulsionando mais a reengenharia de aplicativos e facilitando que os usuários continuem usando seu aplicativo em vários dispositivos.

### <a name="what-should-become-an-activity"></a>O que deve se tornar uma atividade?

Como cada aplicativo é diferente, é responsabilidade de cada desenvolvedor de aplicativo entender a melhor maneira de mapear ações no seu aplicativo para atividades do usuário. Por exemplo, os jogos podem criar uma atividade para cada campanha, os aplicativos de criação de documentos podem criar uma atividade para cada documento exclusivo e aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho.

Aplique as seguintes diretrizes à medida que você define atividades em seu aplicativo:

**DO:** Grave uma única atividade para um grupo de ações de usuário relacionadas.
Se seu aplicativo for usado para uma sequência de conteúdo relacionado, provavelmente faz sentido gravar uma única atividade para toda a sessão de envolvimento.

*Cenários de playlist:* Isso é especialmente relevante para playlists de música ou programas de TV — uma única atividade do usuário pode ser atualizada para mostrar seu progresso. Nesse caso, você terá uma única [](/graph/api/resources/projectrome-historyitem) atividade de usuário com vários itens de histórico que representam períodos de envolvimento em vários dias ou semanas.

**DO:** Armazene dados do usuário na nuvem.
Se você deseja dar suporte a atividades entre dispositivos, é necessário garantir que o conteúdo necessário para reengenhar essa atividade seja armazenado em um local de nuvem. Por exemplo, se você publicar uma atividade sempre que um usuário editar um documento, o documento deverá ser armazenado na nuvem em vez de localmente no dispositivo do usuário para habilitar o reengenhar entre dispositivos.

**NÃO FAÇA ISSO:** Crie uma atividade do usuário para ações que os usuários não precisam retomar no futuro.
Se seu aplicativo for usado para concluir operações simples e única que não persistem no status para você rastrear no futuro, você provavelmente não precisará gravar uma atividade do usuário.

Para ficar claro, mesmo que as atividades do usuário apareçam na linha do tempo Windows, isso não foi projetado como uma ferramenta de versão — escolher uma atividade baseada em documento sempre deve mostrar a versão mais recente desse documento (incluindo alterações feitas por outro usuário).)

**NÃO FAÇA ISSO:** Crie uma atividade de usuário para ações concluídas por *outros usuários.*
Se alguém enviar uma mensagem ao usuário ou @mentions o usuário em seu aplicativo, você não deverá gravar uma nova atividade. Essas interações são melhor atendidas por notificações de surfacing.

*Cenários de colaboração:* Se várias pessoas estão trabalhando na mesma atividade (como um documento do Word), haverá casos em que outro usuário fez alterações no documento após a última edição. Nesse caso, os desenvolvedores de aplicativos podem querer atualizar os elementos visuais na atividade para refletir as alterações feitas no documento. Para fazer isso, o aplicativo pode atualizar a atividade existente sem criar um novo item de histórico.

>**Observação:** Se você estiver publicando atividades para um aplicativo Web, é importante incluir um e um `activationURL` para cada uma de suas `fallbackURL` atividades. As atividades iniciarão o usuário de volta ao seu aplicativo conforme esperado das experiências da Microsoft, como Windows Linha do Tempo.

## <a name="app-interaction-patterns-and-user-activities"></a>Padrões de interação do aplicativo e atividades do usuário
As atividades do usuário que você criar variarão com base no padrão de interação do aplicativo. Embora cada aplicativo seja diferente, a maioria se enquadra em um dos seguintes padrões de interação:

* **Aplicativos baseados** em documentos — Crie uma atividade por documento com um ou mais registros de histórico refletindo períodos de uso. É importante atualizar seu cartão de atividade à medida que as alterações são feitas no documento.
* **Aplicativos de reprodução de** mídia — Crie uma atividade por grupo lógico de conteúdo, como uma playlist, um programa ou um conteúdo autônomo.
* **Jogos** — crie uma atividade para cada jogo ou mundo salvo. Se o jogo oferece suporte apenas a uma única sequência de níveis, você pode gravar a mesma atividade ao longo do tempo, embora você queira atualizar seu cartão para mostrar seus progressos ou conquistas mais recentes.
* **Aplicativos utilitários** — se não houver nada em seu aplicativo que os usuários gostaria de retomar, você não deve publicar atividades. Um bom exemplo é um aplicativo simples de finalidade única, como calculadora.
* **Aplicativos de linha de negócios** — Muitos aplicativos existem para gerenciar tarefas simples ou fluxos de trabalho. Crie uma atividade para cada fluxo de trabalho separado acessado por meio do aplicativo. Por exemplo, cada relatório de despesas seria uma atividade separada, pois talvez você queira clicar nessa atividade para ver se ele foi aprovado.

*Alguns aplicativos complexos incluem vários padrões de interação. Talvez você queira seguir diferentes padrões de criação de atividades do usuário para diferentes cenários manipulados pelo aplicativo.*

<!-- Add content or remove H2.
## Common use cases
-->

## <a name="next-steps"></a>Próximas etapas

- Consulte o [recurso de atividade](/graph/api/resources/projectrome-activity) e defina as atividades do aplicativo para ajudar os usuários a retomar tarefas importantes.
- Explore os [exemplos de cartões adaptáveis](https://adaptivecards.io/samples/) para ideias para tornar suas atividades **pop**.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

**Procurando mais ideias?**

- Veja [como as experiências da Microsoft estão usando atividades](https://channel9.msdn.com/events/Build/2017/B8108).
- Saiba mais [sobre a API de feed de atividade e escolha de onde eu deixei](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011).
