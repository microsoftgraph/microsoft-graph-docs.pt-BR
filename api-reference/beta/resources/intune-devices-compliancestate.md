---
title: tipo de número de complianceState
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9bc115882461351f28a954f35be7267fca3c1c1b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791836"
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



