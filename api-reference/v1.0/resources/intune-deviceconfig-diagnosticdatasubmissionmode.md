---
title: tipo denum diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cc92f564c323d3a0d7303b1074c523f158a96979
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445135"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo denum diagnosticDataSubmissionMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário desem conjunto.|
|none|1|Nenhum dado de telemetria é enviado de componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. Usar essa configuração em outros dispositivos é equivalente à definição do valor 1.|
|basic|2|Envia dados básicos de telemetria.|
|enhanced|3|Envia dados de telemetria aprimorados, incluindo dados de uso e insights.|
|full|4 |Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|



