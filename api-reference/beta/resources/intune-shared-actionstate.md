---
title: tipo de número actionState
description: Estado da ação no dispositivo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c23caa7638054d50cd12c0081312f534d37f06bf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039305"
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



