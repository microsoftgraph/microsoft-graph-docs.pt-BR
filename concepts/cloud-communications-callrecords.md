---
title: Chamar registros na API de comunicações na nuvem
description: Obtenha insights sobre as chamadas e reuniões online que ocorrem em sua organização ao usar o Microsoft Teams ou Skype for Business.
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: dc1c071ed6de21325fe154cc0a20f75e497d28c5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436338"
---
# <a name="call-records"></a>Registros de chamadas

Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business. Os dados de uso e diagnóstico podem ser consumidos para produzir relatórios personalizados para sua empresa para ajudar a monitorar a adoção ou solucionar problemas de qualidade de chamadas.

As organizações podem assinar alterações em registros de chamada usando a funcionalidade de [assinaturas de webhook](/graph/api/resources/webhooks) do Microsoft Graph, permitindo que elas criem relatórios quase em tempo real com base nos dados ou alertem em determinados cenários, como chamadas de emergência.

> [!IMPORTANT]
> Use o critério ao conceder a permissão CallRecords.Read.All aos aplicativos. Os registros de chamadas podem fornecer informações sobre a operação da sua empresa e, portanto, podem ser um destino para atores mal-intencionados. Conceda essa permissão apenas aos aplicativos que você confia para atenderem aos seus requisitos de proteção de dados.

## <a name="subscribe-to-call-records"></a>Assinar registros de chamada

Organizações e parceiros geralmente têm suas próprias ferramentas para gerar relatórios sobre chamadas e reuniões online. Usando webhooks, eles podem receber um feed contínuo de registros de chamada à medida que são criados. Esse modelo de push permite que organizações e parceiros criem suas próprias soluções de relatório em tempo real.

## <a name="look-up-a-call-record-by-its-call-id"></a>Pesquisar um registro de chamada por sua ID de chamada

Os aplicativos podem recuperar [um registro de chamada](/graph/api/resources/callrecords-callrecord) por sua ID. Essa ID pode ser determinada de uma notificação de webhook ou recuperada de ferramentas administrativas.

## <a name="get-call-record-reports"></a>Obter relatórios de registro de chamada

As organizações que usam o Microsoft Teams para se conectar à PSTN (rede telefônica pública comuada) geralmente querem acompanhar esse uso para entender os custos associados. As [funções getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls) e [getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls) retornam uma projeção [](/graph/api/resources/callrecords-callrecord) de dados de registro de chamada em um formato tabular.

## <a name="see-also"></a>Confira também

- [Permissões dos registros de chamadas](./permissions-reference.md#call-records-permissions)
- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)
