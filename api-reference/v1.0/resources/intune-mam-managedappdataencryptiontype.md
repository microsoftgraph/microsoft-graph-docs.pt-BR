---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 67c74dea08eac63fe22aa003af1c282be85669b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038056"
---
# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enumeração managedAppDataEncryptionType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|,0|Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.|
|afterDeviceRestart|1|Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|duas|Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos|
|whenDeviceLocked|3D|Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado|



