---
title: Microsoft 365 Lighthouse Visão geral da API
description: Microsoft 365 Lighthouse é um portal de administração que ajuda os MSPs (Provedores de Serviços Gerenciados) a proteger e gerenciar dispositivos, dados e usuários em escala para clientes de pequenas e médias empresas (SMB) que estão usando o Microsoft 365 Business Premium.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 2c05851c8cffb445feb49b089112516f6d2133373490a150d0176d7a51d670b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236931"
---
# <a name="overview-for-multi-tenant-management-using-the-microsoft-365-lighthouse-api"></a>Visão geral do gerenciamento de vários locatários usando Microsoft 365 Lighthouse API

Microsoft 365 Lighthouse é um portal de administração que permite que os MSPs (Provedores de Serviços Gerenciados) gerenciem remotamente vários locatários de clientes. Ele ajuda os MSPs a proteger e gerenciar dispositivos, dados e usuários em escala para clientes de pequenas e médias empresas (SMB) que estão usando Microsoft 365 Business Premium.

Microsoft 365 Lighthouse ajuda os MSPs a simplificar a integração de Microsoft 365 Business Premium locatários do cliente. Ele oferece a um MSP a conveniência de exibições de vários locatários em todos os ambientes de locatários do cliente. Ele pode recomendar linhas de base de configuração de segurança personalizadas para os clientes SMB do MSP. Com Microsoft 365 Lighthouse, os MSPs podem dimensionar o gerenciamento de seus locatários de clientes, se concentrar no que é mais importante, encontrar e investigar riscos rapidamente e tomar medidas para ajudar a obter seus locatários de clientes para um estado íntegre e seguro.

> [!NOTE]  
> Esta documentação trata da API Microsoft 365 Lighthouse disponível no _Microsoft Graph_. Uma oferta semelhante, o Azure Lighthouse, ajuda os provedores de serviços a fornecer serviços gerenciados para serviços do Azure usando ferramentas de gerenciamento abrangentes e robustas integradas à plataforma _do Azure._ Para saber mais, confira [O que é o Farol do Azure.](/azure/lighthouse/overview)

## <a name="why-integrate-with-microsoft-365-lighthouse"></a>Por que se integrar Microsoft 365 Lighthouse?

Como um MSP, você pode usar a API Microsoft 365 Lighthouse no Microsoft Graph para obter informações sobre riscos identificados e tomar medidas para ajudar a obter seus clientes em um estado saudável e seguro.

### <a name="devices"></a>Dispositivos

Você pode usar a API do Farol para executar as seguintes tarefas de dispositivo:

- Analise [as tendências de conformidade](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) do dispositivo para entender melhor como a conformidade do dispositivo está evoluindo ao longo do tempo para seus clientes.
- Entenda quais [políticas de conformidade de](/graph/api/resources/managedtenants-manageddevicecompliance) dispositivo foram criadas em seus clientes e o status das políticas.

### <a name="threat-management"></a>Gerenciamento de ameaças

Você pode usar a API do Farol para executar as seguintes tarefas de gerenciamento de ameaças:

- Obtenha informações sobre o estado de [malware](/graph/api/resources/managedtenants-windowsdevicemalwarestate) presente nos dispositivos Windows registrados para gerenciamento em seus clientes.
- Exibir o [estado de proteção](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) para dispositivos Windows registrados para gerenciamento em seus clientes para garantir que os usuários Windows Defender estão em um estado saudável.

### <a name="users"></a>Usuários

Você pode usar a API do Farol para executar as seguintes tarefas de usuário:

- Descubra [usuários arriscados](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) em seus clientes.
- Exibir resumo do registro do usuário [de credencial](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) para entender o que os usuários em seus clientes registraram para autenticação multifaionária e redefinição de senha de autoatendados.

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

Consulte [Microsoft 365 Lighthouse API no Microsoft Graph (visualização)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).

> [!NOTE]
> A Microsoft 365 Lighthouse api é definida no subnamespace OData, `microsoft.graph.managedTenants` .


## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre o [Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) portal.
- Saiba mais sobre os [novos recursos e atualizações mais recentes para](/graph/whats-new-overview) a API do Farol.
- Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.
