---
title: Tipo denum managedAppDataEncryptionType
description: Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8cc9e89b13d69a56a9aa0d232bcde84284ffb45c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075120"
---
# <a name="managedappdataencryptiontype-enum-type"></a>Tipo denum managedAppDataEncryptionType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o nível para o qual os dados do aplicativo são criptografados para aplicativos gerenciados

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useDeviceSettings|0|Os dados do aplicativo são criptografados com base nas configurações padrão no dispositivo.|
|afterDeviceRestart|1|Os dados do aplicativo são criptografados quando o dispositivo é reiniciado.|
|whenDeviceLockedExceptOpenFiles|2|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo está bloqueado, exceto dados em arquivos que estão abertos|
|whenDeviceLocked|3|Os dados do aplicativo associados a essa política são criptografados quando o dispositivo é bloqueado|



