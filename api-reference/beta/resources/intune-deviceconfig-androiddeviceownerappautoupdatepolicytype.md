---
title: tipo de número androidDeviceOwnerAppAutoUpdatePolicyType
description: Valores possíveis do Proprietário do Dispositivo Android para estados da política de atualização automática do aplicativo do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc427cb78e3a008f1fb2cc856217648bbb670015
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58779197"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>tipo de número androidDeviceOwnerAppAutoUpdatePolicyType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis do Proprietário do Dispositivo Android para estados da política de atualização automática do aplicativo do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Não configurado; esse valor é ignorado.|
|userChoice|1|O usuário pode controlar as atualizações automáticas.|
|never|2|Os aplicativos nunca são atualizados automaticamente.|
|wiFiOnly|3|Os aplicativos são atualizados automaticamente Wi-Fi somente.|
|always|4 |Os aplicativos são atualizados automaticamente a qualquer momento. Os encargos de dados podem ser aplicados.|



