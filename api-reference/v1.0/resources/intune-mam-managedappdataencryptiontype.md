---
title: Tipo denum managedAppDataEncryptionType
description: Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a3cbe74f8dbc81330b899b4acedcbc880b8d81d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754494"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Tipo denum managedAppDataEncryptionType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|0|Os dados do aplicativo são criptografados com base nas configurações padrão no dispositivo.|
|afterDeviceRestart|1|Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|2|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado, exceto dados em arquivos que estão abertos|
|whenDeviceLocked|3|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado|




