---
title: Tipo de número deviceEnrollmentConfigurationType
description: Descreve TemplateFamily para a entidade Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 85ffeb3b0d8215309b0667be4e0ba874aad66bfa
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63378703"
---
# <a name="deviceenrollmentconfigurationtype-enum-type"></a>Tipo de número deviceEnrollmentConfigurationType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve TemplateFamily para a entidade Template

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Padrão. Definir como desconhecido se o tipo de configuração não puder ser determinado.|
|limite|1|Indica que a configuração é do limite de tipo que se refere ao número de dispositivos que um usuário tem permissão para se registrar.|
|platformRestrictions|2|Indica que a configuração é do tipo restrição de plataforma que se refere aos tipos de dispositivos que um usuário tem permissão para se registrar.|
|windowsHelloForBusiness|3|Indica que a configuração é do tipo Windows Hello que se refere ao método de autenticação que os dispositivos usariam.|
|defaultLimit|4|Indica que a configuração é do tipo limite padrão que se refere aos tipos de dispositivos que um usuário tem permissão para se inscrever por padrão.|
|defaultPlatformRestrictions|5|Indica que a configuração é do tipo de restrição de plataforma padrão que se refere aos tipos de dispositivos que um usuário tem permissão para se registrar por padrão.|
|defaultWindowsHelloForBusiness|6 |Indica que a configuração é do tipo padrão Windows Hello que se refere ao método de autenticação que os dispositivos usariam por padrão.|
|defaultWindows10EnrollmentCompletionPageConfiguration|7 |Indica que a configuração é do tipo página de status de registro padrão que se refere à página de inicialização exibida durante o OOBE em dispositivos do Autopilot por padrão.|
|windows10EnrollmentCompletionPageConfiguration|8 |Indica que a configuração é do tipo Página de status de registro que se refere à página de inicialização exibida durante o OOBE em dispositivos do Autopilot.|
|deviceComanagementAuthorityConfiguration|9 |Indica que a configuração é do tipo Comanagement Authority que se refere às políticas aplicadas a Co-Managed dispositivos.|
|singlePlatformRestriction|10 |Indica que a configuração é do tipo de restrição de plataforma única que se refere a tipos de dispositivos que um usuário tem permissão para se registrar.|
|unknownFutureValue|11|Valor futuro desconhecido|




