---
title: Tipo denum win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a40d6a0de3cb23173d8b3e454e0a25d2df53dc0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009263"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>Tipo denum win32LobAppRestartBehavior

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de ação de reinicialização.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|basedOnReturnCode|0|O Intune reiniciará o dispositivo após executar a instalação do aplicativo se a operação retornar um código de reinicialização.|
|allow|1|O Intune não tomará nenhuma ação específica sobre códigos de reinicialização resultantes de instalações do aplicativo. O Intune não tentará suprimir reinicializações para aplicativos MSI.|
|suppress|2|O Intune tentará suprimir reinicializações para aplicativos MSI.|
|force|3|O Intune força o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.|



