---
title: Visão geral da API de críticas de acesso
description: A API de críticas de acesso permite que você revise programaticamente o acesso aos recursos do Azure AD. Isso ajuda a garantir que as identidades certas tenham o acesso certo aos recursos corretos na organização.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: e09914b7e52f3be2961d3a55dd308262442eb1b1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335896"
---
# <a name="overview-of-the-access-reviews-api"></a>Visão geral da API de análises de acesso

[Azure Active Directory (Azure AD) access reviews](/azure/active-directory/governance/access-reviews-overview) is a feature of Azure AD Identity Governance that helps to ensure that the right identities (or principals) have the right access to the right resources in the organization. Essa revisão pode ser implementada programaticamente usando a [API de críticas de acesso](/graph/api/resources/accessreviewsv2-overview) no Microsoft Graph.

## <a name="participants-in-an-access-review"></a>Participantes em uma revisão de acesso

As avaliações do Access são sobre como atestar ou recertificar o acesso contínuo de uma entidade a um recurso. As entidades podem ser usuários, grupos ou aplicativos individuais.  

Os recursos para os quais o acesso pode ser revisado incluem grupos, funções privilegiadas (incluindo funções do Azure AD e funções de recurso do Azure), pacotes de acesso e aplicativos.

Os revisadores, ou os atestados, na revisão de acesso podem incluir os seguintes usuários ou grupos de usuários:

+ Um usuário (usuário convidado ou membro) revisando seu próprio acesso e atestando sua necessidade de acesso contínuo.
+ Outro usuário, por exemplo, um administrador em uma função de Administrador de Segurança, revisando o acesso para outras entidades.
+ O gerente de um usuário atestando a necessidade de acesso contínuo aos relatórios diretos.
+ Membros de um grupo.
+ Proprietários do grupo, incluindo proprietários que podem atender a critérios específicos.
+ Proprietários de aplicativos.

## <a name="building-blocks-of-the-access-review-api"></a>Blocos de construção da API de revisão de acesso

A API de análises de acesso é estruturada logicamente e é composta pelos seguintes blocos de construção.  

### <a name="1-access-reviews-schedule-definition"></a>1. Definição de agendamento de revisões do Access

Este é o plano lógico que contém as configurações de uma revisão de acesso e suas instâncias. Essas configurações incluem:

+ Os recursos que estão sendo acessados.
+ As entidades que acessam o recurso.
+ Os revisadores que atestam a necessidade das entidades de entidades manterem o acesso aos recursos.
+ A frequência da revisão de acesso.
+ Os estágios da revisão de acesso (para uma revisão de acesso em vários estágios).
+ Decisões padrão a aplicar se as decisões não são gravadas.

### <a name="2-access-review-instance"></a>2. Instância de revisão do Access

Representa uma única atividade de revisão, ou ocorrência, em relação à qual os revisadores tomarão decisões. Uma definição de revisão de acesso pode ter várias instâncias, como acontece em revisões recorrentes. As avaliações exclusivas têm exatamente uma instância. Para uma revisão de acesso em vários estágios, cada instância contém até três estágios.

### <a name="3-decision-item-recorded-for-a-review"></a>3. Item de decisão gravado para uma revisão

Representa uma decisão tomada por um revistor em uma instância, incluindo o carimbo de data/hora e a justificativa da decisão. Cada instância de revisão tem tantas decisões quanto o número de entidades em revisão. Se não houver decisões tomadas, ou seja, os revisadores não responderam à revisão, não haverá objetos de decisão para a instância.

As decisões recomendadas geradas pelo sistema podem ser fornecidas para cada item de decisão. Eles se baseiam na última data de entrada da entidade cujo acesso está sob revisão. Esse recurso dá aos revisadores visibilidade de contas inativas na organização e recomenda que as decisões se apliquem sobre o acesso contínuo da entidade.

As análises do Access também suportam a auditoria das decisões tomadas em cada instância de revisão de acesso, com as decisões também baixáveis para auditoria offline.

## <a name="scope-of-calling-the-access-reviews-api"></a>Escopo de chamada da API de críticas de acesso

A API de críticas de acesso dá suporte a [contextos delegados](/graph/auth-v2-user) [e de](/graph/auth-v2-service) aplicativos.

Em um contexto delegado (usuário), um aplicativo chama a API de críticas de acesso em nome de um usuário. Cenários típicos incluem:

+ Um administrador usa um script para criar, ler ou atualizar uma revisão de acesso.
+ Um proprietário de recursos usa um aplicativo ou um script para criar uma revisão de acesso para um recurso que ele possui.
+ Um administrador coleta automaticamente todas as decisões para uma ou mais críticas de acesso.

Em um contexto de aplicativo, um aplicativo chama a API de críticas de acesso sem um usuário interno presente. Um cenário típico é um script de plano de fundo agendado coletando decisões regularmente para todas as avaliações de acesso.

## <a name="next-steps"></a>Próximas etapas 

+ [Usar a API de críticas de acesso](/graph/api/resources/accessreviewsv2-overview)
+ [Leia mais sobre as avaliações de acesso do Azure AD](/azure/active-directory/governance/access-reviews-overview)
+ Experimente os seguintes tutoriais para gerenciar análises de acesso:
    + [Usar a API de avaliações de acesso para revisar o acesso aos seus grupos de segurança](tutorial-accessreviews-securitygroup.md)
    + [Use a API de críticas de acesso para revisar o acesso de convidados aos grupos Microsoft 365 seus clientes](tutorial-accessreviews-M365group.md)