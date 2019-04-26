---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c462df866b3c711bf4738c70ad4a1b0d68ceeb4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549122"
---
# <a name="compliancestate-enum-type"></a>tipo de enumeração compliancestate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|com|1 |Com.|
|incompatível|2 |O dispositivo não está em conformidade e é bloqueado de recursos corporativos.|
|apresentar|3 |Conflito com outras regras.|
|erro|4 |Erro|
|inGracePeriod|254|O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos|
|configmanager|255|Gerenciado pelo Gerenciador de configuração|





