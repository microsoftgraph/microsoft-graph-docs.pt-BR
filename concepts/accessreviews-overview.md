---
title: Visão geral da API de críticas de acesso
description: A API de críticas de acesso permite que você revise programaticamente o acesso aos recursos do Azure AD.
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: 92ea2d49fae37c5b4d5ae82e390f897af9ff4cde
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067058"
---
# <a name="overview-of-the-access-reviews-api"></a>Visão geral da API de análises de acesso

A [API de revisões](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) de acesso no Microsoft Graph permite que você revise programaticamente o acesso aos recursos do Azure AD. Isso inclui:
+ Criando, lendo, atualizando e excluindo avaliações de acesso, configurações de revisão de acesso e agendamentos.
+ Investigando as análises de acesso anteriores e as decisões tomadas pelos revisadores, incluindo as etapas que o Azure AD tomou automaticamente.

## <a name="scope-of-use"></a>Escopo de uso

As APIs de críticas de acesso suportam contextos delegados e de aplicativos. Em um contexto de usuário (delegado), um aplicativo chama a API de críticas de acesso em nome de um usuário. Cenários típicos incluem:
+ Um administrador usando um script para criar, ler ou atualizar uma revisão de acesso.
+ Um proprietário de recursos usando um aplicativo ou um script para criar uma revisão de acesso para um recurso que ele possui.
+ Um administrador coleta automaticamente todas as decisões para uma ou mais avaliações de acesso.
  
Para autorizar seu aplicativo em um contexto de usuário (delegado), consulte [obter acesso em nome de um usuário](/graph/auth-v2-user).

Em um contexto de aplicativo, um aplicativo chama a API de críticas de acesso sem um usuário interno presente. Um cenário típico é um script de plano de fundo agendado coletando decisões regularmente para todas as avaliações de acesso. Para autorizar seu aplicativo nesse contexto, consulte [obter acesso sem um usuário](/graph/auth-v2-service).

## <a name="building-blocks-of-an-access-review"></a>Blocos de construção de uma revisão de acesso

As avaliações do Access são estruturadas logicamente e são compostas por esses blocos de construção:
+ **Definições de agendamento de revisões do Access** - O plano lógico que contém as configurações de uma revisão de acesso e suas instâncias.
+ **Instância de revisão do Access** - Representa uma atividade de revisão que tem um escopo, revisadores e um status. Uma definição de revisão de acesso pode ter várias instâncias, como acontece em revisões recorrentes. As avaliações exclusivas têm exatamente uma instância.
+ **Itens de decisão registrados para uma** revisão - Representam uma decisão tomada por um revistor em uma instância, incluindo o carimbo de data/hora e a justificativa para a decisão. Cada instância de revisão tem tantas decisões quanto o número de usuários sob revisão. Se não houver decisões tomadas, ou seja, os revisadores não responderam à revisão, não haverá objetos de decisão para a instância.

## <a name="next-steps"></a>Próximas etapas

Experimente os seguintes tutoriais para gerenciar análises de acesso:

+ [Usar a API de avaliações de acesso para grupos para revisar o acesso aos seus grupos de segurança](tutorial-accessreviews-securitygroup.md)
+ [Usar a API de críticas de acesso para grupos para revisar o acesso a todos os grupos Microsoft 365 com usuários convidados](tutorial-accessreviews-M365group.md)

## <a name="see-also"></a>Confira também

+ [Planejamento Azure Active Directory implantação de Avaliações do Access](/azure/active-directory/governance/deploy-access-reviews)
+ [Criar uma revisão de acesso de grupos & aplicativos](/azure/active-directory/governance/create-access-review)
+ [Obter acesso em nome de um usuário](/graph/auth-v2-user)
+ [Obter acesso sem um usuário](/graph/auth-v2-service)
