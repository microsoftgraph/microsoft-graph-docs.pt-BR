---
title: Usar as APIs de conformidade e privacidade do Microsoft Graph
description: As APIs de conformidade e privacidade da Microsoft Graph fornecem uma interface unificada e um esquema para integração com as soluções disponíveis no centro de conformidade da Microsoft e dos parceiros do ecossistema. Isto pode ajudar os clientes a otimizar suas operações de conformidade e privacidade para melhor gerenciar e monitorar seus dados, proteger informações, minimizar riscos internos, realizar investigações legais e internas e cumprir com as normas legais ou regulamentares.
ms.localizationpriority: high
author: mahage-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: ea9cccfea27ba891010343428db4cdf037fb0844
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609728"
---
# <a name="use-the-microsoft-graph-compliance-and-privacy-apis"></a>Usar as APIs de conformidade e privacidade do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As APIs de conformidade e privacidade da Microsoft Graph fornecem uma interface unificada e um esquema para integração com as soluções disponíveis no centro de conformidade da Microsoft e dos parceiros do ecossistema. Isto pode ajudar os clientes a otimizar suas operações de conformidade e privacidade para melhor gerenciar e monitorar seus dados, proteger informações, minimizar riscos internos, realizar investigações legais e internas e cumprir com as normas legais ou regulamentares. Para mais informações, consulte a [ documentação do Centro de conformidade do Microsoft 365](/microsoft-365/compliance).

Utilize as APIs de conformidade e privacidade do Microsoft Graph para criar aplicativos que:

- Automatize tarefas comuns na Descoberta Eletrônica
- Criar e gerenciar solicitações de direitos do titular
- Automatizar tarefas no gerenciamento de registros

## <a name="ediscovery"></a>Descoberta eletrônica

A Descoberta Eletrônica no Microsoft 365 fornece um fluxo de trabalho completo para preservar, coletar, revisar, analisar e exportar dados que respondam às investigações internas e externas da sua organização. Saiba mais sobre a [Descoberta Eletrônica Avançada do Microsoft 365](/microsoft-365/compliance/overview-ediscovery-20).

Explorar as [APIs de Descoberta Eletrônica do Microsoft 365](ediscovery-ediscoveryapioverview.md).

## <a name="subject-rights-request"></a>Solicitação de direitos do titular

As Solicitações de Direitos do Titular Priva da Microsoft fornece recursos poderosos para ajudá-lo a lidar com solicitações de pessoas que procuram gerenciar seus dados pessoais dentro de sua organização. Esses pedidos são às vezes também chamados de Solicitações do titular dos dados (DSRs), Solicitações de acesso ao titular dos dados (DSARs), ou Solicitações de direitos do consumidor. O Microsoft Priva permite que o pessoal responsável pelo cumprimento das solicitações de direitos do titular a identificar facilmente os titulares dos dados e encontrar suas informações pessoais entre os dados de sua organização em Exchange, SharePoint, OneDrive e Teams. Saiba mais sobre as [Solicitações de Direitos do Titular Priva](/microsoft-365/compliance/privacy-management-subject-rights-requests).

Explore as [APIs de solicitação de direitos do titular](subjectrightsrequest-subjectrightsrequestapioverview.md).

## <a name="records-management-preview"></a>Gerenciamento de registros (versão prévia)

O gerenciamento de registros no Microsoft Purview fornece a capacidade de gerenciar registros regulatórios, legais e críticos para os negócios em dados corporativos. Ele ajuda as organizações a gerenciar a retenção e a exclusão de dados para cumprir suas obrigações legais e com os regulamentos de conformidade, e aumenta a eficiência, permitindo a disposição regular de itens que não precisam mais ser retidos.

Para obter mais detalhes, consulte [Gerenciamento de registros do Microsoft Purview](/microsoft-365/compliance/records-management).

A API de gerenciamento de registros é definida no subnamespace OData, microsoft.graph.security.
Explore as [APIs de gerenciamento de registros do Microsoft Purview](security-recordsManagement-overview.md).

<!--
## Labels

??? Labels should be moved from security to here.  They are currently under a node called Information protection.
-->
