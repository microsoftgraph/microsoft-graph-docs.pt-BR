---
title: Tipo denum embeddedSIMDeviceStateValue
description: Descreve os vários estados para um código de ativação de SIM incorporado.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 82a7cf1d28976da03183618e0f47a26d125495d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046845"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>Tipo denum embeddedSIMDeviceStateValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve os vários estados para um código de ativação de SIM incorporado.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notEvaluated|0|Designa que o código de ativação do SIM incorporado é gratuito e disponível para ser atribuído a um dispositivo.|
|failed|1|Designa que o Serviço do Intune falhou ao entregar esse perfil a um dispositivo.|
|instalando|2|Designa que o código de ativação do SIM incorporado foi atribuído a um dispositivo e que o dispositivo está instalando o token.|
|instalado|3|Designa que o código de ativação do SIM incorporado foi instalado com êxito no dispositivo de destino.|
|exclusão|4 |Designa que o Serviço do Intune está tentando excluir o perfil do dispositivo.|
|erro|5 |Designa que há erro com esse perfil.|
|deleted|6 |Designa que o perfil é excluído do dispositivo.|
|removedByUser|7 |Designa que o perfil foi removido do dispositivo pelo usuário|



