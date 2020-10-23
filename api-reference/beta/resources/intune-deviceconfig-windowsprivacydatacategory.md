---
title: tipo de enumeração windowsPrivacyDataCategory
description: Especificador de categoria de dados de privacidade do Windows para acesso a dados de privacidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 302b683086287e086bd52314ecbb1346bb6f0aa2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684859"
---
# <a name="windowsprivacydatacategory-enum-type"></a>tipo de enumeração windowsPrivacyDataCategory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especificador de categoria de dados de privacidade do Windows para acesso a dados de privacidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Nenhum nível de acesso especificado, sem tentativas. O dispositivo pode se comportar como no UserInControl ou no ForceAllow. Pode depender que os dados de privacidade foram acessados, versões do Windows e outros fatores.|
|accountInfo|1|Permite que aplicativos acessem o nome do usuário, a imagem e outras informações da conta criadas na conta da Microsoft. Adicionado no Windows 10, versão 1607.|
|appsRunInBackground|duas|Permitir que os aplicativos recebam informações, enviem notificações e permaneçam atualizados, mesmo quando o usuário não estiver usando-os. Lembre-se de que ao desabilitar os aplicativos de comunicação (email, voz, etc.) do acesso em segundo plano, esses aplicativos podem ou não funcionar como estão com o acesso em segundo plano. Adicionado no Windows 10, versão 1703.|
|calendar|3D|Permitir que aplicativos acessem o calendário do usuário. Adicionado no Windows 10, versão 1607.|
|callHistory|4 |Permitir que aplicativos acessem o histórico de chamadas do usuário. Adicionado no Windows 10, versão 1607.|
|Câmara|5 |Permitir que os aplicativos acessem a câmera no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|contacts|6 |Permitir que aplicativos acessem as informações de contato do usuário. Adicionado no Windows 10, versão 1607.|
|diagnosticsInfo|7 |Permitir que aplicativos acessem informações de diagnóstico sobre outros aplicativos em execução. Adicionado no Windows 10, versão 1703.|
|email|8 |Permitir que os aplicativos acessem e enviem emails. Adicionado no Windows 10, versão 1607.|
|location|9 |Permitir que os aplicativos acessem os dados de local preciso do usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|SMS|10 |Permitir que os aplicativos leiam ou enviem mensagens, texto ou MMS. Adicionado no Windows 10, versão 1607.|
|microfone|11|Permitir que os aplicativos usem o microfone no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|movimento|12 |Permitir que os aplicativos usem dados de movimento gerados no usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|por|13 |Permitir que aplicativos acessem notificações do usuário. Adicionado no Windows 10, versão 1607.|
|phone|14 |Permitir que aplicativos acessem dados de telefone e façam chamadas telefônicas. Adicionado no Windows 10, versão 1607.|
|rádios|15 |Permitir que os aplicativos usem rádios, incluindo Bluetooth, para enviar e receber dados. Adicionado no Windows 10, versão 1607.|
|tarefas|16 |Permitir que aplicativos acessem o Agendador de tarefas. Adicionado no Windows 10, versão 1703.|
|syncWithDevices|17 |Permita que os aplicativos compartilhem e sincronizem informações com dispositivos sem fio que não sejam explicitamente emparelhados com o dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|trustedDevices|18 |Permitir que aplicativos acessem dispositivos confiáveis. Adicionado no Windows 10, versão 1607.|





