---
title: Tipo denum win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90eb7ed2c3f7568dfd4a69a4ffab8c52b7d79adb
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451349"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>Tipo denum win32LobAppRestartBehavior

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de ação de reinicialização.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|basedOnReturnCode|0|O Intune reiniciará o dispositivo após executar a instalação do aplicativo se a operação retornar um código de reinicialização.|
|allow|1|O Intune não tomará nenhuma ação específica sobre códigos de reinicialização resultantes de instalações do aplicativo. O Intune não tentará suprimir reinicializações para aplicativos MSI.|
|suppress|2|O Intune tentará suprimir reinicializações para aplicativos MSI.|
|force|3|O Intune força o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.|



