---
title: Visão geral do PC na nuvem do Windows 365 no Microsoft Graph
description: Windows 365 é um serviço baseado em nuvem que provisiona e hospeda PCs na nuvem como máquinas virtuais para usuários finais.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
ms.openlocfilehash: 3aada87e5f1087beb0f62b6fd2972edbcb0e6454
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589328"
---
# <a name="overview-for-windows-365-cloud-pc-on-microsoft-graph-preview"></a>Visão geral do PC na nuvem do Windows 365 no Microsoft Graph (visualização)

Windows 365 é um serviço baseado em nuvem que provisiona e hospeda PCs na nuvem como máquinas virtuais para usuários finais. Os administradores podem configurar, gerenciar e dimensionar facilmente Windows 365 de nuvem para se ajustar às necessidades da organização. Os usuários finais individuais podem transmitir com segurança sua experiência de Windows personalizada , incluindo seus aplicativos, dados, conteúdo e configurações, da nuvem da Microsoft para qualquer dispositivo, a qualquer momento, com seus PC na nuvem do Windows 365.

## <a name="why-integrate-with-windows-365-cloud-pcs"></a>Por que se integrar com Windows 365 Cloud PCs? 

Ao integrar e criar em cima de Windows 365, você pode provisionar, gerenciar e proteger os PCs de Nuvem para usuários finais o mais rápido e facilmente possível. Usando o microsoft API do Graph, você pode provisionar PCs de nuvem, gerenciar imagens de dispositivo, criar e executar verificações de saúde em conexões de rede do Azure, criar e atribuir políticas de provisionamento e muito mais.  

### <a name="create-azure-network-connections"></a>Criar conexões de rede do Azure

Crie [conexões de rede do Azure](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) para dar linha de visão a um controlador de domínio. Uma vez criada, se não estiver em uso, uma conexão de rede do Azure poderá ser excluída. Verificações de saúde também podem ser executados em uma conexão de rede do Azure para verificar seu status de saúde e, se necessário, a senha de domínio do AD pode ser atualizada. 

### <a name="provision-cloud-pcs"></a>Provisione PCs na nuvem

Crie [políticas de provisionamento](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) e atribua a grupos de usuários para provisionar PCs na Nuvem a eles quando eles também têm licenças atribuídas. Após a criação de política de provisionamento, você também pode listar, atualizar e excluir políticas de provisionamento. 

### <a name="upload-device-images"></a>Upload de dispositivo

Upload e gerenciar imagens do sistema operacional [](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) para PCs na Nuvem para determinar qual versão do Windows com quais aplicativos e outros detalhes de imagem devem ser usados para PCs de Nuvem quando provisionados.  

### <a name="view-end-users-cloud-pcs-and-their-properties"></a>Exibir os PCs de Nuvem dos usuários finais e suas propriedades

Depois de provisionado, liste e exibirá os [PCs de Nuvem](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) dos usuários finais e todas as propriedades associadas. Essa visibilidade do Cloud PC permite o gerenciamento hands-on e a facilidade de solução de problemas quando necessário. 

## <a name="api-reference"></a>Referência da API

Procurando a referência da API para o serviço?
- [Trabalhando com Cloud PCs do Windows 365 usando a API do Microsoft Graph](/graph/api/resources/cloudpc-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-step"></a>Próxima etapa

- Experimente as APIs Windows 365 Cloud PCs usando o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
