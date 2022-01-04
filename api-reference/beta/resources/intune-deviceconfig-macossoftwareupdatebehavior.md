---
title: Tipo de número macOSSoftwareUpdateBehavior
description: Atualize as opções de comportamento para atualizações de software macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a0fa894d17e126287ccb1e1c63e36160cf2dcd3e
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712079"
---
# <a name="macossoftwareupdatebehavior-enum-type"></a>Tipo de número macOSSoftwareUpdateBehavior

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as opções de comportamento para atualizações de software macOS.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Não configurado.|
|Padrão.|1|Baixe e/ou instale a atualização de software, dependendo do estado atual do dispositivo.|
|downloadOnly|2|Baixe a atualização de software sem instalá-la.|
|installASAP|3|Instale uma atualização de software já baixada.|
|notifyOnly|4|Baixe a atualização de software e notifique o usuário por meio da App Store.|
|installLater|5|Baixe a atualização de software e instale-a posteriormente.|




