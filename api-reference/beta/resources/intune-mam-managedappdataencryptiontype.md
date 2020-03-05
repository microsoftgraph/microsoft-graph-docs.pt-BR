---
title: tipo de enumeração managedAppDataEncryptionType
description: Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 62e329c2fa400689c708b4155ea5145bc8eaed34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527950"
---
# <a name="managedappdataencryptiontype-enum-type"></a>tipo de enumeração managedAppDataEncryptionType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível ao qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|,0|Os dados do aplicativo são criptografados com base nas configurações padrão do dispositivo.|
|afterDeviceRestart|1 |Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|2 |Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado, exceto dados em arquivos que estão abertos|
|whenDeviceLocked|3 |Os dados de aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado|



