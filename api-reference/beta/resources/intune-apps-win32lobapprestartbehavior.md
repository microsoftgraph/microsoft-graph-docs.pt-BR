---
title: Tipo denum win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d850410b5380864988b9bd43abed41d9729138dbecd7d11f615da063a2b21c7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153255"
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
|allow|1 |O Intune não tomará nenhuma ação específica sobre códigos de reinicialização resultantes de instalações do aplicativo. O Intune não tentará suprimir reinicializações para aplicativos MSI.|
|suppress|2|O Intune tentará suprimir reinicializações para aplicativos MSI.|
|force|3 |O Intune força o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.|




