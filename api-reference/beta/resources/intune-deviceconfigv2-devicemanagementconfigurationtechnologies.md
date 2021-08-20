---
title: tipo de número deviceManagementConfigurationTechnologies
description: Descreve com qual tecnologia essa configuração pode ser implantada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9c935c1f69e843940a9e4aa29199dbfd9b5a02aa3528f7612c72055ab3f2efbc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185793"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>tipo de número deviceManagementConfigurationTechnologies

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve com qual tecnologia essa configuração pode ser implantada

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|A configuração não pode ser implantada por meio de qualquer canal|
|mdm|1 |A configuração pode ser implantada por meio do canal MDM|
|windows10XManagement|2|A configuração pode ser implantada por meio do canal Windows10XManagement|
|configManager|4 |A configuração pode ser implantada por meio do canal ConfigManager|
|microsoftSense|128|A configuração pode ser implantada por meio do canal do agente SENSE|




