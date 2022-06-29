---
title: Visão geral da API de análises de acesso
description: Use a API de revisões de acesso para examinar programaticamente o acesso aos recursos Azure AD para garantir que as identidades certas tenham o acesso certo aos recursos corretos.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 929eaeaf259b3f6f8db163ba7cec1a99fad17e7b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437076"
---
# <a name="overview-of-the-access-reviews-api"></a>Visão geral da API de análises de acesso

As revisões de acesso do [Azure AD (Azure Active Directory)](/azure/active-directory/governance/access-reviews-overview) são um recurso do Azure AD Identity Governance que ajuda a garantir que as identidades corretas (ou entidades de segurança) tenham o acesso certo aos recursos certos na organização. Essa revisão pode ser implementada programaticamente usando a [API de revisões de acesso](/graph/api/resources/accessreviewsv2-overview) no Microsoft Graph.

## <a name="participants-in-an-access-review"></a>Participantes em uma revisão de acesso

As revisões de acesso são sobre como atestar ou recertificar o acesso contínuo de uma entidade de segurança a um recurso. As entidades de segurança podem ser usuários, grupos ou aplicativos individuais.  

Os recursos para os quais o acesso pode ser revisado incluem grupos, funções privilegiadas (incluindo funções Azure AD funções de recurso do Azure), pacotes de acesso e aplicativos.

Os revisores, ou os atestados, na revisão de acesso podem incluir os seguintes usuários ou grupos de usuários:

+ Um usuário (usuário convidado ou um membro) examinando seu próprio acesso e atestando sua necessidade de acesso contínuo.
+ Outro usuário, por exemplo, um administrador em uma função de Administrador de Segurança, examinando o acesso de outras entidades de segurança.
+ O gerente de um usuário que atesta a necessidade de acesso contínuo a seus relatórios diretos.
+ Membros de um grupo.
+ Proprietários de grupo, incluindo proprietários que podem atender a critérios específicos.
+ Proprietários de aplicativos.

## <a name="building-blocks-of-the-access-review-api"></a>Blocos de construção da API de revisão de acesso

A API de revisões de acesso é estruturada logicamente e é composta pelos seguintes blocos de construção.  

### <a name="1-access-reviews-schedule-definition"></a>1. Definição da agenda de revisões de acesso

Esse é o blueprint lógico que contém as configurações de uma revisão de acesso e suas instâncias. Essas configurações incluem:

+ Os recursos que estão sendo acessados.
+ As entidades de segurança que acessam o recurso.
+ Os revisores que atestam a necessidade das entidades de segurança manterem o acesso aos recursos.
+ A frequência da revisão de acesso.
+ Os estágios da revisão de acesso (para uma revisão de acesso de vários estágios).
+ Decisões padrão a serem aplicadas se as decisões não forem registradas.

### <a name="2-access-review-instance"></a>2. Instância de revisão de acesso

Representa uma única atividade de revisão, ou ocorrência, em relação à qual os revisores toma decisões. Uma definição de revisão de acesso pode ter várias instâncias, como é o caso em revisões recorrentes. As revisões one-off têm exatamente uma instância. Para uma revisão de acesso de vários estágios, cada instância contém até três estágios.

### <a name="3-decision-item-recorded-for-a-review"></a>3. Item de decisão registrado para revisão

Representa uma decisão que um revisador tomou em uma instância, incluindo o carimbo de data/hora e a justificativa para a decisão. Cada instância de revisão tem tantas decisões quanto o número de entidades de segurança em revisão. Se não houver decisões tomadas, ou seja, os revisores não responderam à revisão, não haverá objetos de decisão para a instância.

Decisões recomendadas geradas pelo sistema podem ser fornecidas para cada item de decisão. Eles se baseiam na data de último logon da entidade de segurança cujo acesso está sob revisão. Esse recurso dá aos revisores visibilidade de contas inativas na organização e recomenda que as decisões se apliquem sobre o acesso contínuo da entidade de segurança.

As revisões de acesso também dão suporte à auditoria das decisões que foram tomadas em cada instância de revisão de acesso, com as decisões também baixáveis para auditoria offline.

## <a name="scope-of-calling-the-access-reviews-api"></a>Escopo da chamada à API de revisões de acesso

A API de revisões de acesso dá suporte [a contextos delegados](/graph/auth-v2-user) [e de](/graph/auth-v2-service) aplicativo.

Em um contexto delegado (usuário), um aplicativo chama a API de revisões de acesso em nome de um usuário. Cenários típicos incluem:

+ Um administrador usa um script para criar, ler ou atualizar uma revisão de acesso.
+ Um proprietário de recurso usa um aplicativo ou um script para criar uma revisão de acesso para um recurso que ele possui.
+ Um administrador coleta automaticamente todas as decisões para uma ou mais revisões de acesso.

Em um contexto de aplicativo, um aplicativo chama a API de revisões de acesso sem um usuário conectado presente. Um cenário típico é um script em segundo plano agendado que coleta regularmente decisões para todas as revisões de acesso.

## <a name="next-steps"></a>Próximas etapas 

+ [Usar a API de revisões de acesso](/graph/api/resources/accessreviewsv2-overview)
+ [Leia mais sobre Azure AD revisões de acesso](/azure/active-directory/governance/access-reviews-overview)
+ Experimente os seguintes tutoriais para gerenciar revisões de acesso:
    + [Usar a API de revisões de acesso para examinar o acesso aos seus grupos de segurança](tutorial-accessreviews-securitygroup.md)
    + [Usar a API de revisões de acesso para examinar o acesso de convidados aos seus grupos do Microsoft 365](tutorial-accessreviews-M365group.md)