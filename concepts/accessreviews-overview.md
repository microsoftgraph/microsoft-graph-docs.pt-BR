---
title: Visão geral da API de críticas de acesso
description: A API de críticas de acesso permite que você revise programaticamente o acesso aos recursos do Azure AD.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 128732f237a6a639152d9739e05b1cdbe389f00a
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651404"
---
# <a name="overview-of-the-access-reviews-api"></a>Visão geral da API de análises de acesso

A [API de revisões](/graph/api/resources/accessreviewsv2-overview) de acesso no Microsoft Graph permite que você revise programaticamente o acesso aos recursos do Azure AD. Essa revisão ajuda a garantir que as pessoas certas tenham o acesso certo aos recursos certos na organização.

Usando a API de críticas de acesso, você pode fazer as seguintes ações:
+ Crie, leia, atualize e exclua avaliações de acesso, configurações de revisão de acesso e agendamentos.
+ Investigue as avaliações de acesso passado e as decisões tomadas pelos revisadores, incluindo as etapas que o Azure AD tomou automaticamente.

## <a name="scope-of-use"></a>Escopo de uso

As APIs de críticas de acesso suportam contextos delegados e de aplicativos. Em um contexto de usuário (delegado), um aplicativo chama a API de críticas de acesso em nome de um usuário. Cenários típicos incluem:
+ Um administrador usando um script para criar, ler ou atualizar uma revisão de acesso.
+ Um proprietário de recursos usando um aplicativo ou um script para criar uma revisão de acesso para um recurso que ele possui.
+ Um administrador coleta automaticamente todas as decisões para uma ou mais avaliações de acesso.
  
Para autorizar seu aplicativo em um contexto de usuário (delegado), consulte [obter acesso em nome de um usuário](/graph/auth-v2-user).

Em um contexto de aplicativo, um aplicativo chama a API de críticas de acesso sem um usuário interno presente. Um cenário típico é um script de plano de fundo agendado coletando decisões regularmente para todas as avaliações de acesso. Para autorizar seu aplicativo nesse contexto, consulte [obter acesso sem um usuário](/graph/auth-v2-service).

## <a name="building-blocks-of-an-access-review"></a>Blocos de construção de uma revisão de acesso

As avaliações do Access são estruturadas logicamente e são compostas por esses blocos de construção:
+ **Definições de agendamento de revisões do Access** - O plano lógico que contém as configurações de uma revisão de acesso e suas instâncias. As configurações incluem os recursos contra os quais o acesso é revisado e os revisadores que atestam o acesso a esses recursos.
+ **Instância de revisão do Access** - Representa uma única atividade de revisão em relação à qual os revisadores tomarão decisões. Uma definição de revisão de acesso pode ter várias instâncias, como acontece em revisões recorrentes. As avaliações exclusivas têm exatamente uma instância.
+ **Itens de decisão registrados para uma** revisão - Representa uma decisão tomada por um revistor em uma instância, incluindo o carimbo de data/hora e a justificativa para a decisão. Cada instância de revisão tem tantas decisões quanto o número de usuários sob revisão. Se não houver decisões tomadas, ou seja, os revisadores não responderam à revisão, não haverá objetos de decisão para a instância.

## <a name="next-steps"></a>Próximas etapas

Experimente os seguintes tutoriais para gerenciar análises de acesso:

+ [Tutorial: use a API de críticas de acesso para revisar o acesso aos seus grupos de segurança](tutorial-accessreviews-securitygroup.md)
+ [Tutorial: use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes](tutorial-accessreviews-M365group.md)
