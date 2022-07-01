---
title: Implantações no serviço de implantação do Windows Update para Empresas
description: Use o serviço Windows Update implantação do Windows Update Business para criar implantações, definir configurações e definir o estado do ciclo de vida. Atribuir um dispositivo a várias implantações.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 38165c5f4da09e97102cb3a7f6bc9e26c9f60ff6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437510"
---
# <a name="deployments-in-the-windows-update-for-business-deployment-service"></a>Implantações no serviço de implantação do Windows Update para Empresas

As implantações são a base do serviço de implantação Windows Update para Empresas. Por meio de uma implantação, você pode direcionar um conjunto de dispositivos para receber conteúdo específico Windows Update, como uma atualização [de software](windowsupdates-software-updates.md).

As implantações têm os seguintes aspectos principais:

1. Conteúdo: a atualização disponível para implantação do catálogo. Isso é representado pela propriedade **de conteúdo** do [tipo deployableContent](/graph/api/resources/windowsupdates-deployablecontent) .
2. Público-alvo: os dispositivos para receber conteúdo. Essa é uma **relação de** público-alvo do [tipo deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) .
3. Configurações: as configurações que regem como e quando o conteúdo deve ser entregue aos dispositivos. Isso é representado pela propriedade **settings** do tipo [deploymentSettings](/graph/api/resources/windowsupdates-deploymentsettings) .
4. Estado: o estado atual da implantação em seu ciclo de vida. Isso é representado pela propriedade **de estado** do tipo [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) .

## <a name="create-a-deployment-with-content-and-an-audience"></a>Criar uma implantação com conteúdo e um público-alvo

Como o conteúdo e o público-alvo são chave para a definição de uma implantação, você precisa atribuir ambos no momento da criação. Embora as atribuições de conteúdo e audiência não possam ser alteradas posteriormente, a associação de dispositivo dentro de um público-alvo pode.

Para saber mais sobre como criar uma implantação, consulte [Implantar uma atualização de recurso](windowsupdates-deploy-update.md) e [implantar uma atualização de segurança acelerada](windowsupdates-deploy-expedited-update.md).

## <a name="configure-settings"></a>Definir configurações

### <a name="rollout"></a>Implantação

[As configurações de distribuição](/graph/api/resources/windowsupdates-rolloutsettings) regem como o conteúdo é implantado ao longo do tempo em dispositivos no público de implantação. Você pode definir configurações de distribuição para implantações de atualizações de recursos.

Para saber mais sobre as configurações de distribuição, consulte [Agendar uma implantação](windowsupdates-schedule-deployment.md).

### <a name="monitoring"></a>Monitoramento

Você pode usar [as configurações de monitoramento para](/graph/api/resources/windowsupdates-monitoringsettings) configurar alertas e ações automatizadas a serem tomadas com base em sinais de atualização dos dispositivos. As configurações de monitoramento podem ser definidas para implantações de atualizações de recursos.


Para saber mais sobre as configurações de monitoramento, consulte [Gerenciar regras de monitoramento](windowsupdates-manage-monitoring-rules.md).

### <a name="user-experience"></a>Experiência do usuário

Para implantações de atualizações de qualidade aceleradas, as configurações de experiência do usuário substituem temporariamente as políticas [existentes](/graph/api/resources/windowsupdates-userexperiencesettings) no dispositivo para a experiência de atualização.

Para saber mais sobre as configurações de experiência do usuário, [confira Implantar uma atualização de segurança acelerada](windowsupdates-deploy-expedited-update.md).

## <a name="get-or-set-lifecycle-state"></a>Obter ou definir o estado do ciclo de vida

### <a name="states"></a>Estados

As implantações são movidas pelos estados do ciclo de vida, conforme descrito na tabela a seguir.

| Estado       | Descrição                                                                                       |
|-------------|---------------------------------------------------------------------------------------------------|
| `scheduled` | A implantação está aguardando que as condições da oferta sejam atendidas para começar a oferecer a atualização aos dispositivos. |
| `offering`  | A implantação está oferecendo a atualização para dispositivos.                                                 |
| `paused`    | A implantação é pausada e impedida de oferecer a atualização aos dispositivos até que ela não seja pausada.  |
| `faulted`   | A implantação não está oferecendo a atualização para dispositivos devido a um motivo pelo qual o serviço não pode resolver.  |


### <a name="transitions"></a>Transitions

| Transition                           | Condição                                |
|--------------------------------------|------------------------------------------|
| `scheduled` → `offering`             | A condição de agendamento foi atendida.             |
| `offering` → `scheduled`             | A condição de agendamento não foi atendida.         |
| `scheduled`ou →`offering``paused` | Há uma solicitação ou uma ação automática para pausar. |
| `paused``scheduled`→ ou`offering` | Não há mais uma solicitação ou ação automática para pausar. |
| `offering`, `scheduled`ou `paused` → `faulted` | Há um erro que o serviço não pode resolver. |

### <a name="resource-model"></a>Modelo de recurso

O [recurso de](/graph/api/resources/windowsupdates-deployment) implantação tem uma **propriedade de** estado do tipo [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) que fornece informações sobre o estado atual do ciclo de vida.

O serviço determina o valor efetivo  do estado de implantação como resultado líquido de várias entradas e processos assíncronos, mas você pode solicitar um valor específico definindo **requestedValue** como uma dessas entradas. Outras entradas para o valor de estado de implantação efetivo incluem configurações de distribuição e configurações de monitoramento.

## <a name="assign-a-device-to-multiple-deployments"></a>Atribuir um dispositivo a várias implantações

Você pode atribuir um dispositivo a várias implantações ao mesmo tempo. Essas implantações podem ser para conteúdo da mesma categoria de atualização (por exemplo, todas as implantações são atualizações de recursos) ou para conteúdo de categorias de atualização diferentes.

Quando você atribui um dispositivo a duas implantações para conteúdo de categorias de atualização diferentes (por exemplo, uma atualização de recurso e uma atualização de qualidade acelerada), o serviço de implantação oferece conteúdo em uma sequência de acordo com a recomendação da Microsoft.

Quando você atribui um dispositivo a duas implantações para conteúdo da mesma categoria de atualização (por exemplo, versões de atualização de recursos 20H1 e 20H2 ou atualizações de qualidade de março de 2021 e abril de 2021), o serviço de implantação oferece o conteúdo que é mais classificado pela Microsoft. Para atualizações de recursos e atualizações de qualidade, as atualizações mais recentes são mais bem classificadas. Esse comportamento não se aplicará se uma das implantações ainda estiver agendada para o dispositivo e não estiver pronta para oferecer conteúdo. Nesse caso, a outra implantação fornece conteúdo para o dispositivo.
