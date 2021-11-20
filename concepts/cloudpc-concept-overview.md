---
title: Visão geral do Windows 365 Cloud PC no Microsoft Graph
description: Windows 365 é um serviço baseado em nuvem que provisiona e hospeda PCs de nuvem como máquinas virtuais para usuários finais.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
ms.openlocfilehash: f0c8f2fe2e197a1f0b44d532e09438c889e5dc24
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2021
ms.locfileid: "61124144"
---
# <a name="overview-for-windows-365-cloud-pc-on-microsoft-graph-preview"></a>Visão geral do Windows 365 Cloud PC no Microsoft Graph (visualização)

Windows 365 é um serviço baseado em nuvem que provisiona e hospeda PCs de nuvem como máquinas virtuais para usuários finais. Os administradores podem configurar, gerenciar e dimensionar facilmente Windows 365 PCs de Nuvem para se ajustar às necessidades da organização. Os usuários finais individuais podem transmitir com segurança sua experiência rica e personalizada Windows , incluindo seus aplicativos, dados, conteúdo e configurações, da nuvem da Microsoft para qualquer dispositivo, a qualquer momento, com seu computador Windows 365 Cloud.

## <a name="why-integrate-with-windows-365-cloud-pcs"></a>Por que se integrar com Windows 365 Cloud PCs? 

Ao integrar e criar na parte superior do Windows 365, você pode provisionar, gerenciar e proteger os PCs de Nuvem para usuários finais o mais rápido e facilmente possível. Usando a API do Microsoft Graph, você pode provisionar PCs de nuvem, gerenciar imagens de dispositivo, criar e executar verificações de saúde em conexões de rede locais, criar e atribuir políticas de provisionamento e muito mais.  

### <a name="create-on-premises-network-connections"></a>Criar conexões de rede locais

Crie [conexões de rede locais](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) para dar linha de visão a um controlador de domínio. Uma vez criada, se não estiver em uso, uma conexão de rede local poderá ser excluída. Verificações de saúde também podem ser executados em uma conexão de rede local para verificar seu status de saúde e, se necessário, a senha de domínio do AD pode ser atualizada. 

### <a name="provision-cloud-pcs"></a>Provisione PCs na nuvem

Crie [políticas de provisionamento](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) e atribua a grupos de usuários para provisionar PCs na Nuvem a eles quando eles também têm licenças atribuídas. Após a criação de política de provisionamento, você também pode listar, atualizar e excluir políticas de provisionamento. 

### <a name="upload-device-images"></a>Upload de dispositivo

Upload e gerenciar imagens [](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) do sistema operacional para PCs de Nuvem para determinar qual versão do Windows com quais aplicativos e outros detalhes de imagem devem ser usados para PCs na Nuvem quando provisionados.  

### <a name="view-end-users-cloud-pcs-and-their-properties"></a>Exibir os PCs de Nuvem dos usuários finais e suas propriedades

Depois de provisionado, liste e exibirá os PCs de [Nuvem](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) dos usuários finais e todas as propriedades associadas. Essa visibilidade do Cloud PC permite o gerenciamento hands-on e a facilidade de solução de problemas quando necessário. 

## <a name="api-reference"></a>Referência da API

Procurando a referência da API para o serviço?
- [Trabalhando com Cloud PCs do Windows 365 usando a API do Microsoft Graph](/graph/api/resources/cloudpc-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-step"></a>Próxima etapa

- Experimente as APIs Windows 365 Cloud PCs usando o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
