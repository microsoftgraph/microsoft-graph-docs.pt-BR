---
title: tipo de enum managedAppDataEncryptionType
description: Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413686"
---
# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enum managedAppDataEncryptionType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa o nível ao qual os dados de aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|0|Dados de aplicativo são criptografados com base nas configurações padrão no dispositivo.|
|afterDeviceRestart|1|Dados de aplicativo são criptografados quando o dispositivo for reiniciado.|
|whenDeviceLockedExceptOpenFiles|2|Dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto os dados em arquivos que estão abertos|
|whenDeviceLocked|3|Dados de aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado|




