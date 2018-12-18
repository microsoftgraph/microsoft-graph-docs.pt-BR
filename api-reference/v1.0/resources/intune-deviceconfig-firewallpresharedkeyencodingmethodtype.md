---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
ms.openlocfilehash: b8ab119c58aec6e62c0a32ccf310f43eab029573
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343586"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>tipo de enum firewallPreSharedKeyEncodingMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallPreSharedKeyEncodingMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|none|1|Chave pré compartilhada não é codificado. Em vez disso, ele é mantido em seu formato de caractere largo|
|utF8|2|Codificar a chave pré compartilhada usando a codificação UTF-8|



