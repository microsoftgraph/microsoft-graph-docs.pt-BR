---
title: Usar a API REST de feed de atividades
description: 'Você pode usar a API do feed de atividades no Microsoft Graph para retomar a atividade de um usuário entre dispositivos e plataformas. As solicitações da API de feed de atividades são realizadas em nome de um usuário via permissões delegadas e a permissão de atividade do usuário, que pode ser usada com contas pessoais ou corporativas e de estudante. '
localization_priority: Normal
ms.prod: project-rome
doc_type: conceptualPageType
author: ailae
ms.openlocfilehash: 4ed2b55c06710b17be984e2c9be71ba8496d5991
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523361"
---
# <a name="use-the-activity-feed-rest-api"></a>Usar a API REST de feed de atividades

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Você pode usar a API do feed de atividades no Microsoft Graph para retomar a atividade de um usuário entre dispositivos e plataformas. As solicitações da API de feed de atividades são realizadas em nome de um usuário via [permissões delegadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) e a [permissão de atividade do usuário](/graph/permissions-reference), que pode ser usada com contas pessoais ou corporativas e de estudante.

As atividades do usuário são representadas pelo recurso [atividade](/graph/api/resources/projectrome-activity) e são organizadas em um feed baseado em tempo representado pela coleção me/Activities.
<!-- Add missing content.
Each activity represents a unique...
-->
## <a name="what-makes-a-great-user-activity"></a>O que faz uma boa atividade do usuário?

As atividades do usuário não apenas iniciam aplicativos – elas são links profundos para conteúdo específico no seu aplicativo. As atividades do usuário que você cria não podem ser usadas somente em seu próprio aplicativo, mas também aparecerão na Cortana e na linha do tempo do Windows, levando mais reenvolvimento de aplicativos e facilitando o uso do aplicativo em vários dispositivos.

### <a name="what-should-become-an-activity"></a>O que deve se tornar uma atividade?

Como todos os aplicativos são diferentes, é para cada desenvolvedor de aplicativos entender a melhor maneira de mapear ações dentro de seu aplicativo para as atividades do usuário. Por exemplo, os jogos podem criar uma atividade para cada campanha, os aplicativos de criação de documentos podem criar uma atividade para cada documento exclusivo, e os aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho.

Aplique as seguintes diretrizes ao definir atividades em seu aplicativo:

**Fazer:** Registrar uma única atividade para um grupo de ações de usuário relacionadas.
Se o aplicativo for usado para uma sequência de conteúdo relacionado, provavelmente fará sentido registrar uma única atividade para toda a sessão de compromisso.

*Cenários de playlist:* Isso é especialmente relevante para playlists de música ou programas de TV — uma única atividade de usuário pode ser atualizada para mostrar seu progresso. Nesse caso, você terá uma única atividade de usuário com vários [itens de histórico](/graph/api/resources/projectrome-historyitem) representando períodos de contrato em vários dias ou semanas.

**Fazer:** Armazenar dados de usuário na nuvem.
Se você quiser dar suporte a atividades entre dispositivos, precisará certificar-se de que o conteúdo necessário para recontratar essa atividade está armazenado em um local de nuvem. Por exemplo, se você publicar uma atividade cada vez que um usuário edita um documento, o documento deve ser armazenado na nuvem, em vez de localmente no dispositivo do usuário para habilitar o reenvolvimento entre dispositivos.

Não **:** Criar uma atividade do usuário para ações que os usuários não precisam retomar no futuro.
Se seu aplicativo for usado para concluir operações simples e de um único tempo que não persistem status para que você acompanhe no futuro, provavelmente não precisará escrever uma atividade do usuário.

Para ser claro, mesmo que as atividades do usuário apareçam na linha do tempo do Windows, isso não é projetado como uma ferramenta de controle de versão, a escolha de uma atividade baseada em documento deve sempre mostrar a versão mais recente do documento (incluindo as alterações feitas por outro usuário.)

Não **:** Criar uma atividade de usuário para ações concluídas por *outros usuários*.
Se alguém enviar uma mensagem para o usuário ou @mentions o usuário no seu aplicativo, você não deve escrever uma nova atividade. Essas interações são mais bem servidas por notificações do revelar.

*Cenários de colaboração:* Se várias pessoas estiverem trabalhando na mesma atividade (como um documento do Word), haverá casos quando outro usuário tiver feito alterações no documento depois da última edição. Nesse caso, os desenvolvedores de aplicativos podem querer atualizar os elementos visuais na atividade para refletir as alterações feitas no documento. Para fazer isso, o aplicativo pode atualizar a atividade existente sem criar um novo item de histórico.

>**Observação:** Se você estiver publicando atividades para um aplicativo Web, é importante incluir um `activationURL` e um `fallbackURL` para cada uma de suas atividades. As atividades iniciarão o usuário de volta para o aplicativo conforme o esperado das experiências da Microsoft, como a linha do tempo do Windows.

## <a name="app-interaction-patterns-and-user-activities"></a>Padrões de interação de aplicativos e atividades do usuário
As atividades do usuário que você criar irão variar com base no padrão de interação do seu aplicativo. Embora cada aplicativo seja diferente, a maioria se enquadrará em um dos seguintes padrões de interação:

* **Aplicativos baseados em documentos** — crie uma atividade por documento com um ou mais registros de histórico que refletem os períodos de uso. É importante atualizar seu cartão de atividades à medida que as alterações são feitas no documento.
* **Aplicativos de reprodução de mídia** — crie uma atividade por agrupamento lógico de conteúdo como uma lista de reprodução, programa ou conteúdo autônomo.
* **Jogos** — crie uma atividade para cada jogo ou mundo salvo. Se seu jogo suportar apenas uma única sequência de níveis, você pode escrever a mesma atividade com o passar do tempo, embora você queira atualizar seu cartão para mostrar o andamento ou as realizações mais recentes.
* **Aplicativos Utilitários** — se não houver nada no aplicativo que os usuários desejam retomar, você não deve publicar atividades. Um bom exemplo é um aplicativo simples de uso único, como a calculadora.
* **Aplicativos de linha de negócios** — muitos aplicativos existem para gerenciar tarefas simples ou fluxos de trabalho. Crie uma atividade para cada fluxo de trabalho separado acessado por meio de seu aplicativo. Por exemplo, cada relatório de despesas seria uma atividade separada, porque talvez você queira clicar nessa atividade para ver se ela foi aprovada.

*Alguns aplicativos complexos incluem vários padrões de interação. Você pode querer seguir padrões diferentes de criação de atividades do usuário para diferentes cenários manipulados pelo seu aplicativo.*

<!-- Add content or remove H2.
## Common use cases
-->

## <a name="next-steps"></a>Próximas etapas

- Consulte o [recurso atividade](/graph/api/resources/projectrome-activity) e defina as atividades do seu aplicativo para ajudar os usuários a retomar tarefas importantes.
- Explore os exemplos de [cartões adaptáveis](https://adaptivecards.io/samples/) para ideias para tornar suas atividades **pop**.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

**Procurando mais ideias?**

- Veja [como as experiências da Microsoft estão usando atividades](https://channel9.msdn.com/events/Build/2017/B8108).
- Saiba mais sobre [a API de feed de atividades e escolha onde eu parou](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011).
