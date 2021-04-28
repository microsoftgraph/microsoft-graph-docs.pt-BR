---
title: Windows visão geral da API de atualizações
description: O Windows de implantação update for Business fornece controle à sua organização sobre as atualizações oferecidas aos seus dispositivos.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 98b75f278e33f56cf726a18c266000b06d817a6f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067653"
---
# <a name="windows-updates-api-overview"></a>Windows visão geral da API de atualizações

O Windows de implantação update for Business fornece controle sobre as atualizações de dispositivo por meio da capacidade de aprovar, agendar e proteger o conteúdo fornecido pelo Windows Update. 

## <a name="why-use-the-windows-update-for-business-deployment-service"></a>Por que usar o serviço de implantação Windows Atualização para Empresas?

Profissionais de TI e fornecedores de ferramentas de gerenciamento podem usar o serviço de implantação para:
* Agendar implantações de atualização para começar em uma data específica
* Implantações em estágios por um período de dias ou semanas usando expressões ricas
* Ignorar políticas pré-configuradas Windows Update for Business para implantar imediatamente uma atualização de segurança
* Garantir a cobertura de hardware e software em sua organização por meio de implantações personalizadas para populações exclusivas de dispositivos

Hoje, o serviço de implantação dá suporte ao gerenciamento Windows 10 de recursos e àgilizar Windows 10 de segurança. Para saber mais sobre o serviço de implantação no contexto do Windows Update for Business, consulte [Overview of the deployment service](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview).

## <a name="prerequisites"></a>Pré-requisitos    

Para usar o serviço de implantação, sua organização deve ter uma das seguintes assinaturas:
* Windows 10 Enterprise E3 ou E5 (incluído no Microsoft 365 F3, E3 ou E5)
* Windows 10 Education A3 ou A5 (incluído no Microsoft 365 A3 ou A5)
* Windows Virtual Desktop Access E3 ou E5
* Microsoft 365 Business Premium

Além disso, os dispositivos gerenciados pelo serviço de implantação devem:
* Ser ingressado no Azure AD ou Ingresso no AD Híbrido
* Execute uma das seguintes edições Windows 10: Windows 10 Pro, Windows 10 Enterprise, Windows 10 Education, Windows 10 Pro Education
* Ter instalado Windows 10 versão 1709 ou posterior

## <a name="enroll-devices-to-be-managed"></a>Registrar dispositivos a serem gerenciados

Para começar a usar o serviço de implantação, [inscreva dispositivos no gerenciamento de atualizações.](windowsupdates-enroll.md)

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a>Aprovar e agendar Windows conteúdo entregue do Windows Update

O serviço de implantação simplifica a revisão, aprovação, agendamento e implantação de conteúdo para um ecossistema de dispositivos diversificado. Existe um catálogo de atualizações para fornecer uma exibição personalizada para aprovações, ajudando você a se concentrar nas decisões de aprovação que importam e evitando a necessidade de classificar por meio de listas profundas de atualizações relacionadas.

Depois de escolher uma atualização para implantar, você pode agendar implantações para iniciar em uma hora futura ou implantar por um período de tempo. Se você optar por implantar uma atualização por um período de tempo, o serviço de implantação otimizará automaticamente a ordem na qual os dispositivos são oferecidos atualizações. Quando possível, o serviço ordena dispositivos para garantir que uma diversidade de ativos de hardware e software seja representada no início da implantação para minimizar o número de dispositivos que podem encontrar um problema de atualização inesperado. 

Saiba mais sobre o serviço de implantação:
* [Atualizações de software](windowsupdates-software-updates.md)
* [Implantações](windowsupdates-deployments.md)
* [Agendar uma implantação](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a>Implantar imediatamente uma atualização quando surgirem necessidades críticas

No caso de um problema crítico de segurança, você pode usar o serviço de implantação para ignorar uma política de atualização padrão e acelerar a implantação de uma atualização de segurança.

Para saber mais, confira [Implantar uma atualização de segurança acelerada.](windowsupdates-deploy-expedited-update.md)

## <a name="protect-devices-by-default"></a>Proteger dispositivos por padrão

Aproveite o benefício das [proteções](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) de proteção que impedem que dispositivos com um problema de qualidade ou compatibilidade instalem uma atualização, resultando em falha ou reação de outra forma.

Além disso, você pode configurar regras de monitoramento exclusivas da sua organização. Essas regras podem enviar um alerta ou pausar uma implantação com base em sinais de dispositivo, como reações.

Para saber mais, confira [Gerenciar regras de monitoramento para uma implantação](windowsupdates-manage-monitoring-rules.md).

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

Consulte [Windows API de atualizações no Microsoft Graph beta](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true).
