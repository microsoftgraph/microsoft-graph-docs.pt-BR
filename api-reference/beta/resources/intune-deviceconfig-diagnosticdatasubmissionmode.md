---
title: tipo denum diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2d4aa4818e018cecbf56f37936b84105a6162495
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791195"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo denum diagnosticDataSubmissionMode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria de diagnóstico e uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário desem conjunto.|
|Nenhuma|1|Nenhum dado de telemetria é enviado de componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. Usar essa configuração em outros dispositivos é equivalente à definição do valor 1.|
|basic|2|Envia dados básicos de telemetria.|
|enhanced|3|Envia dados de telemetria aprimorados, incluindo dados de uso e insights.|
|full|4 |Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|



