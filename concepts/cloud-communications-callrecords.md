---
title: Visão geral dos registros de chamada
description: Os registros de chamadas dão informações sobre as chamadas e reuniões que ocorrem em sua organização.
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: eb471bedc5156e537015eeb8de0d68483eaff7ad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136184"
---
# <a name="call-records-overview"></a>Visão geral dos registros de chamada

Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business. Os dados de uso e diagnóstico podem ser consumidos para produzir relatórios personalizados para sua empresa para ajudar a monitorar a adoção ou a solucionar problemas de qualidade de chamada.

As organizações podem assinar alterações nos registros de chamadas usando o recurso de assinaturas de [webhook](/graph/api/resources/webhooks.md) do Microsoft Graph, permitindo que elas criem relatórios quase em tempo real a partir dos dados ou alertem em determinados cenários, como chamadas de emergência.

> **Importante:** Use a discrição ao conceder a permissão CallRecords.Read.All aos aplicativos. Os registros de chamada podem fornecer informações sobre a operação da sua empresa e, portanto, podem ser um alvo para atores mal-intencionados. Conceda essa permissão apenas aos aplicativos que você confia para atenderem aos seus requisitos de proteção de dados.

## <a name="subscribe-to-call-records"></a>Inscrever-se nos registros de chamada

Organizações e parceiros geralmente têm suas próprias ferramentas para gerar relatórios sobre chamadas e reuniões online. Usando webhooks, eles podem receber um feed contínuo de registros de chamada à medida que são criados. Esse modelo de push permite que organizações e parceiros criem suas próprias soluções de relatório em tempo real.

## <a name="look-up-a-call-record-by-its-call-id"></a>Procurar um registro de chamada por meio de sua ID de chamada

Os aplicativos podem recuperar [um registro de chamada](/graph/api/resources/callrecords-callrecord.md) por sua ID. Essa ID pode ser determinada a partir de uma notificação de webhook ou recuperada de ferramentas administrativas.

## <a name="get-call-record-reports"></a>Obter relatórios de registro de chamada

As organizações que usam Microsoft Teams para se conectar à PSTN (rede telefônica pública comutado) geralmente querem rastrear esse uso para entender os custos associados. As [funções getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls) e [getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls) [](/graph/api/resources/callrecords-callrecord) retornam uma projeção de dados de registro de chamada em um formato tabular.

## <a name="see-also"></a>Confira também

- [Permissões dos registros de chamadas](./permissions-reference.md#call-records-permissions)
