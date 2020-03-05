---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 09cd5012d0b3a07a203b89ed76062232c47cfa82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530030"
---
# <a name="edgetelemetrymode-enum-type"></a>tipo de enumeração edgeTelemetryMode

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de dados de navegação enviados para a análise do Microsoft 365

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Padrão – nenhum dado de telemetria coletado ou enviado|
|Internet|1 |Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet|
|provedor|2 |Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet|
|intranetAndInternet|3 |Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet|



