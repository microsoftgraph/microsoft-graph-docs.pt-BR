---
title: Trabalhando com Cloud PCs do Windows 365 usando a API do Microsoft Graph
description: A API Graph microsoft habilita o acesso programático às ações de gerenciamento e informações do Cloud PC em sua organização.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 566c2e37c2b6ca6f36b6ef41d3f2911fc0539a6f
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123709"
---
# <a name="working-with-windows-365-cloud-pcs-using-the-microsoft-graph-api"></a>Trabalhando com Cloud PCs do Windows 365 usando a API do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Windows 365 é um serviço baseado em nuvem que cria automaticamente um tipo de máquina virtual do Windows (PCs na nuvem) para os seus usuários finais. Cada computador cloud é atribuído a um usuário individual como um dispositivo Windows exclusivo. O Windows 365 fornece os benefícios de produtividade, segurança e colaboração do Microsoft 365.

A API Graph microsoft habilita o acesso programático às ações de gerenciamento e informações do Cloud PC em sua organização. A API executa as mesmas operações que as disponíveis por meio Microsoft Endpoint Manager. 

> [!IMPORTANT]
> Usar a API Graph Microsoft para PCs na Nuvem requer uma licença [Windows 365](https://www.microsoft.com/windows-365) ativa para a organização. Atualmente, a API do Microsoft Graph está disponível para Windows 365 Enterprise e não Windows 365 Business. 

## <a name="using-the-microsoft-graph-api-for-cloud-pcs"></a>Usando a API Graph Microsoft para PCs na Nuvem

Com o Microsoft Graph, você pode provisioná-los e gerenciar os PCs de Nuvem em sua organização. Se usado em conjunto com a API do Intune, você também pode gerenciar os PCs de Nuvem junto com pontos de extremidade físicos. 

## <a name="using-microsoft-graph-permissions"></a>Uso das permissões do Microsoft Graph

O Microsoft Graph controla o acesso aos recursos por meio de permissões. Como desenvolvedor, você deve especificar as permissões que você precisa para acessar Windows 365 recursos. Normalmente, você deve especificar as permissões no portal do Azure Active Directory. Para obter mais informações, [consulte Referência](/graph/permissions-reference) Graph permissões da Microsoft e navegue até a seção Permissões do Cloud [PC.](/graph/permissions-reference#cloud-pc-permissions) 

## <a name="common-use-cases"></a>Casos de uso comuns

|Casos de uso|Recursos REST|Confira também|
|:---|:---|:---|
|Listar, obter, criar, atualizar, excluir ou atribuir políticas de provisionamento|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|[Visão geral do provisionamento](/windows-365/enterprise/provisioning)|
|Gerenciar computadores de nuvem, incluindo reprovisionamento, período de carência de computador na nuvem final, reprovisionamento em massa e resize computadores cloud|[cloudPC](../resources/cloudpc.md)|[Ciclo de vida de PCs na Nuvem](/windows-365/enterprise/lifecycle)|
|Listar, obter, criar, excluir, obter imagens de origem e reupcar imagens do sistema operacional do Cloud PC|[cloudPCDeviceImage](../resources/cloudpcdeviceimage.md)|[Visão geral das imagens do dispositivo](/windows-365/enterprise/device-images)|
|Listar, obter, criar, atualizar exclusão, atualizar senha de domínio do AD e executar verificações de saúde para conexões de rede locais|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|[Visão geral da conexão de rede local](/windows-365/enterprise/on-premises-network-connections)|
|Listar eventos de auditoria para PCs na Nuvem, obter um evento de auditoria específico e obter tipos de atividade de auditoria|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|[Obter logs de auditoria do Cloud PC](/windows-365/enterprise/get-cloud-pc-audit-logs-using-powershell)|
|Listar, obter, criar, atualizar, excluir ou atribuir configurações de usuário|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|[Visão geral das configurações do usuário](../resources/cloudpcusersetting.md)|

## <a name="whats-new"></a>Novidades

Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas
- Confira a visão [geral do Windows 365 Cloud PC no Microsoft Graph](/graph/cloudpc-concept-overview).
- Experimente as APIs Windows 365 Cloud PCs usando o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).