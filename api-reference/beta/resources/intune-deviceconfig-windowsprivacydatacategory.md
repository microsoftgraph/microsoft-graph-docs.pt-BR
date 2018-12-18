---
title: tipo de enum windowsPrivacyDataCategory
description: Especificador de categoria Windows privacidade dados para acesso aos dados de privacidade.
author: tfitzmac
ms.openlocfilehash: f5a9f0fc23e7fa5f3036b8653609db694f6932dd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304946"
---
# <a name="windowsprivacydatacategory-enum-type"></a>tipo de enum windowsPrivacyDataCategory

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Especificador de categoria Windows privacidade dados para acesso aos dados de privacidade.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Nenhum nível de acesso não especificado, nenhum propósitos. Dispositivo pode se comportam tanto como UserInControl ou ForceAllow. Ele pode depender os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|accountInfo|1|Permitir que o nome do usuário do access apps, imagem e outras informações de conta criada na conta da Microsoft. Adicionado no Windows 10, versão 1607.|
|appsRunInBackground|2|Permitir aplicativos receber informações, enviar notificações e mantenha-se atualizado, mesmo quando o usuário não está usando a eles. Lembre-se de que quando desabilitando os aplicativos de comunicação (Email, voz, etc.) contra o acesso de plano de fundo esses aplicativos podem, ou talvez não funcione como estão com o acesso de plano de fundo. Adicionado ao Windows 10, versão 1703.|
|calendário|3|Permitir que o calendário do usuário do access apps. Adicionado no Windows 10, versão 1607.|
|callHistory|4|Permitir que o histórico de chamadas do usuário de acesso de aplicativos. Adicionado no Windows 10, versão 1607.|
|câmera|5|Permitem que aplicativos acessar a câmera no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|contatos|6|Permitir que as informações de contato do usuário de acesso de aplicativos. Adicionado no Windows 10, versão 1607.|
|diagnosticsInfo|7|Permitem que aplicativos acessar informações de diagnóstico sobre outros aplicativos em execução. Adicionado ao Windows 10, versão 1703.|
|email|8|Permitir que o acesso de aplicativos e enviar email. Adicionado no Windows 10, versão 1607.|
|location|9|Permitem que aplicativos acessar os dados de localização precisas do usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|mensagens|10|Permitem que aplicativos ler ou enviar mensagens, texto ou MMS. Adicionado no Windows 10, versão 1607.|
|microfone|11|Permitem que aplicativos use microfone no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|movimento|12|Permitem que aplicativos usam dados de movimento gerados no usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|notificações|13|Deixe as notificações do usuário do access apps. Adicionado no Windows 10, versão 1607.|
|phone|14|Permitir que o access apps dados de telefone e fazer chamadas telefônicas. Adicionado no Windows 10, versão 1607.|
|rádios|15|Permitem que aplicativos use rádios, incluindo Bluetooth, para enviar e receber dados. Adicionado no Windows 10, versão 1607.|
|tarefas|16|Acesso permitem que aplicativos Agendador de tarefas. Adicionado ao Windows 10, versão 1703.|
|syncWithDevices|17|Permitem que aplicativos compartilhar automaticamente e sincronizar informações com dispositivos sem fio que não explicitamente emparelhar com o dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|trustedDevices|18|Permitem que aplicativos acessar dispositivos confiáveis. Adicionado no Windows 10, versão 1607.|





