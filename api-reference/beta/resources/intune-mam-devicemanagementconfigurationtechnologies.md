---
title: Tipo de enumeração deviceManagementConfigurationTechnologies
description: Descreve com qual tecnologia essa configuração pode ser implantada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6efdc017f80a37529344f197c1d0e071a3936686
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671446"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>Tipo de enumeração deviceManagementConfigurationTechnologies

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve com qual tecnologia essa configuração pode ser implantada

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|A configuração não pode ser implantada por meio de qualquer canal|
|Mdm|1|A configuração pode ser implantada por meio do canal MDM|
|windows10XManagement|2|A configuração pode ser implantada por meio do canal Windows10XManagement|
|configManager|4|A configuração pode ser implantada por meio do canal ConfigManager|
|appleRemoteManagement|64|A configuração pode ser implantada por meio do canal AppleRemoteManagement|
|microsoftSense|128|A configuração pode ser implantada por meio do canal do agente SENSE|
|exchangeOnline|256|A configuração pode ser implantada por meio do canal Exchange Online agente|
|linuxMdm|1024|A configuração pode ser implantada por meio do canal Mdm do Linux|
|unknownFutureValue|1073741824|Membro do Sentinel para casos em que o cliente não pode manipular os novos valores de enumeração.|




