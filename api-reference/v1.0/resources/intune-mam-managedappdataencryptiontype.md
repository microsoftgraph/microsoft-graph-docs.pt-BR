---
title: Tipo de enumeração managedAppDataEncryptionType
description: Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d7480b7db8a28ef36a2ec0402de5024790881da
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734673"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Tipo de enumeração managedAppDataEncryptionType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|0|Os dados do aplicativo são criptografados com base nas configurações padrão no dispositivo.|
|afterDeviceRestart|1|Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|2|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado, exceto os dados em arquivos abertos|
|whenDeviceLocked|3|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado|





