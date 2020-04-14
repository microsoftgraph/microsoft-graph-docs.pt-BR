---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c088f3a0fc3a4bd4b01f29da5f228920f00a398f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465140"
---
# <a name="compliancestate-enum-type"></a>tipo de enumeração compliancestate

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|com|1|Com.|
|incompatível|duas|O dispositivo não está em conformidade e é bloqueado de recursos corporativos.|
|apresentar|3D|Conflito com outras regras.|
|erro|4 |Erro|
|inGracePeriod|254|O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos|
|configmanager|255|Gerenciado pelo Gerenciador de configuração|



