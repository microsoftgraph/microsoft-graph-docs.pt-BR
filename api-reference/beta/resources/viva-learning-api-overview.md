---
title: Usar a API de aprendizado de funcionários para integrar-se ao Aprendizagem do Viva
description: Saiba como registrar um provedor e integrar seus registros de conteúdo e aprendiz do seu provedor de aprendizagem ao Aprendizagem do Viva.
ms.localizationpriority: medium
author: malabikaroy
ms.prod: employee-learning
doc_type: conceptualPageType
ms.openlocfilehash: f8112d21cc4d3677c4b36398539a529c247ecd39
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883247"
---
# <a name="use-the-employee-learning-api-to-integrate-with-viva-learning"></a>Usar a API de aprendizado de funcionários para integrar-se ao Aprendizagem do Viva

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aprendizagem do Viva é um hub centralizado de aprendizado de funcionários no Microsoft Teams que permite que os funcionários integrem o aprendizado e a criação de habilidades em seu dia de trabalho. Nesse Aprendizagem do Viva, as equipes podem descobrir, compartilhar, recomendar e aprender com bibliotecas de conteúdo fornecidas por sua organização e parceiros. Eles podem acessar rapidamente o conteúdo de aprendizado atribuído ou concluído recentemente e fazer tudo isso sem sair do Microsoft Teams.

A API de aprendizado de funcionários no Microsoft Graph permite que os aplicativos dispobilizem conteúdo de um LMS (Sistema de Gerenciamento de Aprendizagem) ou de um provedor de aprendizado no Aprendizagem do Viva. Use os seguintes recursos para integração com Aprendizagem do Viva:

- [Provedor de aprendizagem](learningprovider.md) para gerenciar provedores de aprendizado, incluindo registro, habilitação, desabilitação ou exclusão de provedores.
- [Conteúdo de aprendizagem](learningcontent.md) para carregar e gerenciar metadados de conteúdo de aprendizado de seu LMS ou provedor de aprendizado em Aprendizagem do Viva.


## <a name="how-do-integrations-work"></a>Como funcionam as integrações?
Como administradores, você pode integrar seu conteúdo e seus registros de aprendiz (atribuições de funcionários e registros de curso concluídos) do LMS ou provedor de aprendizagem com o Aprendizagem do Viva, usando integrações integradas em que o Aprendizagem do Viva pode efetuar pull de metadados de conteúdo e registros de aprendizado do lmS ou do provedor de aprendizagem. Você também pode [usar a API de aprendizado](#use-cases-for-the-employee-learning-api-in-microsoft-graph) de funcionários no Microsoft Graph para enviar por push metadados de conteúdo de seu LMS ou provedor de aprendizado para Aprendizagem do Viva. 

Quando os metadados de conteúdo, as atribuições de funcionários e seus registros de curso concluídos são carregados no Aprendizagem do Viva, eles aparecem em Aprendizagem do Viva nos seguintes locais:
- O conteúdo aparece na home page na **seção Procurar cursos** –  Provedores.
- As tarefas e os registros de curso concluídos aparecem na página **Meu Aprendizado** nas seções Atribuídas  a **Você** e Concluídas, respectivamente.

## <a name="authorization"></a>Autorização
Com as permissões de aprendizado de funcionários delegadas ou de aplicativo [apropriadas](/graph/permissions-reference#employee-learning-permissions), seu aplicativo pode usar a API de aprendizado de funcionários para gerenciar provedores de aprendizado e seu conteúdo para um hub de aprendizado em um locatário. Para obter mais informações sobre tokens de acesso, registro de aplicativo e permissões delegadas e de aplicativo, consulte [noções básicas de autenticação e autorização](/graph/auth/auth-concepts).

## <a name="use-cases-for-the-employee-learning-api-in-microsoft-graph"></a>Casos de uso para a API de aprendizado de funcionários no Microsoft Graph
Use as APIs de aprendizado de funcionário para fazer o seguinte:
- Registre um provedor com [Aprendizagem do Viva](../api/employeeexperience-post-learningproviders.md), forneça um nome de exibição, um logotipo quadrado exibido em um cartão de conteúdo de aprendizagem e um logotipo longo exibido na página Detalhes, que é  necessário para que o conteúdo do provedor seja exibido no Aprendizagem do Viva. A ID de registro retornada pode ser usada para fazer as chamadas subsequentes para ingestão de conteúdo.
- Habilite ou desabilite um registro e atualize o nome de exibição e as URLs do logotipo de um provedor.  
- [Obtenha os detalhes sobre um provedor no](../api/learningprovider-get.md) Aprendizagem do Viva para uma **registrationId específica**.  
- [Obtenha a lista de registros de provedor](../api/employeeexperience-list-learningproviders.md) no Aprendizagem do Viva para um locatário.
- [Exclua um](../api/employeeexperience-delete-learningproviders.md) registro de um provedor no Aprendizagem do Viva.
- [Envie por push os metadados](../api/learningcontent-update.md) Aprendizagem do Viva conteúdo para disponibilizar o Aprendizagem do Viva para consumo pelos usuários.  
- [Obtenha uma lista dos metadados do conteúdo ingerido](../api/learningprovider-list-learningcontents.md) de um provedor usando **a registrationId** de um provedor.  
- [Obtenha os metadados especificados do conteúdo ingerido](../api/learningcontent-get.md) de um provedor Aprendizagem do Viva.
- [Exclua os metadados especificados do conteúdo ingerido de um provedor](../api/learningprovider-delete-learningcontents.md).

>**Observação**: as atribuições e os registros de curso concluídos ainda não estão disponíveis na API de aprendizagem do funcionário.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas
- [Habilite o aprendizado dos funcionários usando os recursos colaborativos no Teams](/graph/teams-concept-overview#enable-employee-learning-using-the-collaborative-capabilities-in-teams).
- Experimente a API de aprendizado de funcionário no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
