---
title: tipo de número androidManagedStoreAutoUpdateMode
description: Priorização para atualizações automáticas de aplicativos da Loja Gerenciada do Android definidos na atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b571d8f1667d3a2eb7ccbde5bf0cefe176716a9c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337473"
---
# <a name="androidmanagedstoreautoupdatemode-enum-type"></a>tipo de número androidManagedStoreAutoUpdateMode

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Priorização para atualizações automáticas de aplicativos da Loja Gerenciada do Android definidos na atribuição.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Padrão.|0|Comportamento de atualização padrão (o dispositivo deve estar conectado ao Wifi, carregando e não usado ativamente).|
|adiada|1|As atualizações são adiadas por um máximo de 90 dias após o aplicativo ficar desa datado.|
|prioridade|2|O aplicativo é atualizado assim que possível pelo desenvolvedor. Se o dispositivo estiver online, ele será atualizado em minutos.|
|unknownFutureValue|3|Modo futuro desconhecido (reservado, não usado no momento).|




