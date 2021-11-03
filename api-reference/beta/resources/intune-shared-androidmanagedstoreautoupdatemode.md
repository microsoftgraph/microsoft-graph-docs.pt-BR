---
title: tipo de número androidManagedStoreAutoUpdateMode
description: Priorização para atualizações automáticas de aplicativos da Loja Gerenciada do Android definidos na atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: adaca71257f5ee18cec8af62bfaf1e12d201ba3f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695495"
---
# <a name="androidmanagedstoreautoupdatemode-enum-type"></a>tipo de número androidManagedStoreAutoUpdateMode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Priorização para atualizações automáticas de aplicativos da Loja Gerenciada do Android definidos na atribuição.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Padrão.|0|Comportamento de atualização padrão (o dispositivo deve estar conectado ao Wifi, carregando e não usado ativamente).|
|adiada|1|As atualizações são adiadas por um máximo de 90 dias após o aplicativo ficar desa datado.|
|prioridade|2|O aplicativo é atualizado assim que possível pelo desenvolvedor. Se o dispositivo estiver online, ele será atualizado em minutos.|
|unknownFutureValue|3|Modo futuro desconhecido (reservado, não usado no momento).|



