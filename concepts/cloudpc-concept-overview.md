---
title: PC na nuvem do Windows 365 no Microsoft Graph (versão prévia)
description: Integre-PC na nuvem do Windows 365 para criar conexões de rede do Azure, provisionar PCs na nuvem, gerenciar imagens de dispositivo e criar e atribuir políticas de provisionamento.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
ms.openlocfilehash: 75d67a10b12d15430c61a30bedc25eb5a8ab1bb6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442138"
---
# <a name="overview-for-windows-365-cloud-pc-on-microsoft-graph-preview"></a>Visão geral do PC na nuvem do Windows 365 no Microsoft Graph (versão prévia)

Windows 365 é um serviço baseado em nuvem que provisiona e hospeda PCs na nuvem como máquinas virtuais para usuários finais. Os administradores podem configurar, gerenciar e dimensionar facilmente Windows 365 PCs na nuvem para atender às necessidades da organização. Os usuários finais individuais podem transmitir com segurança sua experiência avançada e personalizada do Windows&mdash;, incluindo seus aplicativos&mdash;, dados, conteúdo e configurações da nuvem da Microsoft para qualquer dispositivo, a qualquer momento, com seus PC na nuvem do Windows 365.

## <a name="why-integrate-with-windows-365-cloud-pcs"></a>Por que integrar com Windows 365 na nuvem? 

Com a integração e a criação com base no Windows 365, você pode provisionar, gerenciar e proteger PCs na nuvem para os usuários finais o mais rápido e fácil possível. Usando o Microsoft API do Graph, você pode provisionar PCs na nuvem, gerenciar imagens de dispositivo, criar e executar verificações de integridade em conexões de rede do Azure, criar e atribuir políticas de provisionamento e muito mais.  

### <a name="create-azure-network-connections"></a>Criar as conexões de rede do Azure

Crie [conexões de rede do Azure](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) para dar linha de visão a um controlador de domínio. Depois de criada, se não estiver em uso, uma conexão de rede do Azure poderá ser excluída. As verificações de integridade também podem ser executadas em uma conexão de rede do Azure para verificar seu status de integridade e, se necessário, a senha de domínio do Active Directory pode ser atualizada. 

### <a name="provision-cloud-pcs"></a>Provisionar PCs na nuvem

Crie [políticas de provisionamento](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) e atribua a grupos de usuários para provisionar PCs na nuvem a eles quando eles também tiverem licenças atribuídas. Após a criação da política de provisionamento, você também pode listar, atualizar e excluir políticas de provisionamento. 

### <a name="upload-device-images"></a>Carregar imagens do dispositivo

Carregue e gerencie [](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) imagens do sistema operacional para PCs na nuvem para determinar qual versão do Windows com quais aplicativos e outros detalhes de imagem devem ser usados para PCs na nuvem quando provisionados.  

### <a name="view-end-users-cloud-pcs-and-their-properties"></a>Exibir computadores na nuvem dos usuários finais e suas propriedades

Depois de provisionado, liste e exiba os [computadores](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) na nuvem dos usuários finais e todas as propriedades associadas. Essa visibilidade do PC na nuvem permite o gerenciamento prático e a facilidade de solução de problemas quando necessário. 

## <a name="api-reference"></a>Referência da API

Procurando a referência de API para o serviço?

- [Trabalhando com Cloud PCs do Windows 365 usando a API do Microsoft Graph](/graph/api/resources/cloudpc-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-step"></a>Próxima etapa

- Experimente as APIs PC na nuvem do Windows 365 usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
