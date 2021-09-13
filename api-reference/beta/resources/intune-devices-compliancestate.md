---
title: tipo de número de complianceState
description: Estado de conformidade.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 051cc43f82dc1ed9a2e1155778eb111387219b86
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111015"
---
# <a name="compliancestate-enum-type"></a>tipo de número de complianceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Desconhecido.|
|compatível|1|Compatível.|
|noncompliant|2|O dispositivo não é compatível e é bloqueado de recursos corporativos.|
|conflict|3|Conflita com outras regras.|
|erro|4 |Erro|
|inGracePeriod|254|O dispositivo não é compatível, mas ainda tem acesso a recursos corporativos|
|configManager|255|Gerenciado pelo Gerenciador de Configurações|



