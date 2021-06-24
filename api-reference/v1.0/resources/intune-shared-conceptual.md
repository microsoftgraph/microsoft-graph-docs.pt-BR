---
title: Recursos compartilhados em Microsoft Intune
description: Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.  A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 0af56b1ec3014fdee14dc4b70d3c14208321581a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108884"
---
# <a name="shared-resources-in-microsoft-intune"></a>Recursos compartilhados em Microsoft Intune

Namespace: microsoft.graph

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

Esses pontos de extremidade são usados em várias API do Microsoft Graph para fluxos de trabalho do Intune.  A intenção, a finalidade e as permissões necessárias para usar um determinado recurso varia de acordo com o fluxo de trabalho específico e o contexto da chamada subjacente.  Além disso, determinados métodos, propriedades e ações são suportados apenas para fluxos de trabalho específicos.

Os seguintes Graph são compartilhados entre fluxos de trabalho do Intune:  

- [Destino de atribuição de todos os dispositivos](intune-shared-alldevicesassignmenttarget.md)
- [Destino de atribuição de todos os usuários licenciados](intune-shared-alllicensedusersassignmenttarget.md)
- [Android enterprise sempre no tipo de pacote VPN](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [Status de conformidade](intune-shared-compliancestatus.md)
- [Destino da atribuição da coleção configuration manager](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [Destino de atribuição de gerenciamento de aplicativo e dispositivo](intune-shared-deviceandappmanagementassignmenttarget.md)
- [Destino de atribuição de grupos de exclusão](intune-shared-exclusiongroupassignmenttarget.md)
- [Destino de atribuição de grupo](intune-shared-groupassignmenttarget.md)
- [Intenção de instalação](intune-shared-installintent.md)
- [Conteúdo MIME](intune-shared-mimecontent.md)
- [Opções de geração do estado da interface do usuário salvas](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [Tipo de conta do token VPP](intune-shared-vpptokenaccounttype.md)