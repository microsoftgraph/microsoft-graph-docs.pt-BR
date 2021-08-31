---
title: deviceManagementConfigurationTemplateFamily enum type
description: Descreve TemplateFamily para a entidade Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5a4544dfbd9f87114d7e1cc83102a88aaa1a2c1d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791843"
---
# <a name="devicemanagementconfigurationtemplatefamily-enum-type"></a>deviceManagementConfigurationTemplateFamily enum type

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve TemplateFamily para a entidade Template

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Padrão para a família de modelos quando a política não está vinculada a um modelo|
|endpointSecurityAntivirus|10 |Família de Modelos para EndpointSecurityAntivirus que gerencia o grupo discreto de configurações de antivírus para dispositivos gerenciados|
|endpointSecurityDiskEncryption|11 |Família de Modelos para EndpointSecurityDiskEncryption que fornece configurações relevantes para um método de criptografia integrado de dispositivos, como FileVault ou BitLocker|
|endpointSecurityFirewall|12 |Família de Modelos para EndpointSecurityFirewall que ajuda a configurar um firewall integrado de dispositivos para dispositivos que executem macOS e Windows 10|
|endpointSecurityEndpointDetectionAndResponse|13|Família de modelos para EndpointSecurityEndpointDetectionAndResponse que facilita o gerenciamento das configurações EDR e dispositivos de integração do Microsoft Defender para Ponto de Extremidade|
|endpointSecurityAttackSurfaceReduction|14 |Família de Modelos para EndpointSecurityAttackSurfaceReduction que ajudam a reduzir suas superfícies de ataque, minimizando os locais onde sua organização está vulnerável a ameaças cibernéticas e ataques|
|endpointSecurityAccountProtection|15 |Família de modelos para EndpointSecurityAccountProtection que facilita a proteção da identidade e contas dos usuários|
|endpointSecurityApplicationControl|16 |Família de Modelos para ApplicationControl que ajuda a reduzir as ameaças de segurança restringindo os aplicativos que os usuários podem executar e o código que é executado no System Core (kernel)|



