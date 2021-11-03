---
title: Trabalhando com Windows 365 Cloud PCs usando a API Graph Microsoft
description: Com o Microsoft Graph, você pode provisionar e gerenciar PCs de Nuvem em sua organização e, se usado em conjunto com a API do Intune, você também pode gerenciar os PCs de Nuvem juntamente com pontos de extremidade físicos.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e4e205631424ed2f93b748371c8f32c31b4398ee
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695423"
---
# <a name="working-with-windows-365-cloud-pcs-using-the-microsoft-graph-api"></a>Trabalhando com Windows 365 Cloud PCs usando a API Graph Microsoft

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows 365 é um serviço baseado em nuvem que provisiona e hospeda PCs de nuvem como máquinas virtuais para usuários finais. Os administradores podem configurar, gerenciar e dimensionar facilmente Windows 365 PCs de Nuvem para se ajustar às necessidades da organização. Os usuários finais individuais podem transmitir com segurança sua experiência rica e personalizada Windows , incluindo seus aplicativos, dados, conteúdo e configurações, da nuvem da Microsoft para qualquer dispositivo, a qualquer momento, com seu computador Windows 365 Cloud.

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