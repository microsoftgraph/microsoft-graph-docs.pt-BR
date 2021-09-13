---
title: Tipo de número managedAppFlaggedReason
description: O motivo pelo qual um usuário foi sinalizado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b139ce9aaf192473d835a001fd71d9dfca710d40
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075085"
---
# <a name="managedappflaggedreason-enum-type"></a>Tipo de número managedAppFlaggedReason

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O motivo pelo qual um usuário foi sinalizado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Nenhum problema.|
|rootedDevice|1|O registro do aplicativo está sendo executado em um dispositivo rooted/desbloqueado.|
|androidBootloaderUnlocked|2|O registro do aplicativo está sendo executado em um dispositivo Android no qual o carregador de inicialização é desbloqueado.|
|androidFactoryRomModified|3|O registro do aplicativo está sendo executado em um dispositivo Android no qual a ROM de fábrica foi modificada.|



