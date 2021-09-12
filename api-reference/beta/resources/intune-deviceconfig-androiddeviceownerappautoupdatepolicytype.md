---
title: tipo de número androidDeviceOwnerAppAutoUpdatePolicyType
description: Valores possíveis do Proprietário do Dispositivo Android para estados da política de atualização automática do aplicativo do dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9dcb3b22bd1a58f846ea696cfe88566478814a58
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017559"
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



