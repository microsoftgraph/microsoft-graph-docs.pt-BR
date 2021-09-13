---
title: Implantações no serviço de implantação Windows Atualização para Empresas
description: As implantações são a base do serviço de implantação Windows Update for Business. Por meio de uma implantação, você pode direcionar um conjunto de dispositivos para receber conteúdo específico do Windows Update, como uma atualização de software.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 550879fed2ea694f4c7c8c9dd5470c2eeace446b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117575"
---
# <a name="deployments-in-the-windows-update-for-business-deployment-service"></a>Implantações no serviço de implantação Windows Atualização para Empresas

As implantações são a base do serviço de implantação Windows Update for Business. Por meio de uma implantação, você pode direcionar um conjunto de dispositivos para receber conteúdo específico do Windows Update, como uma [atualização de software.](windowsupdates-software-updates.md)

As implantações têm os seguintes aspectos principais:

1. Conteúdo: a atualização disponível para implantação do catálogo. Isso é representado pela propriedade **de conteúdo** do [tipo deployableContent.](/graph/api/resources/windowsupdates-deployablecontent)
2. Público-alvo: os dispositivos para receber conteúdo. Esta é uma **relação de** audiência do [tipo deploymentAudience.](/graph/api/resources/windowsupdates-deploymentaudience)
3. Configurações: as configurações que regem como e quando o conteúdo deve ser entregue aos dispositivos. Isso é representado pela propriedade **settings** do tipo [deploymentSettings.](/graph/api/resources/windowsupdates-deploymentsettings)
4. Estado: o estado atual da implantação em seu ciclo de vida. Isso é representado pela propriedade **state** do [tipo deploymentState.](/graph/api/resources/windowsupdates-deploymentstate)

## <a name="create-a-deployment-with-content-and-an-audience"></a>Criar uma implantação com conteúdo e uma audiência


Como conteúdo e audiência são fundamentais para a definição de uma implantação, você deve atribuir ambos no momento da criação. Embora as atribuições de conteúdo e audiência não possam ser alteradas posteriormente, a associação de dispositivos em uma audiência pode.

Para saber mais sobre como criar uma implantação, consulte [Deploy a feature update and](windowsupdates-deploy-update.md) Deploy an [expedited security update](windowsupdates-deploy-expedited-update.md).

## <a name="configure-settings"></a>Definir configurações

### <a name="rollout"></a>Lançamento

[As configurações de distribuição](/graph/api/resources/windowsupdates-rolloutsettings) governam como o conteúdo é implantado ao longo do tempo para dispositivos na audiência de implantação. Você pode definir configurações de distribuição para implantações de atualizações de recursos.

Para saber mais sobre as configurações de distribuição, consulte [Agendar uma implantação](windowsupdates-schedule-deployment.md).

### <a name="monitoring"></a>Monitoramento

Você pode usar [as configurações de](/graph/api/resources/windowsupdates-monitoringsettings) monitoramento para configurar alertas e ações automatizadas a ser realizadas com base em sinais de atualização de dispositivos. As configurações de monitoramento podem ser configuradas para implantações de atualizações de recursos.


Para saber mais sobre as configurações de monitoramento, consulte [Gerenciar regras de monitoramento.](windowsupdates-manage-monitoring-rules.md)

### <a name="user-experience"></a>Experiência do usuário

Para implantações de atualizações de qualidade aceleradas, as configurações de experiência do usuário substituem temporariamente as políticas [existentes](/graph/api/resources/windowsupdates-userexperiencesettings) no dispositivo para a experiência de atualização.

Para saber mais sobre as configurações de experiência do usuário, [consulte Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).

## <a name="get-or-set-lifecycle-state"></a>Obter ou definir o estado do ciclo de vida

### <a name="states"></a>Estados

As implantações se movem pelos estados de ciclo de vida, conforme descrito na tabela a seguir.

| Estado     | Descrição                                                                                       |
|-----------|---------------------------------------------------------------------------------------------------|
| `scheduled` | A implantação aguarda condições de oferta a serem atendidas para começar a oferecer a atualização para dispositivos. |
| `offering`  | A implantação está oferecendo a atualização para dispositivos.                                                 |
| `paused`    | A implantação é pausada e impedida de oferecer a atualização para dispositivos até que ela não seja implantada.  |


### <a name="transitions"></a>Transitions

| Transition                     | Condition                                |
|--------------------------------|------------------------------------------|
| `scheduled` → `offering`           | A condição de agendamento é atendida.             |
| `offering` → `scheduled`           | A condição de agendamento não é atendida.         |
| `scheduled` ou `offering` → `paused` | Há uma solicitação ou uma ação automática para pausar. |
| `paused` → `scheduled` ou `offering` | Não há mais uma solicitação ou ação automática para pausar. |

### <a name="resource-model"></a>Modelo de recurso

O [recurso de](/graph/api/resources/windowsupdates-deployment) implantação tem uma propriedade de **estado** do tipo [deploymentState](/graph/api/resources/windowsupdates-deploymentstate) que fornece informações sobre o estado atual do ciclo de vida.

O serviço determina  o valor efetivo do estado de implantação como resultado líquido de várias entradas e processos assíncronos, mas você pode solicitar um valor específico definindo **requestedValue** como uma dessas entradas. Outras entradas para o valor de estado de implantação efetivo incluem configurações de distribuição e configurações de monitoramento.

## <a name="multiple-deployments"></a>Várias implantações

Você pode atribuir um dispositivo a várias implantações ao mesmo tempo. Essas implantações podem ser para conteúdo da mesma categoria de atualização (por exemplo, todas as implantações são atualizações de recursos) ou para conteúdo de categorias de atualização diferentes.

Quando você atribui um dispositivo a duas implantações para conteúdo de categorias de atualização diferentes (por exemplo, uma atualização de recursos e uma atualização de qualidade acelerada), o serviço de implantação oferece conteúdo em uma sequência de acordo com a recomendação da Microsoft.

Quando você atribui um dispositivo a duas implantações para conteúdo da mesma categoria de atualização (por exemplo, versões de atualização de recursos 20H1 e 20H2 ou atualizações de qualidade de março de 2021 e abril de 2021), o serviço de implantação oferece o conteúdo que está mais classificado pela Microsoft. Para atualizações de recursos e atualizações de qualidade, as atualizações mais recentes são classificadas mais alto. Esse comportamento não se aplica se uma das implantações ainda estiver agendada para o dispositivo e não estiver pronto para oferecer conteúdo. Nesse caso, a outra implantação fornece conteúdo para o dispositivo.
