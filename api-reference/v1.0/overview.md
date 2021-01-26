---
title: Referência da API REST do Microsoft Graph v1.0
description: Bem-vindo à referência da API REST do Microsoft Graph para o ponto de extremidade v1.0.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: non-product-specific
doc_type: conceptualPageType
ms.openlocfilehash: 56bc6b580fe691810600feee468c94cdd8a4d852
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980812"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a>Referência da API REST do Microsoft Graph v1.0

Bem-vindo à referência da API REST do Microsoft Graph para o ponto de extremidade v1.0.

Os conjuntos de APIs no ponto de extremidade v1.0 (`https://graph.microsoft.com/v1.0`) estão no status de disponibilidade geral (GA) e passaram por um processo rigoroso de revisão e comentários com os clientes para atender às necessidades práticas de produção. Atualizações para APIs neste ponto de extremidade são de natureza aditiva e não quebram os cenários de aplicativos existentes.

## <a name="common-use-cases"></a>Casos comuns de uso

O poder do Microsoft Graph reside na fácil navegação de entidades e relacionamentos entre diferentes serviços expostos em um único ponto de extremidade REST do Microsoft Graph.

Vários desses serviços são projetados para permitir cenários ricos em torno de um [usuário](./resources/user.md) e em torno de um [grupo](./resources/group.md).

### <a name="user-centric-use-cases-in-v10"></a>Casos de uso centrado no usuário na v1.0

1. [Obter o perfil](./api/user-get.md) e a [foto](./resources/profilephoto.md) de um usuário, Lisa.
2. [Obter as informações de perfil sobre o gerente de Lisa](./api/user-list-manager.md) e as [IDs de seus subordinados diretos](./api/user-list-directreports.md), todos armazenados no Azure Active Directory.
3. [Acessar os arquivos de Lisa no OneDrive for Business](./api/driveitem-list-children.md), localizar a [identidade](./resources/identityset.md) da última pessoa que modificou um [arquivo](./resources/driveitem.md) e navegar até o perfil dessa pessoa.
4. [Acessar o calendário de Lisa](./api/calendar-get.md) no Exchange Online e [determinar o melhor horário para Lisa se reunir com sua equipe](./api/user-findmeetingtimes.md) nas próximas duas semanas.
5. [Inscrever-se](./api/subscription-post-subscriptions.md) e [acompanhar as mudanças](./api/event-delta.md) no calendário de Lisa, dizer a Lisa quando ela estiver gastando mais de 80% de seu tempo em reuniões.
6. [Definir respostas automáticas](./api/user-update-mailboxsettings.md#example-1) quando Lisa estiver fora do escritório.
7. [Receber as pessoas mais relevantes para a Lisa](./api/user-list-people.md), com base nas relações de comunicação, colaboração e negócios.
8. Obter a última projeção de vendas de um [gráfico](./resources/chart.md) em um arquivo do Excel no OneDrive for Business de Lisa.
9. [Encontrar as tarefas atribuídas a Lisa no Planner](./api/planneruser-list-tasks.md).

### <a name="microsoft-365-group-use-cases-in-v10"></a>Casos de uso de um grupo do Microsoft 365 na v1.0

1. Emitir um relatório sobre grupos do Microsoft 365 em uma organização e identificar o grupo com mais [comunicação entre os membros do grupo](./api/reportroot-getoffice365groupsactivitycounts.md).
2. [Localizar os planos desse grupo do Microsoft 365](./api/plannergroup-list-plans.md) e a [atribuição de tarefas](./resources/plannerassignments.md) nesse plano.
3. [Iniciar uma nova conversa](./api/group-post-conversations.md) no grupo do Microsoft 365 para determinar se os membros desejam [criar](./api/group-post-groups.md) outro grupo para compartilhar a carga de trabalho.
4. [Obter o bloco de anotações padrão](./api/notebook-get.md) para o grupo e [criar uma página](./api/section-post-pages.md) para anotar o resultado da investigação.

## <a name="other-api-versions"></a>Outras versões da API

Existem atualmente 2 versões de APIs REST do Microsoft Graph - v1.0 e beta.
Se você estiver interessado em APIs novas ou aprimoradas que ainda estejam no status de visualização, consulte [referência de ponto de extremidade beta do Microsoft Graph](/graph/api/overview?view=graph-rest-beta&preserve-view=true). Esteja ciente de que as APIs no status de visualização estão sujeitas a alterações e podem interromper os cenários existentes sem aviso prévio. Não obtenha uma dependência de produção de APIs no ponto de extremidade beta.

Encontre mais informações em [Suporte e controle de versão](/graph/versioning-and-support).

## <a name="call-the-v10-endpoint"></a>Chame o ponto de extremidade do v 1.0

As solicitações da API do Microsoft Graph para o ponto de extremidade v1.0 usam o seguinte padrão:

```http
https://graph.microsoft.com/v1.0/{resource}?[query_parameters]
```

Para detalhes, consulte [Usando a API do Microsoft Graph](/graph/use-the-api).

## <a name="whats-new"></a>Novidades
Saiba mais sobre [os recursos e atualizações mais recentes](/graph/whats-new-overview) no ponto de extremidade v1.0.

## <a name="connect-with-us"></a>Fale conosco

Existem APIs adicionais ou recursos que você gostaria de ver no Microsoft Graph? Poste novas solicitações de recursos no [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).

Possui comentários para APIs existentes do Microsoft Graph? Conecte-se conosco em [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).
