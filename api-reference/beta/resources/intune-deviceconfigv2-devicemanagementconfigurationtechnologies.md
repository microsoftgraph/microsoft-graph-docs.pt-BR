---
title: tipo de número deviceManagementConfigurationTechnologies
description: Descreve com qual tecnologia essa configuração pode ser implantada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fc7e240c4e48dfcab9974ff7c6ab4d1c30a629a8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335016"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>tipo de número deviceManagementConfigurationTechnologies

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve com qual tecnologia essa configuração pode ser implantada

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|A configuração não pode ser implantada por meio de qualquer canal|
|mdm|1|A configuração pode ser implantada por meio do canal MDM|
|windows10XManagement|2|A configuração pode ser implantada por meio do canal Windows10XManagement|
|configManager|4|A configuração pode ser implantada por meio do canal ConfigManager|
|microsoftSense|128|A configuração pode ser implantada por meio do canal do agente SENSE|
|exchangeOnline|256|A configuração pode ser implantada por meio do canal Exchange Online agente|
|linuxMdm|1024|A configuração pode ser implantada por meio do canal Mdm do Linux|
|unknownFutureValue|1073741824|Membro do Sentinel para casos em que o cliente não pode manipular os novos valores de numeração.|




