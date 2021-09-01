---
title: tipo de número actionState
description: Estado da ação no dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 248e268eff326f3b5280cf237d90b37e2c56702b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801042"
---
# <a name="actionstate-enum-type"></a>tipo de número actionState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado da ação no dispositivo

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Não é um estado de ação válido|
|pendente|1|A ação está pendente|
|cancelado|2|A ação foi cancelada.|
|active|3|A ação está ativa.|
|done|4 |Ação concluída sem erros.|
|failed|5 |Falha na ação|
|notSupported|6 |Não há suporte para ação.|



