---
title: Tipo de enumeração deviceEnrollmentConfigurationType
description: Descreve o TemplateFamily para a entidade Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98fef8c27ca10a613c02132a4cd80fb8ab909205
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211316"
---
# <a name="deviceenrollmentconfigurationtype-enum-type"></a>Tipo de enumeração deviceEnrollmentConfigurationType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o TemplateFamily para a entidade Template

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Padrão. Defina como desconhecido se o tipo de configuração não puder ser determinado.|
|limite|1|Indica que a configuração é do limite de tipo que se refere ao número de dispositivos que um usuário tem permissão para registrar.|
|platformRestrictions|2|Indica que a configuração é do tipo restrição de plataforma que se refere aos tipos de dispositivos que um usuário tem permissão para registrar.|
|windowsHelloForBusiness|3|Indica que a configuração é do tipo Windows Hello que se refere ao método de autenticação que os dispositivos usariam.|
|defaultLimit|4|Indica que a configuração é do tipo limite padrão que se refere aos tipos de dispositivos que um usuário tem permissão para registrar por padrão.|
|defaultPlatformRestrictions|5|Indica que a configuração é do tipo de restrição de plataforma padrão que se refere aos tipos de dispositivos que um usuário tem permissão para registrar por padrão.|
|defaultWindowsHelloForBusiness|6 |Indica que a configuração é do tipo padrão Windows Hello que se refere ao método de autenticação que os dispositivos usariam por padrão.|
|defaultWindows10EnrollmentCompletionPageConfiguration|7 |Indica que a configuração é do tipo página de status de registro padrão que se refere à página de inicialização exibida durante o OOBE em dispositivos do Autopilot por padrão.|
|windows10EnrollmentCompletionPageConfiguration|8 |Indica que a configuração é do tipo Página de status de registro que se refere à página de inicialização exibida durante o OOBE em dispositivos do Autopilot.|
|deviceComanagementAuthorityConfiguration|9 |Indica que a configuração é do tipo Comanagement Authority que se refere a políticas aplicadas a Co-Managed dispositivos.|
|singlePlatformRestriction|10|Indica que a configuração é do tipo de restrição de plataforma única que se refere aos tipos de dispositivos que um usuário tem permissão para registrar.|
|unknownFutureValue|11|Valor futuro desconhecido|
|enrollmentNotificationsConfiguration|12 |Indica que a configuração é do tipo Notificação de Registro que se refere aos tipos de notificação que um usuário recebe durante o registro.|




