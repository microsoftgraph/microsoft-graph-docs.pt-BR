---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006267"
---
# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enum managedAppDataEncryptionType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|0|Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.|
|afterDeviceRestart|1|Dados de aplicativo são criptografados quando o dispositivo for reiniciado.|
|whenDeviceLockedExceptOpenFiles|2|Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos|
|whenDeviceLocked|3|Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado|



