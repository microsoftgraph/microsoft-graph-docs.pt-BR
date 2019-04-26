---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 962e759e83b08baf7fc150e07dc84ed7146feb0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563851"
---
# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enumeração managedAppDataEncryptionType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|,0|Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.|
|afterDeviceRestart|1 |Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|2 |Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos|
|whenDeviceLocked|3 |Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado|





