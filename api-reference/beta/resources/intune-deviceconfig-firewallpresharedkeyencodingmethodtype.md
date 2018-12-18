---
title: tipo de enum firewallPreSharedKeyEncodingMethodType
description: Valores possíveis para firewallPreSharedKeyEncodingMethod
author: tfitzmac
ms.openlocfilehash: 3ed2456f54bd27a3efa04d959edba48f7c100692
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324929"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>tipo de enum firewallPreSharedKeyEncodingMethodType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallPreSharedKeyEncodingMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|none|1|Chave pré compartilhada não é codificado. Em vez disso, ele é mantido em seu formato de caractere largo|
|utF8|2|Codificar a chave pré compartilhada usando a codificação UTF-8|





