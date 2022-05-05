---
title: Tipo de enumeração zebraFotaConnectorState
description: Representa vários estados para o conector zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d7d5e8dfd7413b43f7ac1835c7b4ce07c92480f9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212997"
---
# <a name="zebrafotaconnectorstate-enum-type"></a>Tipo de enumeração zebraFotaConnectorState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa vários estados para o conector zebra FOTA.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Valor padrão quando o conector não foi configurado (o recurso ainda não foi usado).|
|Conectado|1|O estado conectado indica que Intune está vinculado ao Zebra Update Services para o locatário atual.|
|Desconectado|2|O estado desconectado indica que a conta foi conectada no passado e depois desconectada.|
|unknownFutureValue|99|Valor de enumeração futuro desconhecido.|




