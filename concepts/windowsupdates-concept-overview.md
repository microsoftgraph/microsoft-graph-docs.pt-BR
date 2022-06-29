---
title: Visão geral da API de atualizações do Windows
description: O Windows Update de implantação do Windows Update business dá controle à sua organização sobre as atualizações oferecidas aos seus dispositivos.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: e6bb301bac7a261db8284ad40a5914a11cca5171
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437524"
---
# <a name="windows-updates-api-overview"></a>Visão geral da API de atualizações do Windows

O Windows Update de implantação do Windows Update business fornece controle sobre as atualizações de dispositivo por meio da capacidade de aprovar, agendar e proteger o conteúdo fornecido pelo Windows Update.

## <a name="why-use-the-windows-update-for-business-deployment-service"></a>Por que usar o serviço Windows Update implantação do Windows Update Business?

Profissionais de TI e fornecedores de ferramentas de gerenciamento podem usar o serviço de implantação para:
* Agende implantações de atualização para começar em uma data específica.
* Preparar implantações em um período de dias ou semanas usando expressões avançadas.
* Ignore as políticas de Windows Update para Empresas pré-configuradas para implantar imediatamente uma atualização de segurança.
* Garanta a cobertura de hardware e software em sua organização por meio de implantações adaptadas para populações exclusivas de dispositivos.

Atualmente, o serviço de implantação dá suporte ao gerenciamento de atualizações de recursos do Windows e à agilizar as atualizações de segurança do Windows. Para saber mais sobre o serviço de implantação no contexto do Windows Update for Business, consulte [Visão geral do serviço de implantação](/windows/deployment/update/deployment-service-overview).

## <a name="prerequisites"></a>Pré-requisitos

Para usar o serviço de implantação, sua organização deve ter uma das seguintes assinaturas:
* Windows 10 Enterprise E3 ou E5 (incluído no Microsoft 365 F3, E3 ou E5)
* Windows 10 Education A3 ou A5 (incluído no Microsoft 365 A3 ou A5)
* Acesso À Área de Trabalho Virtual do Windows E3 ou E5
* Microsoft 365 Business Premium

Além disso, os dispositivos gerenciados pelo serviço de implantação devem:
* Ser Azure AD ingressado ou ingressado no AD Híbrido
* Execute uma das seguintes edições Windows 10: Windows 10 Pro, Windows 10 Enterprise, Windows 10 Education, Windows 10 Pro Education
* Instalei a Windows 10 versão 1709 ou posterior

## <a name="enroll-devices-to-be-managed"></a>Registrar dispositivos a serem gerenciados

Para começar a usar o serviço de implantação, [registre dispositivos no gerenciamento de atualizações](windowsupdates-enroll.md).

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a>Aprovar e agendar o conteúdo do Windows fornecido do Windows Update

O serviço de implantação simplifica a revisão, aprovação, agendamento e implantação de conteúdo para um ecossistema diversificado de dispositivos. Existe um catálogo de atualizações para fornecer uma exibição personalizada para aprovações, ajudando você a se concentrar em decisões de aprovação importantes e evitar a necessidade de classificar por meio de listas profundas de atualizações relacionadas.

Depois de escolher uma atualização a ser implantada, você poderá agendar implantações para iniciar em um momento futuro ou implantá-la durante um período de tempo. Se você optar por implantar uma atualização durante um período de tempo, o serviço de implantação otimizará automaticamente a ordem na qual os dispositivos são oferecidos atualizações. Quando possível, o serviço ordena dispositivos para garantir que uma diversidade de ativos de hardware e software seja representada no início da implantação para minimizar o número de dispositivos que podem encontrar um problema de atualização inesperado. 

Saiba mais sobre o serviço de implantação:
* [Atualizações de software](windowsupdates-software-updates.md)
* [Implantações](windowsupdates-deployments.md)
* [Agendar uma implantação](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a>Implantar imediatamente uma atualização quando surgirem necessidades críticas

No caso de um problema de segurança crítico, você pode usar o serviço de implantação para ignorar uma política de atualização padrão e agilizar a implantação de uma atualização de segurança.

Para saber mais, confira [Implantar uma atualização de segurança acelerada](windowsupdates-deploy-expedited-update.md).

## <a name="protect-devices-by-default"></a>Proteger dispositivos por padrão

Aproveite o benefício [das retenções](/windows/deployment/update/safeguard-holds) de proteção que impedem que dispositivos com um problema de qualidade ou compatibilidade instalem uma atualização, resultando em falha ou reversão caso contrário. Para implantações de Windows 11, o serviço de implantação estende essas retenções de proteção para proteger ainda mais os dispositivos. A Microsoft usa algoritmos de aprendizado de máquina para monitorar a amplitude do ecossistema do Windows à medida que os dispositivos são atualizados para Windows 11. Para dispositivos identificados com maior risco de ter um problema pós-atualização, o serviço de implantação aplica proteções antecipadas para proteger esses dispositivos enquanto o problema é investigado e confirmado.

Para saber mais, confira [Gerenciar proteções para uma implantação](windowsupdates-manage-safeguards.md).

Além disso, você pode configurar regras de monitoramento exclusivas para sua organização. Essas regras podem enviar um alerta ou pausar uma implantação com base em sinais de dispositivo, como reversões.

Para saber mais, confira [Gerenciar regras de monitoramento para uma implantação](windowsupdates-manage-monitoring-rules.md).

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

Consulte [a API de atualizações do Windows no Microsoft Graph beta](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true).
