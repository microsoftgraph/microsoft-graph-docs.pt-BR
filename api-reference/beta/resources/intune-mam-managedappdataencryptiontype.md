---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dee810fde166cef7ada5b5500d4618499c51e879
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991930"
---
# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enumeração managedAppDataEncryptionType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|,0|Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.|
|afterDeviceRestart|1|Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|duas|Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos|
|whenDeviceLocked|3D|Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado|





