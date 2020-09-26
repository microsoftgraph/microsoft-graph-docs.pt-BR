---
title: Visão geral dos registros de chamadas
description: Os registros de chamadas fornecem informações sobre as chamadas e reuniões que ocorrem em sua organização.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 3abe4cb576a546089febce20da10fa8f9409eb7b
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289446"
---
# <a name="call-records-overview"></a>Visão geral dos registros de chamadas

Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business. Os dados de uso e diagnóstico podem ser consumidos para produzir relatórios personalizados para sua empresa para ajudar a monitorar a adoção ou solucionar problemas de qualidade de chamada.

As organizações podem assinar alterações em registros de chamadas usando o recurso de [assinaturas de webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) do Microsoft Graph, permitindo que eles criem relatórios quase em tempo real dos dados ou Alertem em determinados cenários, como chamadas de emergência.

> **Importante:** Use o critério ao conceder a permissão CallRecords. Read. All para aplicativos. Os registros de chamadas podem fornecer informações sobre a operação de sua empresa e, portanto, podem ser um alvo de atores mal-intencionados. Conceda essa permissão apenas aos aplicativos que você confia para atenderem aos seus requisitos de proteção de dados.

## <a name="subscribe-to-call-records"></a>Inscrever-se em registros de chamadas

As organizações e parceiros geralmente têm suas próprias ferramentas para gerar relatórios sobre chamadas e reuniões online. Usando WebHooks, eles podem receber um feed contínuo de registros de chamadas à medida que são criados. Esse modelo de push permite que as organizações e parceiros criem suas próprias soluções de relatórios em tempo real.

## <a name="look-up-a-call-record-by-its-call-id"></a>Pesquisar um registro de chamadas por ID de chamada

Os aplicativos podem recuperar um [registro de chamada](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) por sua ID. Essa ID pode ser determinada de uma notificação de webhook ou recuperada das ferramentas administrativas.

## <a name="get-call-record-reports"></a>Obter relatórios de registros de chamadas

As organizações que usam o Microsoft Teams para se conectar à PSTN (rede telefônica pública comutada) geralmente querem rastrear esse uso para entender os custos associados. As funções [getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) e [getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) retornam uma projeção de dados de [registro de chamada](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) em um formato tabular.

## <a name="see-also"></a>Confira também

- [Permissões dos registros de chamadas](./permissions-reference.md#call-records-permissions)