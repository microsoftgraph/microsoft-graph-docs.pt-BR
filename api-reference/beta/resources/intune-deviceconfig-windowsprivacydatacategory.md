---
title: Tipo de número windowsPrivacyDataCategory
description: Windows de categoria de dados de privacidade para acesso a dados de privacidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bae6c1ea277738940907e08986325e59ee7bcd79
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787283"
---
# <a name="windowsprivacydatacategory-enum-type"></a>Tipo de número windowsPrivacyDataCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows de categoria de dados de privacidade para acesso a dados de privacidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Nenhum nível de acesso especificado, nenhuma intenção. O dispositivo pode se comportar como em UserInControl ou ForceAllow. Pode depender dos dados de privacidade que foram acessados, Windows versões e outros fatores.|
|accountInfo|1|Permitir que os aplicativos acessem o nome do usuário, a imagem e outras informações de conta criadas na conta da Microsoft. Adicionado no Windows 10, versão 1607.|
|appsRunInBackground|2|Permitir que os aplicativos recebam informações, enviem notificações e fiquem atualizados, mesmo quando o usuário não as estiver usando. Esteja ciente de que, ao desabilitar aplicativos de comunicação (Email, Voz, etc.) do acesso em segundo plano, esses aplicativos podem ou não funcionar como estão com o acesso em segundo plano. Adicionado na Windows 10, versão 1703.|
|calendar|3|Permitir que os aplicativos acessem o calendário do usuário. Adicionado no Windows 10, versão 1607.|
|callHistory|4 |Permitir que os aplicativos acessem o histórico de chamada do usuário. Adicionado no Windows 10, versão 1607.|
|camera|5 |Permitir que os aplicativos acessem a câmera no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|contacts|6 |Permitir que os aplicativos acessem as informações de contato do usuário. Adicionado no Windows 10, versão 1607.|
|diagnosticsInfo|7 |Permitir que os aplicativos acessem informações de diagnóstico sobre outros aplicativos em execução. Adicionado na Windows 10, versão 1703.|
|email|8 |Permitir que os aplicativos acessem e enviem emails. Adicionado no Windows 10, versão 1607.|
|location|9 |Permitir que os aplicativos acessem os dados de localização precisos do usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|messaging|10 |Permitir que os aplicativos leiam ou enviem mensagens, texto ou MMS. Adicionado no Windows 10, versão 1607.|
|microphone|11 |Permitir que os aplicativos usem microfone no dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|motion|12 |Permitir que os aplicativos usem dados de movimento gerados no usuário do dispositivo. Adicionado no Windows 10, versão 1607.|
|notificações|13|Permitir que os aplicativos acessem as notificações do usuário. Adicionado no Windows 10, versão 1607.|
|phone|14 |Permitir que os aplicativos acessem dados de telefone e façam chamadas telefônicas. Adicionado no Windows 10, versão 1607.|
|rádios|15 |Permitir que os aplicativos usem rádios, incluindo Bluetooth, para enviar e receber dados. Adicionado no Windows 10, versão 1607.|
|tarefas|16 |Permitir que os aplicativos acessem o Agendador de Tarefas. Adicionado na Windows 10, versão 1703.|
|syncWithDevices|17 |Permitir que os aplicativos compartilhem e sincronizem automaticamente informações com dispositivos sem fio que não emparelham explicitamente com o dispositivo do usuário. Adicionado no Windows 10, versão 1607.|
|trustedDevices|18 |Permitir que os aplicativos acessem dispositivos confiáveis. Adicionado no Windows 10, versão 1607.|



