---
title: Tipo de enumeração diagnosticDataSubmissionMode
description: Permita que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4befef2c9a4e447869a989aad27ddb5ca1641c44
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735114"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>Tipo de enumeração diagnosticDataSubmissionMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permita que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Userdefined|0|Permitir que o usuário defina.|
|none|1|Nenhum dado de telemetria é enviado dos componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. Usar essa configuração em outros dispositivos é equivalente a definir o valor de 1.|
|Basic|2|Envia dados de telemetria básicos.|
|Reforçada|3|Envia dados de telemetria aprimorados, incluindo dados de uso e insights.|
|Cheio|4|Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|





