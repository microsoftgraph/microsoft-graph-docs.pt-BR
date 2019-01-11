---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f57904d45b24f6aaae9d67394facb07692add67e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834143"
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



