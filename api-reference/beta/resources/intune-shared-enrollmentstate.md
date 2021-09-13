---
title: Tipo de número de enrollmentState
description: Ainda não documentado
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f06cb39e94dd526368b237b04d0bfefd9d68d095
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046607"
---
# <a name="enrollmentstate-enum-type"></a>Tipo de número de enrollmentState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O estado de registro do dispositivo é desconhecido|
|inscrito|1|O dispositivo está inscrito.|
|pendingReset|2|Inscrito, mas ele é inscrito por meio do perfil de registro e o perfil inscrito é diferente do perfil atribuído.|
|failed|3|Não registrado e há registro de falha no registro.|
|notContacted|4 |O dispositivo é importado, mas não está inscrito.|
|blocked|5 |O dispositivo está inscrito como sem usuário, mas está impedido de mudar para o registro do usuário porque o aplicativo falhou na instalação.|



