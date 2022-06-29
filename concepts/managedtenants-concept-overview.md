---
title: Gerenciar vários locatários de clientes usando a API de Microsoft 365 Lighthouse
description: Microsoft 365 Lighthouse no Microsoft Graph ajuda os MSPs a gerenciar remotamente dispositivos, dados e usuários para clientes que usam Microsoft 365 Business Premium.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 8a59b310ef6ae5b5d50b423fc013b25bede133f4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440688"
---
# <a name="manage-multiple-customer-tenants-using-the-microsoft-365-lighthouse-api"></a>Gerenciar vários locatários de clientes usando a API de Microsoft 365 Lighthouse

Microsoft 365 Lighthouse é um portal de administração que permite que os MSPs (Provedores de Serviços Gerenciados) gerenciem remotamente vários locatários de clientes. Ele ajuda os MSPs a proteger e gerenciar dispositivos, dados e usuários em escala para clientes de pequenas e médias empresas (SMB) que estão usando Microsoft 365 Business Premium.

Microsoft 365 Lighthouse ajuda os MSPs a simplificar a integração Microsoft 365 Business Premium locatários do cliente. Ele oferece a um MSP a conveniência de exibições multilocatário em todos os seus ambientes de locatário do cliente. Ele pode recomendar linhas de base de configuração de segurança personalizadas para os clientes SMB do MSP. Com Microsoft 365 Lighthouse, os MSPs podem dimensionar o gerenciamento de seus locatários de clientes, se concentrar no que é mais importante, localizar e investigar rapidamente os riscos e tomar medidas para ajudar a colocar seus locatários do cliente em um estado íntegro e seguro.

> [!NOTE]  
> Esta documentação é sobre Microsoft 365 Lighthouse API disponível no _Microsoft Graph_. Uma oferta semelhante, o Azure Lighthouse, ajuda os provedores de serviços a fornecer serviços gerenciados para serviços do Azure usando ferramentas de gerenciamento abrangentes e robustas integradas à plataforma _do Azure_ . Para saber mais, confira [O que é o Azure Lighthouse](/azure/lighthouse/overview).

## <a name="why-integrate-with-microsoft-365-lighthouse"></a>Por que integrar com Microsoft 365 Lighthouse?

Como um MSP, você pode usar a API Microsoft 365 Lighthouse no Microsoft Graph para obter insights sobre os riscos identificados e tomar medidas para ajudar a colocar seus clientes em um estado íntegro e seguro.

### <a name="devices"></a>Dispositivos

Você pode usar a API do Lighthouse para executar as seguintes tarefas de dispositivo:

- Analise [as tendências de conformidade](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) do dispositivo para entender melhor como a conformidade do dispositivo está evoluindo ao longo do tempo para seus clientes.
- Entenda quais [políticas de conformidade do](/graph/api/resources/managedtenants-manageddevicecompliance) dispositivo foram criadas em seus clientes e o status das políticas.

### <a name="threat-management"></a>Gerenciamento de ameaças

Você pode usar a API do Lighthouse para executar as seguintes tarefas de gerenciamento de ameaças:

- Obtenha informações sobre o estado de [malware](/graph/api/resources/managedtenants-windowsdevicemalwarestate) que está presente nos dispositivos Windows registrados para gerenciamento em seus clientes.
- Exiba [o estado de proteção](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) para dispositivos Windows registrados para gerenciamento em seus clientes para garantir que os usuários Windows Defender estejam em um estado íntegro.

### <a name="users"></a>Usuários

Você pode usar a API do Lighthouse para executar as seguintes tarefas de usuário:

- Descubra [usuários arriscados](/graph/api/resources/riskyuser) entre seus clientes.
- [Exiba o resumo do registro de usuário de](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) credencial para entender quais usuários em seus clientes se registraram para autenticação multifator e redefinição de senha de autoatendimento.

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

Consulte [Microsoft 365 Lighthouse API no Microsoft Graph (versão prévia)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).

> [!NOTE]
> A MICROSOFT 365 LIGHTHOUSE api é definida no subnamespace OData. `microsoft.graph.managedTenants`


## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre o [Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) portal.
- Saiba mais sobre os [novos recursos e atualizações mais recentes para](/graph/whats-new-overview) a API do Lighthouse.
- Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.
