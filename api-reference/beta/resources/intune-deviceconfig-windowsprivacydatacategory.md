---
title: tipo de enumeração windowsPrivacyDataCategory
description: Especificador de categoria de dados de privacidade do Windows para acesso a dados de privacidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89f9f74c61888e9acbf40f8059444d41cef8afae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525282"
---
# <a name="windowsprivacydatacategory-enum-type"></a>tipo de enumeração windowsPrivacyDataCategory

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especificador de categoria de dados de privacidade do Windows para acesso a dados de privacidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Nenhum nível de acesso especificado, sem tentativas. O dispositivo pode se comportar como no UserInControl ou no ForceAllow. Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|accountInfo|1 |Permite que aplicativos acessem o nome do usuário, a imagem e outras informações da conta criadas na conta da Microsoft. Adicionado no Windows 10, versão 1607.|
|appsRunInBackground|2 |Permitir que os aplicativos recebam informações, enviem notificações e permaneçam atualizados, mesmo quando o usuário não estiver usando-os. Lembre-se de que ao desabilitar os aplicativos de comunicação (email, voz, etc.) do acesso em segundo plano, esses aplicativos podem ou não funcionar como estão com o acesso em segundo plano. Adicionado no Windows 10, versão 1703.|
|calendar|3 |Permitir que aplicativos acessem o calendário do usuário. Adicionado no Windows 10, versão 1607.|
|callHistory|4 |Permitir que aplicativos acessem o histórico de chamadas do usuário. Adicionado no Windows 10, versão 1607.|
|Câmara|5 |Permitir que os aplicativos acessem a câmera no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|contatos|6 |Permitir que aplicativos acessem as informações de contato do usuário. Adicionado no Windows 10, versão 1607.|
|diagnosticsInfo|7 |Permitir que aplicativos acessem informações de diagnóstico sobre outros aplicativos em execução. Adicionado no Windows 10, versão 1703.|
|email|8 |Permitir que os aplicativos acessem e enviem emails. Adicionado no Windows 10, versão 1607.|
|location|9 |Permitir que os aplicativos acessem os dados de local preciso do usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|SMS|10 |Permitir que os aplicativos leiam ou enviem mensagens, texto ou MMS. Adicionado no Windows 10, versão 1607.|
|microfone|11 |Permitir que os aplicativos usem o microfone no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|movimento|12 |Permitir que os aplicativos usem dados de movimento gerados no usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|por|13 |Permitir que aplicativos acessem notificações do usuário. Adicionado no Windows 10, versão 1607.|
|phone|14 |Permitir que aplicativos acessem dados de telefone e façam chamadas telefônicas. Adicionado no Windows 10, versão 1607.|
|rádios|15 |Permitir que os aplicativos usem rádios, incluindo Bluetooth, para enviar e receber dados. Adicionado no Windows 10, versão 1607.|
|tarefas|16 |Permitir que aplicativos acessem o Agendador de tarefas. Adicionado no Windows 10, versão 1703.|
|syncWithDevices|17 |Permita que os aplicativos compartilhem e sincronizem informações com dispositivos sem fio que não sejam explicitamente emparelhados com o dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|trustedDevices|18 |Permitir que aplicativos acessem dispositivos confiáveis. Adicionado no Windows 10, versão 1607.|





