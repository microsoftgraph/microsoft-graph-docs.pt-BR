---
title: Regras de negócios a serem seguidas ao criar ou atualizar Bookings compromissos usando o Microsoft Graph
description: Este artigo descreve as regras de negócios a serem seguidas ao usar as APIs de criação ou atualização Bookings compromissos no Microsoft Graph.
ms.localizationpriority: medium
author: kwekua
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: e1f4a18fcf48d3d18b90a585f48926df1e6aa264
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755709"
---
# <a name="business-rules-for-bookings-appointments"></a>Regras de negócios para Bookings compromissos

Quando um usuário não administrador cria um compromisso no Microsoft Bookings, o Bookings usa as regras de negócios configuradas para o calendário. Somente os administradores têm a autoridade para substituir Bookings regras.

Os usuários finais ou aplicativos que criam ou atualizam compromissos por meio de APIs do Microsoft Graph (usando permissões de aplicativo) devem seguir as regras de negócio para evitar erros imprevistos.

Se você [usar as](/graph/api/bookingbusiness-post-appointments) APIs [de criação](/graph/api/bookingappointment-update) ou atualização de compromisso com permissões de aplicativo, deverá seguir as regras de negócios descritas neste artigo.

## <a name="business-settings"></a>Configurações de negócios

### <a name="business-hours"></a>Horário comercial

Use a API [update bookingBusiness](/graph/api/bookingbusiness-update?view=graph-rest-beta&tabs=http) para modificar **businessHours**. Observe que um compromisso não pode ser definido fora do horário comercial.

### <a name="scheduling-policy"></a>Política de agendamento

Para obter detalhes sobre a política de agendamento, consulte [bookingSchedulingPolicy](/graph/api/resources/bookingschedulingpolicy).

**Incrementos de tempo (intervalo de intervalo de tempo)** indicam a duração de um compromisso. Ao validar as regras de negócio, verifique se um compromisso tem a mesma duração indicada no serviço.

**O tempo de entrega** mínimo indica o tempo mínimo antes que um compromisso possa ser feito ou cancelado.

**O tempo máximo de** entrega indica o tempo máximo antes que um compromisso possa ser feito.  

**Permitir a** seleção da equipe é que, se um usuário quiser passar membros da equipe por meio da API de compromisso, ele deverá definir o atributo **allowStaffSelection** no tipo de recurso [BookingSchedulingPolicy](/graph/api/resources/bookingschedulingpolicy) como true.

> [!NOTE]
> Essa configuração é chamada **de Controle de** equipe no Bookings Web.

## <a name="service-level-settings"></a>Configurações de nível de serviço

### <a name="scheduling"></a>Agendar

Em um nível de serviço, a política de agendamento é herdada da empresa. O cliente pode optar por substituir as políticas.

### <a name="main-policy"></a>Política principal  

Se existir uma política de agendamento no nível de serviço e no nível de negócios, a política de nível de serviço terá precedência.

### <a name="partially-set-policies"></a>Políticas parcialmente definidas

Se o usuário não definir uma política para a política de nível de serviço, ele usará como padrão a configuração de política de nível de negócios.

### <a name="pre-buffer"></a>Pré-buffer

Esse é o tempo extra necessário para um compromisso antes de um compromisso a seguir. No calendário do membro da equipe, o compromisso tem a duração "tempo de pré-buffer" + "tempo do slot de compromisso".

### <a name="post-buffer"></a>Pós-buffer

Esse é o tempo extra necessário para um compromisso após um compromisso anterior. No calendário do membro da equipe, o compromisso tem a duração "tempo do slot de compromisso" + "tempo de pós-buffer".
